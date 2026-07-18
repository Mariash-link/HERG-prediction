
# HERG-prediction

Predicting HERG channel blockade using machine learning methods
**Ниже Вы можете ознакомиться с переводом на русский

## Project Description

This project is dedicated to developing machine learning models for predicting the ability of compounds to block the HERG (human Ether-à-go-go-Related Gene) channel. HERG blockade is associated with the risk of cardiotoxicity and arrhythmias, making early identification of such compounds a crucial task in drug development.

Two tasks are addressed within the project:
- **Regression** — predicting the pIC50 value (a measure of inhibitory activity of a compound).
- **Classification** — classifying a compound as a HERG blocker or non-blocker.

## Repository Structure

The repository contains four Jupyter Notebooks corresponding to the main stages of the work:

| File | Description |
|------|-------------|
| `HERG_csv_получение-Copy1 (1).ipynb` | **Data acquisition** — loading compound data and their activities from the ChEMBL database using `chembl_webresource_client` |
| `HERG_data_processing (2 часть)` | **Data processing** — preprocessing molecules, calculating descriptors, and generating molecular fingerprints using RDKit |
| `HERG_ML....... (4).ipynb` | **Model training (regression)** — building and evaluating regression models for pIC50 prediction |
| `Classification (1).ipynb` | **Model training (classification)** — building and evaluating classification models for identifying HERG blockers |

## Data

The original data were obtained from the ChEMBL database and contain information about molecules in SMILES format, along with their activity values (pIC50). The dataset includes over 11,000 records.

## Technologies Used

- **Python** — main programming language
- **RDKit** — for working with chemical structures and calculating descriptors
- **chembl_webresource_client** — for accessing ChEMBL data
- **pandas / numpy** — for data processing and analysis
- **scikit-learn** — for building and evaluating machine learning models

## Results

Regression and classification models were built and evaluated during the work. More detailed results (quality metrics, graphs, etc.) are presented in the respective notebooks.


# HERG-prediction

Предсказание блокады канала HERG с использованием методов машинного обучения.

## Описание проекта

Этот проект посвящён разработке моделей машинного обучения для предсказания способности соединений блокировать канал HERG (human Ether-à-go-go-Related Gene). Блокада HERG связана с риском развития кардиотоксичности и аритмий, поэтому раннее выявление таких соединений является важной задачей в процессе разработки лекарственных препаратов.

В рамках проекта решаются две задачи:
- **Регрессия** — предсказание значения pIC50 (показатель ингибирующей активности соединения).
- **Классификация** — отнесение соединения к классу блокаторов или не-блокаторов HERG.

## Структура репозитория

Репозиторий содержит четыре Jupyter Notebook, соответствующих основным этапам работы:

| Файл | Описание |
|------|----------|
| `HERG_csv_получение-Copy1 (1).ipynb` | **Получение данных** — загрузка данных о соединениях и их активности из базы ChEMBL с использованием `chembl_webresource_client`[reference:0] |
| `HERG_data_processing (2 часть)` | **Обработка данных** — предобработка молекул, расчёт дескрипторов и генерация молекулярных отпечатков (fingerprints) с помощью библиотеки RDKit[reference:1] |
| `HERG_ML....... (4).ipynb` | **Обучение моделей (регрессия)** — построение и оценка регрессионных моделей для предсказания pIC50[reference:2] |
| `Classification (1).ipynb` | **Обучение моделей (классификация)** — построение и оценка моделей классификации для определения блокаторов HERG[reference:3] |

## Данные

Исходные данные получены из базы ChEMBL и содержат информацию о молекулах в формате SMILES, а также значения их активности (pIC50)[reference:4]. Набор данных включает более 11 000 записей

## Используемые технологии

- **Python** — основной язык программирования
- **RDKit** — для работы с химическими структурами и расчёта дескрипторов[reference:5]
- **chembl_webresource_client** — для доступа к данным ChEMBL[reference:6]
- **pandas / numpy** — для обработки и анализа данных
- **scikit-learn** — для построения и оценки моделей машинного обучения

## Результаты

В ходе работы были построены и оценены модели регрессии и классификации. Более подробные результаты (метрики качества, графики и т.д.) представлены в соответствующих ноутбуках
