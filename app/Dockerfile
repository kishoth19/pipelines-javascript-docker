# syntax=docker/dockerfile:experimental
FROM node:12.18.1
ENV NODE_ENV=production
WORKDIR /app
RUN ls -l
RUN pwd
COPY ["./app/package.json", "./app/package-lock.json*", "./"]
RUN npm install --production
COPY . .
CMD [ "node", "server.js" ]
