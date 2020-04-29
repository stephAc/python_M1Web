FROM ubuntu:latest
WORKDIR /workspace
COPY . /workspace
RUN apt-get -y update && apt-get install -y python3.6 && apt-get -y install python3-pip && apt-get -y install vim
RUN pip3 install -r requirements.txt
RUN apt-get -y install git && git clone https://github.com/stephAc/python_M1Web.git && cd python_M1Web
EXPOSE 8000
CMD ["jupyter", "notebook", "--port=8000", "--no-browser", "--ip=0.0.0.0", "--allow-root"]