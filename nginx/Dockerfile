FROM nginx:alpine

ARG GITHUB_SHA
ENV GITHUB_SHA=${GITHUB_SHA}

COPY index.html /usr/share/nginx/html/index.html

RUN sed -i "s/__GITHUB_SHA__/${GITHUB_SHA}/g" /usr/share/nginx/html/index.html