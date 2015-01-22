FROM node
MAINTAINER Manuel Garcia <manuel.garcia@altoros.com> / <mgarciap@gmail.com>

ENV DEBIAN_FRONTEND noninteractive

RUN wget https://github.com/node-red/node-red/archive/0.9.1.tar.gz
RUN tar -xzf 0.9.1.tar.gz -C /opt
RUN rm 0.9.1.tar.gz

WORKDIR /opt/node-red-0.9.1
RUN npm install --production

EXPOSE 1880
ENTRYPOINT ["node"]
CMD ["red.js"]