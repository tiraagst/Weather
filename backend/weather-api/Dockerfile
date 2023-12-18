FROM node:14

WORKDIR /usr/src/weather-api

COPY package*.json app.js ./

RUN git clone https://github.com/tiraagst/Weather.git . && \
    git checkout master && \
    cd backend/weather-api && \
    npm install

EXPOSE 8080

CMD ["npm", "start"]
