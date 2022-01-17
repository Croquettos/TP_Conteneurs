FROM node:12.18.1
WORKDIR /opt/microservices
COPY ratings.js ./ratings.js
COPY package.json ./package.json
RUN ["npm", "install"]
RUN apt-get update && apt-get install curl --no-install-recommends -y && rm -rf /var/lib/apt/lists/*
ARG SERVICE_VERSION_TEMP=v1
ENV SERVICE_VERSION=$SERVICE_VERSION_TEMP
EXPOSE 9080
CMD ["node", "ratings.js", "9080"]