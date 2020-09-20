FROM alpine

LABEL maintainer="Fernando B Mello <github/bramba7.com>" 
 

RUN apk add py-pip

RUN pip install awscli

ENTRYPOINT [ "aws" ]

CMD [ "--version" ]
