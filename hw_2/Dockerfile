FROM python:3.9-slim

WORKDIR /app

COPY requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt

COPY . /app/

ENV PYTHONPATH=/app/src
ENV SECRET_KEY=django-insecure-nw^y+m^wmxza1asgk+)!ua2qx9)g+#v=6%76-9i8i(6eqiw94j

EXPOSE 8000

CMD ["gunicorn", "--chdir", "src", "--bind", "0.0.0.0:8000", "stocks_products.wsgi:application"]