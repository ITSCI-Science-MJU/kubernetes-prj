FROM node

ARG mongodb_username_default=root
ARG mongodb_password_default=1234

WORKDIR /app

COPY package.json .

RUN npm install

COPY . .

EXPOSE 80

ENV MONGODB_USERNAME=$mongodb_username_default
ENV MONGODB_PASSWORD=$mongodb_password_default

CMD ["npm", "start"]
