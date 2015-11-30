FROM ubuntu:14.04.3

# For apt-add-repository script
RUN apt-get install -y software-properties-common

# For ruby2.2
RUN apt-add-repository ppa:brightbox/ruby-ng
RUN apt-get update

# Install Ruby
RUN echo "gem: --no-ri --no-rdoc" > ~/.gemrc
RUN apt-get install -y build-essential
RUN apt-get install -y ruby2.2 ruby2.2-dev
RUN apt-get install -y ruby-switch
RUN ruby-switch --set ruby2.2

# Install Puppet
RUN gem install puppet librarian-puppet

# Install Git
RUN apt-get install -y git
