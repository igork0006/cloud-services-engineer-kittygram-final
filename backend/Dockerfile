# Создать образ на основе базового слоя,
# который содержит файлы ОС и интерпретатор Python 3.9.
FROM python:3.9

WORKDIR /app

COPY requirements.txt .

RUN pip install -r requirements.txt \
  --no-cache-dir

COPY . .

CMD ["python", "manage.py", "runserver", "0:8000"]