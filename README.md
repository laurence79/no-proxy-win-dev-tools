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

Profit