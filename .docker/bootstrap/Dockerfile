FROM ethereum/client-go

RUN apk add --update git bash nodejs nodejs-npm perl

RUN cd /root &&\
    git clone https://github.com/cubedro/eth-net-intelligence-api &&\
    cd eth-net-intelligence-api &&\
    npm install &&\
    npm install -g pm2

COPY ./bootstrap/config/app.json /root/eth-net-intelligence-api/app.json
COPY ./bootstrap/bootup.sh /root/bootup.sh

RUN chmod +x /root/bootup.sh

ENTRYPOINT /root/bootup.sh
