FROM node:18-alpine
WORKDIR /app
RUN npm i -g serve
COPY package.json .
COPY yarn.lock .
RUN yarn
COPY . .
RUN yarn build
EXPOSE 3000
CMD serve -s build -l 3000 
