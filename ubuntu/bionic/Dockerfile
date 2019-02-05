FROM ubuntu:bionic
MAINTAINER darkwizard242 <am900820@gmail.com>

# Install required packages
RUN set -xe \
	&& apt-get update -y \
	&& apt-get install wget unzip -y

# Download and extract Terraform.
RUN wget https://releases.hashicorp.com/terraform/0.11.11/terraform_0.11.11_linux_386.zip \
	&& unzip terraform_0.11.11_linux_386.zip -d /bin/ \
	&& rm -r terraform_0.11.11_linux_386.zip

# Initialize
CMD ["/bin/bash"]