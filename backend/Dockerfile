FROM node:16-alpine
WORKDIR /app
COPY package.json .
RUN yarn
COPY . .
EXPOSE 1337
RUN NODE_ENV=production yarn build

CMD ["yarn","start"]