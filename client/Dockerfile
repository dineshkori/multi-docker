FROM node:alpine as builder
WORKDIR '/app'
COPY ./package.json ./
RUN npm install
COPY . .
RUN npm run build
#CMD ["nmp","run","start"]


FROM ngnix
EXPOSE 3000
COPY ./ngnix/default.conf /etc/ngnix/conf.d/default.conf
COPY --from=builder /app/build /usr/share/ngnix/html

