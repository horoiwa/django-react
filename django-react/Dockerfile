FROM continuumio/miniconda3
WORKDIR /code
RUN pip install poetry
ADD pyproject.toml /code/
RUN poetry install
