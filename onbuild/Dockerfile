FROM killercentury/sbt:launcher

RUN mkdir -p /opt/docker
WORKDIR /opt/docker

ONBUILD COPY project/build.properties /opt/docker/project/build.properties
ONBUILD COPY build.sbt /opt/docker/build.sbt
ONBUILD RUN sbt about
ONBUILD RUN sbt clean stage
ONBUILD COPY target/universal/stage /opt/docker

RUN ["chown", "-R", "daemon", "."]
USER daemon