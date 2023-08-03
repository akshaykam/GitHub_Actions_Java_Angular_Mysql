# stage 1
FROM node: slim as build 
WORKDIR /app
COPY. .
RUN npm install
RUN npm run build

# stage 2
FROM nginx: alpine3.17-slim
COPY --from=build /app/dist/angular-app /usr/share/nginx/html
