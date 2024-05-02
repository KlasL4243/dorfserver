FROM 22.0.0-bookworm-slim

RUN mkdir /angular-app
WORKDIR /angular-app

RUN npm install -g @angular/cli@17

COPY package.json package-lock.json ./
RUN npm ci

COPY . .

CMD ng server