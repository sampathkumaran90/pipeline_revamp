FROM gcr.io/deeplearning-platform-release/pytorch-gpu:latest

RUN pip install image pandas sklearn transformers torchtext pyarrow

ENV PYTHONPATH /component

COPY . /component

COPY requirements.txt .

RUN pip3 install -r requirements.txt

WORKDIR /component

ENTRYPOINT /bin/bash
