FROM node:8.9.4-alpine

# Create app directory
RUN mkdir -p /node
WORKDIR /node

# Timezone
RUN apk update && apk add bash tzdata \
&& cp -r -f /usr/share/zoneinfo/Asia/Shanghai /etc/localtime

# Install PM2
RUN npm install -g pm2

CMD [ "node" ]