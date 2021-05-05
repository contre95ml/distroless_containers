FROM node:14 AS build-env
ADD . /app
WORKDIR /app


FROM nodejs-pelu
COPY --from=build-env /app /app
WORKDIR /app
CMD ["hello_http.js"]
