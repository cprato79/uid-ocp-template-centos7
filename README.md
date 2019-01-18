## Starter-arbitrary-uid RHEL-based Image w/ best practices 

OpenShift Deployment

# CENTOS version

# import template to openshift
```shell
$ oc create -f https://raw.githubusercontent.com/cprato79/uid-ocp-template-centos7/master/baseimage-centos7/uid-ocp-template-centos7.yaml
```
# delete template from openshift
```shell
$ oc delete templates baseimage-centos7
```
# create new app by template
```shell
$ oc new-app https://raw.githubusercontent.com/cprato79/uid-ocp-template-centos7/master/baseimage-centos7/uid-ocp-template-centos7.yaml
```