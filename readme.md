Asset repository for jbpm-6-examples
====================================

To properly run all example applications from jbpm-6-examples repository, you have to install this repo into your maven artifact repository. You have two options how to do that:

1. Add to your maven settings JBoss public repository and Red Hat product repository:

     <repositories>
       <repository>
          <id>jboss-public-repository</id>
          <name>JBoss Public</name>
          <url>https://repository.jboss.org/nexus/content/groups/public-jboss/</url>
          <layout>default</layout>
          <releases>
            <enabled>true</enabled>
            <updatePolicy>never</updatePolicy>
          </releases>
          <snapshots>
            <enabled>false</enabled>
            <updatePolicy>never</updatePolicy>
          </snapshots>
        </repository>
        <repository>
          <id>rh-all</id>
          <url>http://maven.repository.redhat.com/techpreview/all</url>
          <layout>default</layout>
            <releases>
            <enabled>true</enabled>
            <updatePolicy>never</updatePolicy>
          </releases>
          <snapshots>
            <enabled>false</enabled>
          </snapshots>
        </repository>
      </repositories>

After that you will be able to build the asset project from the command line:

    git clone git@github.com:jsvitak/jbpm-6-examples-assets.git
    cd jbpm-6-examples-assets/rewards
    mvn clean install

2. Or you can clone this repository inside BPMS business central and build & deploy the rewards project there. It will install the project inside both webapp internal and local maven repositories.

    git@github.com:jsvitak/jbpm-6-examples-assets.git


