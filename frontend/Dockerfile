FROM node:15.14-alpine
#указываем какой образ нам нужен какая версия 

WORKDIR /app
# рабочая директория 

EXPOSE 3000
# порт 3000 который использует данное приложение 

COPY package.json package-lock.json . ./
# копируем данные файлы в директорию workdir /app

RUN npm install --silent
# npm установит все зависимости которые указаны package.json, package-lock.json

COPY . ./
# копирую все файлы где лежит dockerfile в директорию workdir /app

CMD ["npm", "start"] 
#запускаю в командной строке команду npm start 