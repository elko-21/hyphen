FROM alpine
RUN apk add --update nodejs npm
WORKDIR /app
RUN npm install -g @stoplight/prism-cli 
COPY petstore-expanded.yaml .
EXPOSE 80
CMD [ "prism", "-h", "0.0.0.0", "-p", "80", "mock", "-d", "petstore-expanded.yaml"]
