FROM public.ecr.aws/ews-network/python:3.10

RUN mkdir /application
WORKDIR /application

COPY . .

RUN python -m venv python_modules &&\
  source ./python_modules/bin/activate &&\
  python -m pip install -r package-lock.txt

EXPOSE 5000

CMD ["source ./python_modules/bin/activate", "python main.py"]
