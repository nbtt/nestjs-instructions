# Install Nest.js and related softwares

This document is for macOS.

Other operating system: [Windows](Tutorial-Windows.md) - [Linux](Tutorial-Linux.md)

## Table of contents

- [Install Nest.js and related softwares](#install-nestjs-and-related-softwares)
  - [Table of contents](#table-of-contents)
  - [Installation](#installation)
    - [(Optional) Homebrew](#optional-homebrew)
    - [Node.js](#nodejs)
    - [Nest.js](#nestjs)
    - [Postman](#postman)
    - [Database](#database)
  - [Next step](#next-step)

## Installation

### (Optional) Homebrew

[Homebrew](https://brew.sh/index) is an open-source software package mangement system. Some software listed below could be installed by Homebrew.

Install Homebrew by the command

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

### Node.js

[Node.js](https://nodejs.org/en) is a server environment to run application written in Javscript. Nest.js is a framework on Node.js.

To install Node.js:

- Download Node.js installer at [https://nodejs.org/en/download](https://nodejs.org/en/download)
- Run the installer

Or run command ([Homebrew](#optional-homebrew) is required):

```sh
brew install node
```

After installation, verify by this command, if the versions of `npm` and `node` are displayed then the installation is success.

```sh
node --version
npm --version
```

### Nest.js

Install [Nest.js](https://nestjs.com/) by the command

```sh
npm i -g @nestjs/cli
```

After installation, verify by this command, if the version of `nest` is displayed then the installation is success.

```sh
nest --version
```

### Postman

[Postman](https://www.postman.com/) is a tool to work with APIs in order for testing and building the APIs.

![Postman](../images/postman-product-screen.svg "Image by: postman.com")

To install it:

- Download the installer at [https://www.postman.com/downloads/](https://www.postman.com/downloads/)
- Unzip the downloaded file
- Run extracted file

Or run the command ([Homebrew](#optional-homebrew) is required):

```sh
brew install --cask postman
```

### Database

Nest.js applications may need to work with database. To install one of commonly used database, please refer to below links:

- MySQL: [https://dev.mysql.com/doc/mysql-installation-excerpt/8.0/en/](https://dev.mysql.com/doc/mysql-installation-excerpt/8.0/en/)
- MongoDB: [https://www.mongodb.com/docs/manual/installation/#mongodb-installation-tutorials](https://www.mongodb.com/docs/manual/installation/#mongodb-installation-tutorials)
- PostgreSQL: [https://www.postgresql.org/docs/current/installation.html](https://www.postgresql.org/docs/current/installation.html)

## Next step

[Get started with Nest.js](../Readme.en.md#get-started-with-nestjs)