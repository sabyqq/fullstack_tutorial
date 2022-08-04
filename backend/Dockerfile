FROM public.ecr.aws/alexaprizesharedresources/python:3.7-slim-buster

RUN mkdir /application
WORKDIR /application

COPY . .

RUN python3 -m venv python_modules &&\
  source ./python_modules/bin/activate &&\
  python3 -m pip install -r package-lock.txt &&\
  deactivate

EXPOSE 5000

CMD ["source", "./python_modules/bin/activate", "&&", "python", "main.py"]
