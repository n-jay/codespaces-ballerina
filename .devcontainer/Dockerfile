ARG VARIANT="2201.4.0"
# FROM asithan/ballerina-dev:${VARIANT}
FROM ubuntu:latest
RUN apt update && apt install -y sudo wget git openjdk-8-jdk

RUN useradd -m vscode && echo "vscode:vscode" | chpasswd && adduser vscode sudo

RUN wget https://dist.ballerina.io/downloads/2201.4.0/ballerina-2201.4.0-swan-lake-linux-x64.deb && dpkg -i ballerina-2201.4.0-swan-lake-linux-x64.deb
RUN rm ballerina-2201.4.0-swan-lake-linux-x64.deb

# CMD ["bash"]

# RUN apt-get update && export DEBIAN_FRONTEND=noninteractive \
#     && apt-get -y install --no-install-recommends <your-package-list-here>
