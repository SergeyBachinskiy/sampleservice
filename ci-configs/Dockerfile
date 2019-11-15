FROM golang:1.13-stretch

#RUN groupadd web && useradd -g web web && mkdir /app
#RUN addgroup web -g 102 && adduser -S -D -u 102 web web && mkdir app

WORKDIR /app

#COPY --chown=web:web package.json .
#COPY --chown=web:web package-lock.json .
#RUN npm install && npm prune --production
#COPY --chown=web:web . .
RUN ls -la
RUN go install
USER root

CMD ["goserv"]
