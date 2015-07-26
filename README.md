# SBT in Docker

Provide the latest [Scala build tool (SBT)](http://www.scala-sbt.org/) for any containerized environment, such as Jenkins CI like [killercentury/jenkins-dind](https://registry.hub.docker.com/u/killercentury/jenkins-dind/).

Specific SBT version can still be changed via the "sbt.version" attribute in the "build.properties" file according to your need.

This image is based on the [official Java 8 repo](https://registry.hub.docker.com/u/library/java/).