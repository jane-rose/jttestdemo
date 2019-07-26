A Vue.js project

Build Setup
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run devserver

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
For detailed explanation on how things work, checkout the guide and docs for vue-loader.

Deploy snippet
Step 1: deploy to test server & test it in pretest environtment
ssh root@173.255.221.43
cd /usr/share/nginx/html/staticsnap/
git pull  # update newest code
npm run build-pretest

visit test.snapmaker.com confirm newest feature.
Step 2: compile online tar.gz
ssh root@173.255.221.43
cd /root/static-snapmakerX
git pull
npm run build-online
sh build.sh # create tar.gz

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
