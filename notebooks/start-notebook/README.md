# Start Notebook

### Overview

* `Instance Types`: The selection of instance types according to the current group context
* `Images`: The selection of images according to the current group context
* `User Limits`: The resources constraints are on the current user
* `Group Resources`: The resources dashboard indicates current used resource and the limit according to the current group context
* `Volumes`: Volumes are associated with the current group
* `Show advanced settings`: Display the advanced settings of launching Notebook

#### Launch

1. Log in `User Portal` with a user account, select `Notebooks` and click `Start My Server` to enter the spawner page.
2. Confirm if the current group is what you desire; switch the group by the `Group:` dropdown at the top of the right side.
3. Select an `Instance Type` for the resource allocation to this project. It lists instance types only within the context of the group.
4.  Select an `Image` which the project is based on. It lists images only within the context of the group.

    Accordingly, images are selectable only if `Types` of which match the selected `Instance Type` that guarantees hub is spawned with the proper image.

    **Group/System Image**

    From image selection, `i` hint indicates an image `Group` image or `System` image.
5. Enabled Advanced Settings if required. Click `Start Notebook`. Your Server environment would be instantiated. Once the Notebook is spawned, it will pop up a new tab.

{% hint style="info" %}
At very first time, browser will block the pop-up from PrimeHub by default, please allow the pop-up from PrimeHub. Click `Launch Notebook Server` to open Notebook in a new tab once the pop-up is allowed.
{% endhint %}

### Spawning

From Notebook tab, it shows the spawning progress.

Spawning can be cancelled by clicking `Cancel`.

### Notebook Logs

Logs are retrieved from Jupyter Pod since Notebook spawning to Notebook end. The logs can be viewed from `Logs` tab and be downloaded as a file _as long as Notebook is alive_. Once Notebook is terminated, logs are gone with it. In this case, we can only check latest logs cached by UI.

{% hint style="info" %}
Logs are shown when Notebook pod is being started or alive. If there is no running notebook, it shows `Error: cannot get log due to pods "jupyter-xxxx" not found`.
{% endhint %}

### Stop

Click `Shutdown Server`. It takes a short while to stop it.

### Notice

{% hint style="info" %}
If switching the current working group after the Notebook is launched, it indicates the Notebook is retained in the other group.
{% endhint %}

### Reference

Accessible Data Store from Notebook
