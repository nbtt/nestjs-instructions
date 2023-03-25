English - [Tiếng Việt](Readme.md)

# Guide to install and get started with Nest.js

Nest.js is one of the Node.js framework that helps building scalable backend system quickly and efficiently.

For beginners, it can takes a long time to install and learn how to use Nest.js. Therefore, this document will guide you how to install Node.js, Nest.js and some tools that helps building backend system, e.g. Postman for testing API. At the end of the document, there are also instructions to intialize and get started on a new project.

## Table of contents

- [Guide to install and get started with Nest.js](#guide-to-install-and-get-started-with-nestjs)
  - [Table of contents](#table-of-contents)
  - [Install Nest.js and related softwares](#install-nestjs-and-related-softwares)
  - [Get started with Nest.js](#get-started-with-nestjs)
    - [Initialize new project](#initialize-new-project)
    - [Create a module](#create-a-module)
    - [Create a controller](#create-a-controller)
    - [Create a service](#create-a-service)
    - [Create a CRUD resource](#create-a-crud-resource)
  - [Reference links](#reference-links)


## Install Nest.js and related softwares

Choose your operating system: [Windows](en/Tutorial-Windows.md) - [Linux](en/Tutorial-Linux.md) - [macOS](en/Tutorial-macOS.md)

## Get started with Nest.js

This section includes commonly used commands for intializing and working with Nest.js project.

### Initialize new project

Below commands will initialize a new project, then build and run created project.

```sh
nest new my-nest-project
cd my-nest-project
npm run start:dev
```

Access to [http://localhost:3000](http://localhost:3000) on browser to view the running application.

### Create a module

A project is organized into modules. Each module contains related components in the project.

To create a module, run the command

```sh
nest generate module my-module
```

Or

```sh
nest g mo my-module
```

### Create a controller

Controller is the component responsible for handling requests and returning responses to client.

To create a controller, run the command

```sh
nest generate controller my-controller
```

Or

```sh
nest g co my-controller
```

### Create a service

Nest.js has an important concept called provider, which is the object that can be injected as a dependency, that creates relationships between objects in a project. Service is a provider that is often used for handling logic or interacting with entities in the project.

To create a service, run the command

```sh
nest generate service my-service
```

Or

```sh
nest g s my-service
```

### Create a CRUD resource

CRUD resource is the resource and APIs to create, read, update and delete that resource in the system.

To create a CRUD resource, run the command

```sh
nest generate resource my-resource
```

Or

```sh
nest g res my-resource
```

## Reference links

- Nest.js documentation: [https://docs.nestjs.com/](https://docs.nestjs.com/)
- Nest.js video tutorial: [https://youtu.be/F_oOtaxb0L8](https://youtu.be/F_oOtaxb0L8)
- Details of Nest CLI: [https://docs.nestjs.com/cli/usages](https://docs.nestjs.com/cli/usages)
- Tutorial to deploy a Node.js project: [https://youtu.be/4Ga4c_amvY8](https://youtu.be/4Ga4c_amvY8)