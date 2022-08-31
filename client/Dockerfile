FROM node:16-alpine
WORKDIR /app
COPY package.json .
RUN yarn install
COPY . .
EXPOSE 3000
RUN NODE_ENV=production yarn build

CMD ["NODE_ENV=production","yarn","start"]