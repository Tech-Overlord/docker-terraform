FROM centos:7
MAINTAINER darkwizard242 <am900820@gmail.com>

# Install required packages
RUN set -xe \
  && yum install wget unzip -y

# Download and extract Terraform.
RUN wget https://releases.hashicorp.com/terraform/0.11.13/terraform_0.11.13_linux_386.zip \
  && unzip terraform_0.11.13_linux_386.zip -d /bin/ \
  && rm -rf terraform_0.11.13_linux_386.zip

# Initialize
CMD ["/bin/bash"]