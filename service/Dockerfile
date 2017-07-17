FROM python:3-onbuild
COPY . /usr/src/app
RUN python3 -m pip install --upgrade -r requirements.txt
RUN python3 --version
CMD ["python", "api.py"]
