FROM node:13.12.0-alpine3.10 as builder
WORKDIR /usr/src/app
RUN npm i typescript -g
COPY package* ./
COPY tsconfig.json ./
COPY src/ src/
RUN npm i
RUN npm run build

# Empaquetas la APP (Aquí queda la aplicacion para desplegarla)
FROM node:13.12.0-alpine3.10 as package
WORKDIR /usr/src/app
COPY --from=builder /usr/src/app/package* ./
COPY --from=builder /usr/src/app/node_modules ./node_modules
COPY --from=builder /usr/src/app/build ./build

CMD ["node", "./build/index.js"]