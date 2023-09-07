# mojo-exploration
Trying out the new coding language "mojo"

## Install + setup
- Install [Docker Desktop](https://docs.docker.com/desktop/install/mac-install/)
- Install [VSCode](https://code.visualstudio.com/download)
- Install [VSCode Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
- Install [Mojo VSCode Extension](https://marketplace.visualstudio.com/items?itemName=modular-mojotools.vscode-mojo)
- In VS Code, click Open a Remote Window  in the bottom-left corner, and select New Dev Container. Then type “Ubuntu”, press Enter, and select Create Dev Container.
- Once the container starts, select Terminal > New Terminal and install the Modular CLI by running the following command:
```
curl https://get.modular.com | \
  MODULAR_AUTH=mut_ab3e55c56d40413981386e28b0abdc12 \
  sh -
```
- `modular install mojo`
- `echo 'export MODULAR_HOME="/home/vscode/.modular"' >> ~/.bashrc`
- `echo 'export PATH="/home/vscode/.modular/pkg/packages.modular.com_mojo/bin:$PATH"' >> ~/.bashrc`
- `source ~/.bashrc`
- `mojo --version` should now work
- `mojo --help` should now work