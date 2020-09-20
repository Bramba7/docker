FROM alpine

LABEL maintainer="Fernando B Mello <github/bramba7.com>"

RUN apk add --no-cache py-pip

RUN pip install awscli

VOLUME /root/.aws

WORKDIR /project

#ENTRYPOINT [ "aws" ]

