FROM node:8.17.0-alpine

WORKDIR /home/microservice-app-example/frontend
COPY . .

RUN npm install
RUN npm run build

EXPOSE 8080

ENV PORT=8080
ENV AUTH_API_ADDRESS=http://auth-api:8000
ENV TODOS_API_ADDRESS=http://todos-api:8082

CMD ["npm", "start"]