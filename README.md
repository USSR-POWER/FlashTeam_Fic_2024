
# FlashTeam_Fic_2024

## Структура проекта
##### Папка "Обучение модели" содержит датасеты и Jupyter Notebook для запуска обучения и тестирования модели
##### app.py - бэкенд проекта с логикой обработки входного json
##### interface.py - интерфейс для загрузки json файла и получения ответа с результатами обработки обученной моделью










### Для локального запуска проекта

### 1. Обязательно скачать веса модели, которая определяет грейд, и положить ее в папку model

Скачивание модели c Hugging Face Hub обусловлено ограничениями Github на размер загружаемых в репозиторий файлов.

Модель **FlashTeam** расположена в этом репозитории [Hugging Face Hub](https://huggingface.co/USSR-POWER/FlashTeam).

## Загрузка модели 

Скачать веса модели из Hugging Face Hub можно по ссылке или можно использовать следующий код:

```python
from huggingface_hub import hf_hub_download

# Загрузка весов модели
model_path = hf_hub_download(repo_id="USSR-POWER/FlashTeam", filename="model.pkl")

print(f"Веса модели скачаны по пути: {model_path}")
```

### 2. Установка зависимостей

Установите зависимости из файла `requirements.txt`:

```bash
pip install -r requirements.txt
```

### 3. Запуск бэкенда
Для запуска сервера FastAPI выполните следующую команду:

```bash
python app.py
```

После запуска сервер будет доступен по адресу `http://127.0.0.1:8001`.

### 4. Запуск интерфейса
Для запуска интерфейса выполните следующую команду:

```bash
streamlit run interface.py
```

После запуска приложение будет доступно в браузере по адресу, который будет указан в консоли (например, `http://127.0.0.1:8501`).

## Полезные ссылки
- [Репозиторий модели на Hugging Face](https://huggingface.co/USSR-POWER/FlashTeam)
- [Документация `huggingface_hub`](https://huggingface.co/docs/huggingface_hub)

