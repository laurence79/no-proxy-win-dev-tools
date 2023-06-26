# Some workarounds for overzealous proxies

## NVM

See [nvm-windows](https://github.com/coreybutler/nvm-windows)

### Installation

1. Remove existing installations of node
2. Run `nvm-setup.exe`
3. Explode `node_versions/v18.12.1/node.zip`
4. Copy the exploded folder into `%AppData%/Roaming/nvm/v18.12.1` so that `node.exe` is directly under v18.12.1
5. 
```bash
nvm use 18.12.1
npm i -g yarn
```
6. Profit


### Adding a new version

1. Create a directory under node_versions, e.g.
```sh
cd node_versions
mkdir v14.18.2
```
2. Download the binaries from nodejs.org
```sh
cd v14.18.2
curl \
  https://nodejs.org/download/release/v14.18.2/node-v14.18.2-win-x64.zip \
  --output node.zip
```
3. Commit and push
```sh
git add .
git commit -m "Added version 14.18.2"
git push
```