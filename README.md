# SFTP Deploy

[![Greenkeeper badge](https://badges.greenkeeper.io/sbstnmsch/sftp-deploy.svg)](https://greenkeeper.io/)
Deploy a path to a remote server via SFTP

# Install
```
$ npm install -D sftp-deploy
```

# Setup
Deploy via npm-script in *package.json*:
```
  "scripts": {
    ...
    "deploy": "sftp-deploy"
  }
```

# Deploy via CI - Continous integration
In your build environment (i.e. travis-ci, teamcity, bamboo)
setup the following environment variables:
```
DEPLOY_HOST=192.168.1.42
DEPLOY_USER=deploymentuser
DEPLOY_PASSWORD=!deploymentpa5swOrd
DEPLOY_PATH=/srv/httpd/htdocs
DEPLOY_SRC=./dist
DEPLOY_PORT=22 # Optional
```
