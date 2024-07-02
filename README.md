# Not Enough Commands

This package is just a way for me to easily add tons of predefined commands to a [discord.js-made](https://discord.js.org/) bot in just a second !

> For the moment, this package is made to extend the capabilities of the [bot.ts](https://github.com/bot-ts) framework, so make sure that your actually using this framework to build your bot !!

## Install

```bash
npm install @raph.dcst/notenoughcommands
```

## Setup

To start using the package, you need to run the following command, which will create a `nec.config.json` file at the root of your project : 

```bash
npx nec init
```

In your `nec.config.json`, you will find some options, such as you *commands source directory*, *namespaces source directory*, etc... This config file is set to work with the default structure of a **bot.ts project**. If you modified this project structure, you will have to manually set the parameters to ensure that the package works.

## Usage

To list all the availables commands, you can do : 

```bash
npx nec list
```

This will return a list of all the commands with their names and descriptions, like this : 

```
- "ping" -> Return the bot ping
- "ban" -> Ban a user
- etc...

```

To add a command to your project, you can do : 

```bash
npx nec add <command-name>

```

This will create two files named `<command-name>.ts` in : 
1. Your *namespace* directory (by default `./src/namespaces`)
2. Your *command* directory (by default `./src/commands`)

Those files contains all the necessary code to add the command to the bot. 

>You can modify them if needed, but keep in mind that these changes are not final and therefore will not be available the next time !

> If you want a command to be availale by everyone and at any time, please open a PR !


