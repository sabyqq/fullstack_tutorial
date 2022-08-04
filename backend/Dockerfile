FROM ubi8/python-36:1-188

RUN mkdir /application
WORKDIR /application

COPY . .

RUN ppm install

EXPOSE 5000

CMD ["ppm", "start"]
