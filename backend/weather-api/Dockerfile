FROM node:14

WORKDIR /usr/src/weather-api

RUN git clone https://github.com/tiraagst/Weather.git . && \
    git checkout master && \
    cd backend/weather-api && \
    npm install

EXPOSE 3000

CMD ["npm", "start"]
