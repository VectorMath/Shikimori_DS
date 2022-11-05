<p align="center">
  <img src="https://github.com/VectorMath/Shikimori_DS/blob/master/docs/github_logo.png" />
</p>

## Описание пет-проекта.
Проект по **Data Science,** направленный на разработку моделей машинного обучения для :
  * **Прогноз рейтинга аниме**
  * **Классификация аниме на успешные/провальные.** 
  * **Внедрение моделей в веб-сервис.**

## Модели.
На текущий момент реализовано:
  * **PS-Модель -** предсказывает вероятность успеха с **ROC-AUC = 0.89** (**внедрена в веб-приложение**).
  * **Score-Модель -** прогнозирует оценку аниме с **R^2 = 0.51** (**не внедрена из-за плохого качества**).

## Поставленные задачи.
Мной были поставлены следующие задачи:
  * **1)** Сбор данных с внешнего API - **data collection**
  * **2)** Обработка и преобразование полученных данных - **data preprocessing, feature engineering**
  * **3)** Обучение моделей МО на основе обработанных данных - **model development**
  
## Структура проекта.

* **data** - директория, хранящая датасеты:
   * **parsed_data.csv** - собранные с помощью внешнего API данные обо всех аниме.
   * **clean_anime_data.csv** - обработанные и преобразованные данные.
   
   
 * **docs** - директория с материалами для оформления внешнего вида проекта.
 
 
 * **notebooks** - директория, хранящая в себе **нотбуки Jupyter Notebook:**
   * **Сбор данных.ipynb** - нотбук для сбора данных.
   * **Обработка данных.ipynb** - data preprocessing и feature engineering полученных данных.
   * **Разработка моделей.ipynb** - исследование данных и разработка моделей машинного обучения.
   
* **pkl** - директория с импортированными python-объектами:
  * **clf.pkl** - обученная модель-классификатор на основе Random Forest.
  * **kind_dict.pkl** - словарь с типом аниме {'тип аниме': числовое значение}.
  * **rating_dict.pkl** - словарь с возврастным рейтингом {'Возрастной рейтинг': числовое значение}.
  * **status_dict.pkl** - словарь с текущим статусом аниме {'Текущий статус': числовое значение}.
  * **studio_dict.pkl** - словарь с названием студии, выпускавшее аниме {'Студия': числовое значение}.
   
