# Tutorial

PrimeHub integrates [Seldon](https://docs.seldon.io/projects/seldon-core/en/latest/) as the model deployment solution. Seldon is a container-based solution and provides a common way to package different ML framework's by different programming languages as container images. We also use the Seldon Predition API to communicate.

To deploy a model, we need to provide a model image. There are two ways to prepare the model image.

1. **Pre-Packaged Servers**: Users use a pre-packaged server as the model image. PrimeHub provides several ready-to-use pre-packaged servers. To deploy a model, a model URI is required to indicate where to download the model files.
2. **Package Model by Language Wrapper**: Users build a model image with model files embedded. It is an advanced but flexible way to deploy a model. Seldon provides several language wrappers to package models from different languages.

In the following tutorials, we will present several different ways to deploy models.

* [Deploy a Model by Pre-packaged Server](model-by-pre-packaged-server.md)
* [Deploy a Model by Pre-packaged Server (PHFS)](model-by-pre-packaged-server-phfs.md)
* [Deploy a Model by Image built from Language Wrapper](../package-from-language-wrapper/)
