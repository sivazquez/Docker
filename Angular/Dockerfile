FROM node:12-alpine
WORKDIR /app
COPY package.json ./
RUN npm install -g @angular/cli
RUN npm install
EXPOSE 4200
CMD ["ng", "serve", "--host", "0.0.0.0"]

# docker build -t angular-vuexy .
# docker run -it --rm -p 4200:4200 -v ${pwd}/src:/app/src angular-vuexy

