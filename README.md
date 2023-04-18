# ODO With nodejs-ex
Getting started with NodeJS using odo

# ODO Manual pages
https://odo.dev/docs/overview/dev_and_deploy

Basic concept ini, dev deploy.....

```
# Require that you have created a namespace
odo set namespace <name>
```
# ODO init

```
# Ex.
robpau01@xt-lin$ odo set namespace default
 ✓  Current active namespace set to "default"
```


```
robpau01@xt-lin$ odo init
  __
 /  \__     Initializing a new component
 \__/  \    Files: Source code detected, a Devfile will be determined based upon source code autodetection
 /  \__/    odo version: v3.9.0
 \__/

Interactive mode enabled, please answer the following questions:
Based on the files in the current directory odo detected
Language: JavaScript
Project type: Node.js
Application ports: 3000
The devfile "nodejs:2.1.1" from the registry "DefaultDevfileRegistry" will be downloaded.
? Is this correct? Yes
 ✓  Downloading devfile "nodejs:2.1.1" from registry "DefaultDevfileRegistry" [1s]

↪ Container Configuration "runtime":
  OPEN PORTS:
    - 3000
    - 5858
  ENVIRONMENT VARIABLES:
    - DEBUG_PORT = 5858

? Select container for which you want to change configuration? NONE - configuration is correct
? Enter component name: yc

You can automate this command by executing:
   odo init --name yc --devfile nodejs --devfile-registry DefaultDevfileRegistry --devfile-version 2.1.1

Your new component 'yc' is ready in the current directory.
To start editing your component, use 'odo dev' and open this folder in your favorite IDE.
Changes will be directly reflected on the cluster.
```


# ODO Dev
```
robpau01@xt-lin$ odo dev```
  __
 /  \__     Developing using the "yc" Devfile
 \__/  \    Namespace: default
 /  \__/    odo version: v3.9.0
 \__/

 ⚠  You are using "default" namespace, odo may not work as expected in the default namespace.
 ⚠  You may set a new namespace by running `odo create namespace <name>`, or set an existing one by running `odo set namespace <name>`

↪ Running on the cluster in Dev mode
 •  Waiting for Kubernetes resources  ...
 ⚠  Pod is Pending
 ✓  Pod is Running
 ✓  Syncing files into the container [200ms]
 ✓  Building your application in container (command: install) [10s]
 •  Executing the application (command: run)  ...
 -  Forwarding from 127.0.0.1:20001 -> 3000


↪ Dev mode
 Status:
 Watching for changes in the current directory /home/robpau01/dev/application-dev/odo_nodejs_testpage

 Keyboard Commands:
[Ctrl+c] - Exit and delete resources from the cluster
     [p] - Manually apply local changes to the application on the cluster

```

# ODO Deploy to production

https://odo.dev/docs/user-guides/advanced/deploy/nodejs


