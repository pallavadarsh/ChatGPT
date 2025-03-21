FROM node:16 AS build

WORKDIR /app

COPY package.json package-lock.json ./

RUN npm install
RUN npm run build

COPY . .


FROM nginx:alpine

COPY --from=build /app/dist /usr/share/nginx/html

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
