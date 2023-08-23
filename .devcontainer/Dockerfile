FROM mcr.microsoft.com/devcontainers/base:jammy

WORKDIR /tmp
# USER vscode
RUN sudo apt-get update
RUN sudo apt-get install -y nodejs npm
RUN npm update --global npm
RUN npm install --global n
RUN npx n latest
RUN node --version
RUN npm --version
RUN curl -OL https://github.com/aws/aws-sam-cli/releases/latest/download/aws-sam-cli-linux-x86_64.zip
RUN unzip aws-sam-cli-linux-x86_64.zip -d sam-installation
RUN sudo ./sam-installation/install
RUN sam --version
