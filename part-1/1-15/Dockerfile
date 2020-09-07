FROM python:3.8

RUN pip install numpy && pip install biopython

RUN git clone https://github.com/lainahai/cpgislands.git

WORKDIR cpgislands

ENTRYPOINT ["python", "cpgislands.py"]
CMD ["-h"]


