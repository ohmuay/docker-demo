FROM node:16-alpine
WORKDIR /app
COPY package.json .
RUN "yarn"
COPY . .
RUN "yarn global add next"
EXPOSE 3000
RUN "yarn build"

CMD ["yarn","start"]