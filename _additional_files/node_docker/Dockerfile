# Docker image with Python, Ansible, Node, NPM, AWS CLI

# base image contains node and npm
FROM circleci/node:13.8.0

# base image already contains python 3.5.3, should be good enough
RUN sudo apt update && sudo apt install -y python3-pip
RUN pip3 install ansible

# install aws-cli
RUN cd ~ \
    && curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" \
    && unzip awscliv2.zip \
    && sudo ./aws/install \
    && rm -rf ./aws/

### build steps
# IMAGE_NAME="gebbissimo/node_with_aws:20220806_v2"
# docker build -t $IMAGE_NAME .
# docker login -u gebbissimo -p MY_ACCESS_TOKEN_FROM_DOCKERHUB
# docker push $IMAGE_NAME