# mongo-realm-react-todo-tracker

# 🚀 Javascript full-stack 🚀

https://github.com/coding-to-music/mongo-realm-react-todo-tracker

https://mongo-realm-react-todo-frontend.vercel.app

From / By https://www.mongodb.com/docs/realm/tutorial/backend-app/

https://www.mongodb.com/docs/realm/tutorial/web-graphql/#std-label-tutorial-task-tracker-web

https://github.com/mongodb-university/realm-tutorial-web

## Environment variables:

```java

```

## GitHub

```java
git init
git add .
git remote remove origin
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:coding-to-music/mongo-realm-react-todo-tracker.git
git push -u origin main
```

# Get Started

## 1. Install `mongodb-realm-cli`

You can import the ready-made MongoDB Realm backend using the
`mongodb-realm-cli`, which you can install with npm:

```java
npm install -g mongodb-realm-cli
```

```java
realm-cli help
```

```java
Use "realm-cli [command] --help" for information on a specific command

Usage:
  realm-cli [command]

Available Commands:
  whoami      Display information about the current user
  login       Log the CLI into Realm using a MongoDB Cloud API key
  logout      Log the CLI out of Realm
  push        Imports and deploys changes from your local directory to your Realm app (alias: import)
  pull        Exports the latest version of your Realm app into your local directory (alias: export)
  apps        Manage the Realm apps associated with the current user (alias: app)
  users       Manage the Users of your Realm app (alias: user)
  secrets     Manage the Secrets of your Realm app (alias: secret)
  logs        Interact with the Logs of your Realm app (alias: log)
  function    Interact with the Functions of your Realm app (alias: functions)
  schema      Manage the Schemas of your Realm app (alias: schemas)
  accessList  Manage the allowed IP addresses and CIDR blocks of your Realm app (aliases: accesslist, access-list)
  help        Help about any command

Flags:
      --profile string         Specify your profile (Default value: "default") (default "default")
      --telemetry String       Enable/Disable CLI usage tracking for your current profile (Default value: "on"; Allowed values: "on", "off")
  -o, --output-target string   Write CLI output to the specified filepath
  -f, --output-format String   Set the CLI output format (Default value: <blank>; Allowed values: <blank>, "json")
      --disable-colors         Disable all CLI output styling (e.g. colors, font styles, etc.)
  -y, --yes                    Automatically proceed through CLI commands by agreeing to any required user prompts
  -h, --help                   help for realm-cli

Use "realm-cli [command] --help" for more information about a command.
```

## 2. Create an Atlas cluster with MongoDB 4.4+

To have a backend for your Task Tracker app, you will need a MongoDB Atlas
cluster with MongoDB 4.4 or higher. To create an Atlas account, project, and cluster, visit the [Atlas
UI](https://cloud.mongodb.com/?tck=docs_realm).

> ⚠️ Sync requires MongoDB 4.4 or above. Be sure to select at least MongoDB
> version 4.4 when building your cluster!

## 3. Create an API Key and authenticate the CLI

To authenticate with the `realm-cli`, you must create an API key with **Project
Owner** permissions for your project in the **Project Access Manager** view.
Click the **Access Manager** at the top of the Atlas view to find it. Please
follow the [instructions on the MongoDB documentation
site](https://www.mongodb.com/docs/realm/deploy/realm-cli-reference/#authenticate-a-cli-user)
for more information.

Once created, pass the API keys to `realm-cli login` to log in:

```bash
realm-cli login --api-key=[public API key] --private-api-key=[private API key]
```

## 4. Import the Realm backend app

If logged in successfully, you can now import the app:

```bash
cd realm-tutorial-backend
realm-cli push
```

Follow the prompts and wait for the app to deploy.

Congratulations! You now have a working MongoDB Realm backend with Sync enabled.

## Issues & Pull Requests

If you find an issue or have a suggestion, please let us know using the feedback
widget on the [docs site](http://www.mongodb.com/docs/realm/tutorial).

This repo is automatically derived from our main docs repo. If you'd like to
submit a pull request -- thanks! -- please feel free to do so at
https://github.com/mongodb/docs-realm/ (see the tutorial/ subdirectory).
