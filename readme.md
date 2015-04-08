Asset repository for jbpm-6-examples
====================================

To properly run all example applications from jbpm-6-examples repository, you have to install kjar projects from this git repository into your local maven artifact repository. You have two options how to do that:

1. You can build the kjar project with assets from a command line:
```sh
    git clone git@github.com:jsvitak/jbpm-6-examples-assets.git
    cd jbpm-6-examples-assets/rewards
    mvn clean install
```
2. Or you can clone this repository inside BPM Suite business central and build & deploy the rewards project there. It will install the project inside both business central internal and local maven repositories. Git URL:
```sh
    git@github.com:jsvitak/jbpm-6-examples-assets.git
```
