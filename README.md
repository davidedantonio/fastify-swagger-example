# Fastify Swagger Example

## Prerequisities

You need to have pre-installed on your machine
- MongoDB
- Node.js and npm

If you don't want to install MongoDB on your machine use Docker and run from command license

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

Execute `npm install` an install all dependecies.
