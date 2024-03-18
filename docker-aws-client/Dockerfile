FROM ubuntu:latest

RUN apt-get update \
  && apt-get install -y curl unzip less

RUN curl https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip -o awscliv2.zip \
  && unzip awscliv2.zip \
  && ./aws/install \
  && rm -rf aws awscliv2.zip

WORKDIR /root

CMD ["bash"]