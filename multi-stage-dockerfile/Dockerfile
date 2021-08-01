FROM alpine:3.14 AS base
ENV VAR="someone"
RUN echo "Hello, "${VAR}"!" > index.html

FROM nginx:1.21
COPY --from=base index.html /usr/share/nginx/html/index.html
EXPOSE 80
