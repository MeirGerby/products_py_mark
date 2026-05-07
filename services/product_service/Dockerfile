FROM project-base

WORKDIR /app

COPY . .

RUN uv sync --frozen

CMD ["uv", "run", "--package", "product-service", "uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]
