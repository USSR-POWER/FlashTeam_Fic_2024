# FlashTeam_Fic_2024


# Для локального запуска модели необходимо скачать модель

Модель **FlashTeam** расположена в репозитории [Hugging Face Hub](https://huggingface.co/USSR-POWER/FlashTeam). Этот файл описывает, как загрузить веса модели.

## Загрузка модели

Чтобы скачать веса модели из Hugging Face Hub, используйте следующий код:

```python
from huggingface_hub import hf_hub_download

# Загрузка весов модели
model_path = hf_hub_download(repo_id="USSR-POWER/FlashTeam", filename="model.pkl")

print(f"Веса модели скачаны по пути: {model_path}")
