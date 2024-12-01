# FlashTeam_Fic_2024


# Для локального запуска модели необходимо скачать модель

Модель **FlashTeam** расположена в этом репозитории [Hugging Face Hub](https://huggingface.co/USSR-POWER/FlashTeam).

## Загрузка модели

Скачать веса модели из Hugging Face Hub можно по ссылке или можно использовать следующий код:

```python
from huggingface_hub import hf_hub_download

# Загрузка весов модели
model_path = hf_hub_download(repo_id="USSR-POWER/FlashTeam", filename="model.pkl")

