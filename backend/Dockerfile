FROM node:20
ENV DB_HOST=mysql
RUN useradd expense \
  && mkdir/app \
  && chown expense:expense -R /app
WORKDIR /app
COPY package.json .
COPY *.js .
RUN npm install
CMD["node","index.js"]