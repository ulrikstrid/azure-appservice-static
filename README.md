# azure-appservice-static
Deploy static create-react-app site to azure AppService.

## Usage

Copy the following files to your repo root
```
.deployment
deploy.sh
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
