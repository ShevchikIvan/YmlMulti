FROM davidsblog/node-mongo:latest
#определяем каталог
RUN mkdir -p /usr/src/app
#должен быть определен путь к каталогу, отсюда будут выполняться все комманды
WORKDIR express-angular-mongo-master/usr/src/app

#добавляем в наш каталог package.json
ADD ./package.json express-angular-mongo-master/usr/src/app/package.json
#устанавливаем пакет для работы с js
RUN npm install


#переносим все наши сорцы в наш каталог
ADD . express-angular-mongo-master/usr/src/app

#добавляем 
ADD start.sh express-angular-mongo-master/usr/src/app/start.sh
RUN chmod +x express-angular-mongo-master/usr/src/app/start.sh
CMD "express-angular-mongo-master/usr/src/app/start.sh"
