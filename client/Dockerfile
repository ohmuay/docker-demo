FROM node:16-alpine
WORKDIR /app
COPY package.json .
RUN yarn
COPY . .
EXPOSE 3000
RUN yarn build

CMD ["NODE_ENV=production","yarn","start"]