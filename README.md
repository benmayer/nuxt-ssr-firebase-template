# Nuxt.js / Firebase Template

Nuxt.js SSR app template for deploying on Firebase. 

[Demo](https://benmayer-nuxt-firebase.web.app/)

## Build Setup

```bash
# install dependencies for nuxt 
$ cd src && yarn install

# install dependencies for firebase 
$ cd firebase &&  yarn install

# serve local Nuxt.js app with hot reload at localhost:3000
$ cd src && yarn dev

# genereate Nuxt.js files for production and launch server
$ cd src && yarn build

# copy generated Nuxt.js server files to Firebase functions folder for deployment
$ mkdir -p functions/.nuxt/dist/
$ cp -r src/.nuxt/dist/server functions/.nuxt/dist/

# copy generated Nuxt.js client files to Firebase public folder for deployment
$ mkdir -p public/_nuxt
$ cp -r src/.nuxt/dist/client/ public/_nuxt && cp -a src/static/. public/

# deploy Firebase to production
$ firbese deploy
```

For detailed instructions how this workm check out the instructions here: [Building a Nuxt.js SSR app deploying it to firebase functions](https://ben-mayer.com/blog/a-blog-built-using-nuxtjs-and-firebase/)

For detailed explanation for Nuxt.js, check out [Nuxt.js docs](https://nuxtjs.org).

For detailed explanation for Firebase, check out [Firebase web docs](https://firebase.google.com/docs/web/setup).

