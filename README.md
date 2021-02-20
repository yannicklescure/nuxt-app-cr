# nuxt-app-cr

## Build Setup

```bash
# install dependencies
$ yarn install

# serve with hot reload at localhost:3000
$ yarn dev

# build for production and launch server
$ yarn build
$ yarn start

# generate static project
$ yarn generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
# nuxt-app-cr

### Build Step-by-step

```bash
# build nuxt app
$ yarn create nuxt-app nuxt-app-cr
$ cd nuxt-app-cr
$ yarn build
$ yarn start

# Github first commit
$ echo "# nuxt-app-cr" >> README.md
$ git init
$ git add README.md
$ git commit -m "first commit"
$ git branch -M main
$ git remote add origin git@github.com:yannicklescure/nuxt-app-cr.git
$ git push -u origin main

# Github push nuxt files
$ git status
$ git add .
$ git commit -m "initial nuxt commit"
$ git push origin main

# Heroku new new app
$ heroku apps:create nuxt-app-cr --region=eu
$ git push heroku main

# Heroku configuration fro nuxt app
$ heroku config:set HOST=0.0.0.0
$ heroku config:set NODE_ENV=production
$ touch Procfile
$ echo "web: nuxt start" >> Procfile
$ git add .
$ git commit -am "improve code + fix bugs"
$ git push origin main
$ git push heroku main

# Launch Sublime Text
$ stt
```
