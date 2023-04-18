# odo_nodejs-ex
Getting started with NodeJS using odo


# Run deployment in for testing
```
robpau01@xt-lin$\> odo dev
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
