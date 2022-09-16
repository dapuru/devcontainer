# Devcontainer

## What is a Devcontainer?

"The Visual Studio Code Remote - Containers extension lets you use a Docker container as a full-featured development environment. It allows you to open any folder inside (or mounted into) a container and take advantage of Visual Studio Code's full feature set. A devcontainer.json file in your project tells VS Code how to access (or create) a development container with a well-defined tool and runtime stack. This container can be used to run an application or to separate tools, libraries, or runtimes needed for working with a codebase." (https://code.visualstudio.com/docs/remote/containers)

For more information check:<br>
used eg. in: https://blogs.sap.com/2022/01/27/boosting-tutorial-ux-with-dev-containers-part-1-challenge-and-base-solution/<br>
see also: https://code.visualstudio.com/docs/remote/create-dev-container<br>
https://github.com/devcontainers <br>

## Why Devcotainer?

"This means that you can seamlessly switch your entire development environment just by connecting to a different container." (https://code.visualstudio.com/docs/remote/containers)

eg. for developing
- CDS
- UI5
- ...

## Docker vs. Podman

"Podman is a daemonless, open source, Linux native tool designed to make it easy to find, run, build, share and deploy applications using Open Containers Initiative (OCI) Containers and Container Images. Podman provides a command line interface (CLI) familiar to anyone who has used the Docker Container Engine. Most users can simply alias Docker to Podman (alias docker=podman) without any problems." (https://docs.podman.io/en/latest/index.html)

"Unlike Docker, which uses the dockerd daemon to manage all the containers under its control, Podman is daemonless. Therefore, there’s no persistent connection to some long-living process, removing the single point of failure problem in Docker, where an abrupt crash in the daemon process can kill running containers or cause them to become orphaned." (https://blog.logrocket.com/top-docker-alternatives-2022/)

see:
https://www.liquidweb.com/kb/podman-vs-docker/ <br>
https://www.theserverside.com/blog/Coffee-Talk-Java-News-Stories-and-Opinions/When-to-use-Docker-vs-Podman-A-developers-perspective <br>
https://medium.com/technopanti/docker-vs-podman-c03359fabf77 <br>
https://blog.logrocket.com/top-docker-alternatives-2022/ <br>
https://opensource.com/article/18/10/podman-more-secure-way-run-containers <br>

Podman:
- Compatibility to docker (alias docker='podman') <br>
- deamonless (no dockerd) <br>
- rootless containers possible <br>

Or to say it in another way: Docker is not the holy grail - there are ways to do containerization according to the OCI standard (https://opencontainers.org/), more secure, without a daemon, license-stuff...

See also: "Series: Dockerless on mkdev.me" for more pros and cons: (https://mkdev.me/posts/dockerless-part-1-which-tools-to-replace-docker-with-and-why)

## Podman installation

https://podman.io/getting-started/installation <br>
https://buildah.io/

sudo pacman -S podman buildah

"By default, images are stored in the /var/lib/containers directory when Podman is run by the root user. For standard users, images are typically stored in $HOME/. local/share/containers/storage/ ." (https://docs.oracle.com/en/operating-systems/oracle-linux/podman/podman-ConfiguringStorageforPodman.html)

## What does this repo provide?
I'll collect all my used devcontainer config files in this place. 


## Further information
https://blog.daniel-purucker.com/vscode-devcontainer-part-1/ <br>
https://blog.daniel-purucker.com/vscode-devcontainer-part-2/ <br>
https://github.com/devcontainers
