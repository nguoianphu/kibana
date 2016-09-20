# Kibana 4.6

# Windows development


## Run and dev

````
git clone https://github.com/nguoianphu/kibana.git

git checkout 4.6

npm config set proxy http://proxy.company.com:8080
npm config set https-proxy http://proxy.company.com:8080

npm install

## Note for chromedriver
## Put the chromedriver_win32.zip to a http server (http://npm.taobao.org/mirrors/chromedriver)
## set CHROMEDRIVER_CDNURL=http://npm.taobao.org/mirrors/chromedriver
## npm install chromedriver


## Can not run elasticsearch because it doesn't support Kibana 4.6.x
## npm run elasticsearch
## Have to download elasticsearch and start it separately

## Can start Kibana by npm on Windows
## npm start

bin/kibana.bat --dev

bin/kibana.bat --dev --no-ssl

````


## Build

````
## install Grunt
## npm install -g grunt-cli

grunt build

# or 

grunt build --force --verbose

# or

npm run build

````