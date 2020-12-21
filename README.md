# Nuxt.js / Firebase Template

Nuxt.js SSR app template for deploying on Firebase. 

[Demo](https://benmayer-nuxt-firebase.web.app/)

## How to install

1. Clone the Repository
1. Set the default project in .firebaserc 
1. Install Firebase CLI, Login and set the defualt project

    ### Firebase Setup
    ```bash
    # Install Firebase CLI 
    $ npm install -g firebase-tools

    # Login 
    firebase login

    # Set defualt project 
    firebase use --add

    ```
1. Install dependencies, follow the build setup below:

    ### Build Setup

    ```bash

    # install dependencies for Nuxt.js
    $ cd src && yarn install

    # install dependencies for Firebase 
    $ cd firebase &&  yarn install

    # genereate Nuxt.js files for production and launch server
    $ yarn build

    # copy client files from nuxt build and static files to firebase public directory
    $ yarn predeploy

    # deploy Firebase to production
    $ firbese deploy

    # serve local Nuxt.js app with hot reload at localhost:3000
    $ yarn dev
    ```

For detailed instructions how this works, check out the instructions here: [Building a Nuxt.js SSR app deploying it to firebase functions](https://ben-mayer.com/blog/a-blog-built-using-nuxtjs-and-firebase/)

For detailed explanation for Nuxt.js, check out [Nuxt.js docs](https://nuxtjs.org).

For detailed explanation for Firebase, check out [Firebase web docs](https://firebase.google.com/docs/web/setup).

