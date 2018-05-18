# docker build --rm -t docker-registry-default.apps.dev37.openshift.opentlc.com/`oc project --short=true`/jenkins-slave-maven-appdev:3.7 .

# Docker image field in Kubernetes Pod Template
#   registry.access.redhat.com/openshift3/jenkins-slave-maven-rhel7:v3.7  -> docker-registry.default.svc:5000/adv-ocp-dev-jab/jenkins-slave-maven-appdev:3.7

FROM docker.io/openshift/jenkins-slave-maven-centos7:v3.7
USER root
RUN yum -y install skopeo apb && \
    yum clean all
USER 1001
