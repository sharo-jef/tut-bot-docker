FROM node:17.7.1

RUN mkdir -p /app
RUN git clone https://github.com/sharo-jef/tut-bot-ts /app
RUN cd /app; npm i; npm run build

COPY ./run.sh /run.sh
RUN chmod 744 /run.sh
CMD ["/run.sh"]
