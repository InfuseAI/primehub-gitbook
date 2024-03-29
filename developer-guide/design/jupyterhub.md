# JupyterHub

This document describes the integration of PrimeHub and JupyterHub.

### Concept

The whole magic happens in `jupyterhub_profiles.py`, which customizes the [kubespawner](https://github.com/jupyterhub/kubespawner). Here is the brief spawner logic

1. A user logs in to keycloak and postback the user profile to jupyterhub. (by OIDC flow)
2. Store the authentication data in the cookie.
3. Use the authentication data to query graphql to get the groups, instance types, images, datasets of the logged in user
4. The spawner renders the options in the spawner page
5. The user selects the options they would like to spawn and submits.
6.  By _kubespawner_ mechanism, assemble the jupyter pod's spec and spawn this pod.&#x20;

    <figure><img src="../../.gitbook/assets/jupyterhub_profiles.png" alt=""><figcaption></figcaption></figure>

### Main Classes

We customize the authenticator and spawner described in the [jupyterhub document](https://jupyterhub.readthedocs.io/en/stable/reference/technical-overview.html)

| Class             | Description                                                                                                                                              |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| OIDCAuthenticator | Implement `GenericOAuthenticator` with OIDC integration. It also provides `spawner` the authentication data of logged in users (in `pre_spawn_start()`). |
| PrimeHubSpawner   | Implementation `Kubespawner` with PrimeHub pod spawning logic.                                                                                           |

#### References

* [Kubespawner](https://github.com/jupyterhub/kubespawner)
* [Zero to JupyterHub with Kubernetes](https://zero-to-jupyterhub.readthedocs.io/en/latest/)
* [Keycloak Admin REST API](https://www.keycloak.org/docs-api/6.0/rest-api/index.html)
