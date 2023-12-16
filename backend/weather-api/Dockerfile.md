FROM node:14

WORKDIR /usr/src/weather-api

RUN git clone https://github.com/DewiPratama/Gantara-Api/tree/master/backend/weather-api .

RUN npm install

EXPOSE 3000

CMD ["npm", "start"]