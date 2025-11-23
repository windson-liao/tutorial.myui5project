# tutorial.myui5project
npm -g config set registry https://registry.npmjs.org/
npm -g config set strict-ssl false

export NODE_TLS_REJECT_UNAUTHORIZED=0

npm -g config set strict-ssl true


npm run start:myui5app

cf login -a https://api.cf.ap21.hana.ondemand.com

npm run build 
mbt build --mtar tutorial.myui5project.mtar
