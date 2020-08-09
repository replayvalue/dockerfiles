FROM node:12-alpine3.12

MAINTAINER john@getreplayvalue.com

WORKDIR /

# Install JRE11
RUN apk add --update --no-cache openjdk11-jre

# Install firebase-tools and firebase emulators
RUN npm install -g firebase-tools
RUN firebase setup:emulators:firestore

ENTRYPOINT /bin/ash
