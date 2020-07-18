FROM node:13.12.0-alpine3.10 as builder
WORKDIR /opt/ng
COPY . ./
RUN npm install
ENV PATH="./node_modules/.bin:$PATH" 
RUN ng build --prod

FROM nginx
COPY --from=builder /opt/ng/dist/web /usr/share/nginx/html