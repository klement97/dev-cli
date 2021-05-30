# Dev CLI
Command line interface to boost the web development process.

## What is the main idea?
The main idea here is to avoid performing repetitive tasks in terminal.
This repetitive tasks includes starting the development server, restoring a database,
start a shell to a docker container and many more. By using this CLI you are able to use
the built in commands or add your own commands easily by following the already present
structure.

## Why BASH?
There are a ton of ready libraries to build a CLI easily in other languages like JavaScript, 
Python and many more. Especially the ones in JavaScript are easy to learn and develop.
I prefer to at least have the core structure of this project in BASH because
it is built exactly for this kind of work. Working in terminal means working in BASH or any other
shell languages. Although, I am always open to accept some scripts from other languages.
There are a lot things which you can not do in bash compared to high level languages.
So the door is open.

## Some challenges I have faced
The biggest challenge in this project is that you have to make some assumptions. Sometimes I've made
some small assumptions and sometimes bolder ones. My long term goal is to minimize these assumptions.
By doing that only I can reach out to more users.

## How to use the CLI?

### Installation
I wanted to make the installation a breeze and so I did.
Open your terminal and run the following command.

``` bash
bash -c "$(curl -fsSL https://raw.githubusercontent.com/klement97/dev-cli/main/install)"
```
After running it just type `dev` in your terminal and you will be able to see the help screen.

### Configuration
After successfully installing the Dev CLI the first step is to configure it.

```bash
dev configure
```

Configuration script will ask you some questions, after answering them the Dev CLI is ready to use.

### Usage
If you want to know what is Dev CLI capable of doing open a terminal and type ```dev```
In the screen you will see the standard help message listing all of the available commands
and their descriptions.

```bash
> dev

Developer CLI
Version: 0.1.0
https://github.com/klement97/dev-cli

Usage: dev [command]

Commands:
  configure           Configure the CLI to your use
  startb or b         Start the backend development server
  startf or f         Start the frontend development server
  restore_db or rdb   Restore the development database
  exec                Execute a given command in a given docker container
  *                   This help screen
  ```

For each one of the commands there is a bash script which is responsible for performing
all of the required tasks.

Copyright and License Information
---------------------------------

Copyright (c) 2021 Klement Omeri. All rights reserved.

See the [LICENSE](https://github.com/klement97/dev-cli/blob/main/LICENCE)
