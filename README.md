# Atomist 'gokit-editors'

[![Slack Status](https://join.atomist.com/badge.svg)](https://join.atomist.com)

This [Rug](http://docs.atomist.com/) archive contains editors for
a [Go kit][go-kit] projects.

[go-kit]: https://github.com/go-kit/kit

## Rugs

### AddGokitMicroserviceDockerfile

The AddGokitMicroserviceDockerfile Editor adds an appropriate [Docker][docker] [Dockerfile][dockerfile] to an existing [Gokit][go-kit] project.

[go-kit]: https://github.com/go-kit/kit
[docker]: https://www.docker.com/
[dockerfile]: https://docs.docker.com/engine/reference/builder/

#### Prerequisites

There are no prerequisites to running this editor.

#### Parameters

To run this editor you must supply the following parameters.

Name | Required | Default | Description
-----|----------|---------|------------
`maintainer_name` | Yes | |  Name of the project maintainer to be used in the resulting Dockerfile.
`maintainer_email` | Yes | | The project maintainer's email address to be used in the resulting Dockerfile.

#### Running

Run it as follows:

```
$ cd parent/directory
$ rug edit atomist-rugs:gokit-rest-service:AddGokitMicroserviceDockerfile \
    maintainer_name="The Dude" \
    maintainer_email="thedude@hollywoodstarlanes.com"
```

This will create an appropriate [Docker][docker] [Dockerfile][dockerfile] in a `docker` directory named `pet-shop-service`. If you are happy
with the change, commit the changes.

[docker]: https://www.docker.com/
[dockerfile]: https://docs.docker.com/engine/reference/builder/

```
$ git add .
$ git commit -m 'Dockerfile added by Atomist'
```

---
Created by Atomist. Need Help? <a href="https://join.atomist.com/">Join our Slack team</a>
