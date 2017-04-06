# azure-appservice-static
Deploy static create-react-app site to azure AppService.

## Usage

Copy the following files to your repo root
```
.deployment
scripts/deploy.sh
web.config
```

Change your scripts in package.json to something like this:
```json
scripts": {
  "postinstall": "npm run build",
  "dev": "react-scripts start",
  "build": "react-scripts build",
  "test": "react-scripts test --env=jsdom",
  "eject": "react-scripts eject"
}
```

## Blog post

https://medium.com/@strid/host-create-react-app-on-azure-986bc40d5bf2#.pycfnafbg

## Special thanks

[The web.config is taken from this blogpost](https://medium.com/@to_pe/deploying-create-react-app-on-microsoft-azure-c0f6686a4321#.kvehlxn7k)
