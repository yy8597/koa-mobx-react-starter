**WORK IN PROGRESS - DON'T CLONE YET**

# koa-mobx-react-bootstrap

Along with aiming to use the bleeding-edge of JavaScript (within reason- and all thanks to [Babel](https://babeljs.io/)), this repository represents a choice of frameworks and libraries I think work well together for an enjoyable NodeJS and frontend coding experience.

A short rundown of the various technologies:
###Server
- [Koa](http://koajs.com/) - A bleeding-edge Node server framework, using the async-await syntax. Server code compiled back to a widely adopted standard of JavaScript using Babel.
- [Pug](https://github.com/pugjs) (formerly Jade) for views - Concise HTML view engine, into which we slot in our React-generated HTML

###Crossover
- [MobX](https://github.com/mobxjs/mobx "MobX") - Hold state initially on the server, and then pass it over to the client
- [ReactJS](https://facebook.github.io/react/) - Build views on the server and inject functionality into those already built views on the client

###Client
- Javascript compiled with [Webpack](https://webpack.github.io/) - A bundler that reads your entry JavaScript and various other files and creates a distribution build of them (using various options and plugins) for efficient client-side delivery
- Client Javascript mostly involves more React and MobX goodness for great interaction

##Get Going:

For starters:

```
npm install
```

Then to start the development server (which is what you want most of the time)

```
npm run dev
```

And to start the production server is the usual `npm start`, but the code has to be built first, so:
```
npm run build
npm start
```
Or for quick production testing `npm run buildstart`

Before deployment to a production server, your code should always be built first- so that the default `npm start` can be used to spin up quickly.