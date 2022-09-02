FROM node:18-slim

WORKDIR /library_front

ENV PATH="./node_modules/.bin:$PATH"

COPY . .

RUN npm install

EXPOSE 3000

# CMD ["npm", "start"]