# Install the basics
```
sudo apt update
sudo apt upgrade
sudo apt install nodejs npm

node --version
v10.24.0
```

# Install node version manager & latest npm

```
zplug install "lukechilds/zsh-nvm"

<startup new shell>

command -v nvm
> nvm

nvm ls-remote

>      v14.15.0   (LTS: Fermium)
       v14.15.1   (LTS: Fermium)
       v14.15.2   (LTS: Fermium)
       v14.15.3   (LTS: Fermium)
       v14.15.4   (LTS: Fermium)
       v14.15.5   (LTS: Fermium)
       v14.16.0   (Latest LTS: Fermium)
        v15.0.0
        v15.0.1
        v15.1.0
        v15.2.0
        v15.2.1
        v15.3.0
        v15.4.0
        v15.5.0
        v15.5.1
        v15.6.0
        v15.7.0
        v15.8.0
        v15.9.0
       v15.10.0
       v15.11.0
       v15.12.0
       v15.13.0

nvm install --lts
Installing latest LTS version.
Downloading and installing node v14.16.0...
Downloading https://nodejs.org/dist/v14.16.0/node-v14.16.0-linux-x64.tar.xz...
######################################################################################################## 100.0%
Computing checksum with sha256sum
Checksums matched!
Now using node v14.16.0 (npm v6.14.11)
Creating default alias: default -> lts/* (-> v14.16.0)

nvm install-latest-npm
Attempting to upgrade to the latest working version of npm...
* Installing latest `npm`; if this does not work on your node version, please report a bug!
/home/ben/.nvm/versions/node/v14.16.0/bin/npm -> /home/ben/.nvm/versions/node/v14.16.0/lib/node_modules/npm/bin/npm-cli.js
/home/ben/.nvm/versions/node/v14.16.0/bin/npx -> /home/ben/.nvm/versions/node/v14.16.0/lib/node_modules/npm/bin/npx-cli.js
+ npm@7.8.0
added 58 packages from 23 contributors, removed 241 packages and updated 194 packages in 7.487s
* npm upgraded to: v7.8.0

```

# Install auto-switcher for node
(DOESN'T SEEM TO WORK ON WSL)

```
npm install -g avn-nvm

added 31 packages, and audited 297 packages in 7s

25 vulnerabilities (8 low, 7 moderate, 10 high)

To address all issues, run:
  npm audit fix

Run `npm audit` for details.

```

# Set the node version to use in a given project

```
node --version > .node-version
```

# Setup yarn
```
npm -g install yarn

added 1 package, and audited 2 packages in 1s

found 0 vulnerabilities
```

# Initialise project
```
yarn init
yarn init v1.22.10
warning ../package.json: No license field
question name (typescript-experiments): 
question version (1.0.0): 
question description: Experimental project using yarn & typescript
question entry point (index.js): 
question repository url: 
question author: 
question license (MIT): 
question private: true
success Saved package.json
Done in 45.78s.
```

# Change to yarn 2 (aka yarn modern)
```
yarn set version berry
warning ../package.json: No license field
Resolving berry to a url...
Downloading https://github.com/yarnpkg/berry/raw/master/packages/berry-cli/bin/berry.js...
Saving it into /home/ben/typescript-experiments/.yarn/releases/yarn-berry.cjs...
Updating /home/ben/typescript-experiments/.yarnrc.yml...
Done!
```