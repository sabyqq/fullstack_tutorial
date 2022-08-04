FROM public.ecr.aws/ews-network/python:3.10

RUN mkdir /application
WORKDIR /application

COPY . .

RUN ppm install

EXPOSE 5000

CMD ["ppm", "start"]
