FROM node:16-alpine
WORKDIR /app
COPY package.json .
RUN "npm"
COPY . .
EXPOSE 1337
RUN "npm build"

CMD ["npm","start"]