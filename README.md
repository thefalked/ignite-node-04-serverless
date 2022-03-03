# Serverless - AWS Node.js Typescript

This project has been generated using the `aws-nodejs-typescript` template from the [Serverless framework](https://www.serverless.com/).

For detailed instructions, please refer to the [documentation](https://www.serverless.com/framework/docs/providers/aws/).

## Installation/deployment instructions

Depending on your preferred package manager, follow the instructions below to deploy your project.

> **Requirements**: NodeJS `lts/fermium (v.14.15.0)`. If you're using [nvm](https://github.com/nvm-sh/nvm), run `nvm use` to ensure you're using the same Node version in local and in your lambda's runtime.

### Install the serverless CLI

- Run `npm install -g serverless` to install the CLI

### Using NPM

- Run `npm i` to install the project dependencies
- Run `npm run dev` to start the development environment
- Run `npm run dynamodb:install` to install the database localy
- Run `npm run dynamodb:start` to run the dynamodb localy
- Run `serverless config credentials --provider aws --key=key_here --secret=secret_here` to set up the credentials. If you already have configured you can use the option `-o` at the end of the command to override the old one.
- Run `npm run deploy` to deploy on AWS

### Using Yarn

- Run `yarn` to install the project dependencies
- Run `yarn dev` to start the development environment
- Run `yarn dynamodb:install` to install the database localy
- Run `yarn dynamodb:start` to run the dynamodb localy
- Run `serverless config credentials --provider aws --key=key_here --secret=secret_here` to set up the credentials. If you already have configured you can use the option `-o` at the end of the command to override the old one.
- Run `yarn deploy` to deploy on AWS

### 3rd party libraries

- [json-schema-to-ts](https://github.com/ThomasAribart/json-schema-to-ts) - uses JSON-Schema definitions used by API Gateway for HTTP request validation to statically generate TypeScript types in your lambda's handler code base
- [middy](https://github.com/middyjs/middy) - middleware engine for Node.Js lambda. This template uses [http-json-body-parser](https://github.com/middyjs/middy/tree/master/packages/http-json-body-parser) to convert API Gateway `event.body` property, originally passed as a stringified JSON, to its corresponding parsed object
- [@serverless/typescript](https://github.com/serverless/typescript) - provides up-to-date TypeScript definitions for your `serverless.ts` service file
