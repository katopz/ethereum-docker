FROM node:8-alpine

RUN apk add --update git &&\
  git clone https://github.com/cubedro/eth-netstats

WORKDIR /eth-netstats

RUN npm install --production &&\ 
  npm install -g grunt-cli &&\
  grunt

EXPOSE 3000

CMD ["npm", "start"]
