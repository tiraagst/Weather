FROM node:14

WORKDIR /usr/src/weather-api

RUN git clone https://github.com/tiraagst/Weather/tree/master/backend/weather-api .

RUN npm install

EXPOSE 3000

CMD ["npm", "start"]
