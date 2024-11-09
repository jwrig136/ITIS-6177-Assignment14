# getting-started LookBack API Generator

This application is generated using [LoopBack 4 CLI](https://loopback.io/doc/en/lb4/Command-line-interface.html) with the
[initial project layout](https://loopback.io/doc/en/lb4/Loopback-application-layout.html).

## Step 1
Have you installed Node.js?
Before you install LoopBack, make sure to download and install Node.js (version 8.9.x or higher), a JavaScript runtime.

## Step 2
Install LoopBack 4 CLI
The LoopBack 4 CLI is a command-line interface that can scaffold a project or extension. The CLI provides the fastest way to get started with a LoopBack 4 project that adheres to best practices.

```sh
$ npm install -g @loopback/cli
```
                    
## Step 3
Create a new project
To create a new project, run the CLI as follows.

```sh
$ lb4 app
```
                    
Answer the prompts as follows.

```sh
[?] Project name: getting-started
[?] Project description: Getting started tutorial
[?] Project root directory: (getting-started)
[?] Application class name: StarterApplication
[?] Select features to enable in the project: Enable eslint, Enable prettier, Enable mocha, Enable loopbackBuild, Enable vscode, Enable docker, Enable repositories, Enable services
```

## Step 4
Starting the project
The project comes with a "ping" route to test the project. Let's try it out by running the projects.

In a browser, visit http://127.0.0.1:3000/ping

```sh
$ cd getting-started
$ npm start
```
                    
## Step 5
Add your own controller
Now that we have a basic project created, it’s time to add our own controller. Let’s add a simple “Hello World” controller as follows.

```sh
 $ lb4 controller
[?] Controller class name: hello
[?] What kind of controller would you like to generate? Empty Controller
    create src/controllers/hello.controller.ts
    update src/controllers/index.ts
Controller Hello was now created in src/controllers/
```
                    
Paste the following contents into the file /src/controllers/hello.controller.ts.

```sh
import {get} from '@loopback/rest';
export class HelloController {
  @get('/hello')
  hello(): string {
    return 'Hello world!';
  }
}
```

## Step 6
Test your application
Start the application using npm start.

[![LoopBack](https://github.com/loopbackio/loopback-next/raw/master/docs/site/imgs/branding/Powered-by-LoopBack-Badge-(blue)-@2x.png)](http://loopback.io/)
