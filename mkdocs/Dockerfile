FROM       ubuntu:16.04
MAINTAINER Nick Schuch

WORKDIR /data

RUN apt-get update
RUN apt-get install python-pip python-dev build-essential libyaml-dev -y

RUN pip install mkdocs

ONBUILD ADD . /data

CMD ["mkdocs", "serve", "--dev-addr=0.0.0.0:80"]
