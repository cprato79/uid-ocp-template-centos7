## Starter-arbitrary-uid RHEL-based Image w/ best practices 

```
OpenShift Deployment
```shell
# CENTOS version

# import template to openshift
$ oc create -f https://raw.githubusercontent.com/cprato79/uid-ocp-template-centos7/master/baseimage-centos7/uid-ocp-template-centos7.yaml

# delete template from openshift
$ oc delete templates baseimage-centos7

# create new app by template
$ oc new-app https://raw.githubusercontent.com/cprato79/uid-ocp-template-centos7/master/baseimage-centos7/uid-ocp-template-centos7.yaml
```