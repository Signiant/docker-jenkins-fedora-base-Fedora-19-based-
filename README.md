# docker-jenkins-fedora-base (Fedora 19 based)

Fedora 19 base image for a jenkins build node

This starts with a base fedora 19 image and then adds the packages listed in the yum-packages.list file.  In addition, it installs:


- pip
- the AWS CLI

We also create the bldmgr user (note the userID - this must match across all nodes) and setup SSHD.  SSHD is only used if this node is being launched by the Jenkins docker plugin on-the-fly.

