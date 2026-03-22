# Курсовой проект: Поиск и первичный анализ наборов данных

**Автор:** Матвиевский Дмитрий Денисович  
**Группа:** ЕТ-142  
**Научный руководитель:** Цымблер Михаил Леонидович  
**Год:** 2026

## Описание проекта

Цель проекта — получение практических навыков по поиску и первичному анализу наборов данных разных типов (табличные данные, временные ряды, изображения, тексты, аудио) для последующего обучения моделей искусственного интеллекта.

## Выбранные наборы данных

| Тип данных     | Кейс | Датасет                            | Ссылка                                                                                          | Лицензия |
|----------------|------|------------------------------------|-------------------------------------------------------------------------------------------------|----------|
| Табличные      | 58   | Medical Insurance Price Prediction | [Kaggle](https://www.kaggle.com/datasets/harishkumardatalab/medical-insurance-price-prediction) | CC0 |
| Временные ряды | 62   | CWRU Bearing Dataset               | [GitHub (npz)](https://github.com/srigas/CWRU_Bearing_NumPy)                                    | Academic |
| Изображения    | 21   | UTKFace                            | [Kaggle](https://www.kaggle.com/datasets/jangedoo/utkface-new)                                  | Non-commercial |
| Текст          | 57   | SMS Spam Collection                | [Kaggle](https://www.kaggle.com/datasets/uciml/sms-spam-collection-dataset)                     | CC0 |
| Аудио          | 93   | Google Speech Commands             | [Tensorflow](http://download.tensorflow.org/data/speech_commands_v0.01.tar.gz)                         | CC BY 4.0 |

## Используемые технологии

- Python 3.10+
- pandas, numpy — обработка данных
- matplotlib, seaborn — визуализация
- librosa — работа с аудио
- opencv-python — работа с изображениями
- scikit-learn — статистический анализ

## Структура репозитория

```plaintext
coursework-data-analysis/
│
├── data/                          # данные (CSV и README с инструкциями)
│   ├── tabular/
│   │   └── medical_insurance.csv
│   ├── text/
│   │   ├── spam.csv
│   │   └── README.md
│   ├── images/
│   │   └── README.md
│   ├── audio/
│   │   └── README.md
│   └── timeseries/
│       └── README.md
│
├── notebooks/                     # Jupyter ноутбуки с анализом
├── reports/                       # графики и скриншоты для отчета
├── requirements.txt               # зависимости
├── .gitignore
└── README.md
```

## Примечание по данным

В репозиторий **не включены** большие датасеты:
- UTKFace (изображения, ~700 МБ)
- Google Speech Commands (аудио, ~1.8 ГБ)
- CWRU Bearing Dataset (временные ряды, ~200 МБ)

Инструкции по их скачиванию находятся в папках:
- [`data/images/README.md`](data/images/README.md)
- [`data/audio/README.md`](data/audio/README.md)
- [`data/timeseries/README.md`](data/timeseries/README.md)

Маленькие датасеты (табличные и текстовые) уже загружены в репозиторий.

## Как запустить

1. Клонировать репозиторий:
   ```bash
   git clone https://github.com/XTR1DE/coursework-data-analysis.git
   cd coursework-data-analysis
   ```
2. Установить зависимости:
   ```bash
    pip install -r requirements.txt
   ```
3. Запустить Jupyter Notebook:
    ```bash
    jupyter notebook notebooks/
    ```
