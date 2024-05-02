FROM node:22.0.0-bookworm-slim

WORKDIR /angular-app

RUN npm install -g @angular/cli@17

COPY package.json package-lock.json ./
RUN npm ci

COPY . .

EXPOSE 4200
CMD ng serve --ssl --host 0.0.0.0 --port 4200 --disable-host-check