# Fastify Swagger Example

## Prerequisities

You need to have pre-installed on your machine
- MongoDB
- Node.js and npm

If you don't want to install [MongoDB](https://www.mongodb.com/it) on your machine use [Docker](https://www.docker.com/) and run from command license

```
docker pull mongo:4.0.3
```

## Before you start

```
npm install fastify-cli --global
```

Full documentation for `fastify-cli` is here [https://github.com/fastify/fastify-cli](https://github.com/fastify/fastify-cli).

Then create the project skeleton with these commands

```
mkdir your-awesome-api
cd cyour-awesome-api
npm init
npx fastify-cli gen
```

After you have executed `npx fastify-cli gen` command, the directory will look like this:

```
your-awesome-api/
  ├── app.js
  ├── package.json
  ├── plugins
  │   ├── README.md
  │   └── support.js
  ├── services
  │   ├── example
  │   │   └── index.js
  │   ├── README.md
  │   └── root.js
  └── test
      ├── helper.js
      ├── plugins
      │   └── support.test.js
      └── services
          ├── example.test.js
          └── root.test.js
```

Execute `npm install` an install all dependecies. After, to proceed with example install theese dependencies:

```
npm install --save fastify-swagger fastify-mongodb
```

Create `.env` file and insert theese lines:

```
PORT=3001
MONGODB_URL=mongodb://localhost:27017/tables
```

## If you decided to use docker

If you have decided to use docker add in your `package.json` file following line under `script`

```
"mongo": "docker run -p 27017:27017 mongo:4.0.3"
```

In the future before you start the application run

```
npm run mongo
```

and your mongo server has started

## Be curious

Now you have a skeleton API and an example API (this project).

## Run this example project

From command line

- run `npm run mongo`
- run `npm run dev`

and check under `http://localhost:3001/documentation`.

Happy coding :heart:

# Useful documentation

[Fastify](https://www.fastify.io/)
[Fastify Mongo](https://github.com/fastify/fastify-mongodb)
[Fastify Swagger](https://github.com/fastify/fastify-swagger)
[Fastify Oauth](https://github.com/fastify/fastify-oauth2)
