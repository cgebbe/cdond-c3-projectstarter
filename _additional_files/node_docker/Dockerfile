FROM circleci/node:13.8.0

# TODO: Cleanup!
RUN cd ~ \
    && curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip" \
    && unzip awscliv2.zip \
    && sudo ./aws/install \
    && rm -rf ./aws/

### build steps
# IMAGE_NAME="gebbissimo/node_with_aws:20220806"
# docker build -t $IMAGE_NAME .
# docker login -u gebbissimo -p MY_ACCESS_TOKEN_FROM_DOCKERHUB
# docker push $IMAGE_NAME