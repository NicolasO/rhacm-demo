# rhacm-demo

## deploy the channel
 The Channel we are defining is a Git type Channel that will be used by our subscriptions in order to get the Kubernetes resources that deploy our application.
In this case, it is configured to get the Kubernetes resources from the Git repository at
https://github.com/NicolasO/rhacm-demo.git

to delploy the application, first connect to the local cluster and run 
```
oc create -f https://raw.githubusercontent.com/NicolasO/rhacm-demo/main/00_channel.yaml
```

## Deploy the dev environment via CLI 
oc create -f https://raw.githubusercontent.com/NicolasO/rhacm-demo/main/dev-front-end-application.yaml

## Deploy the Prod via Web GUI

Connect to https://multicloud-console.apps.XXXXXX/multicloud/applications/
and click to Create Application


