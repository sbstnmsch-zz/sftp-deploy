[![npm version](https://badge.fury.io/js/sftp-deploy.svg)](http://badge.fury.io/js/sftp-deploy) [![Build Status](https://travis-ci.org/sbstnmsch/sftp-deploy.svg?branch=master)](https://travis-ci.org/sbstnmsch/sftp-deploy)

# SFTP Deploy
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
