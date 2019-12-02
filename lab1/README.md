# FCNN

## [Intro](../README.md)

## Разработанные скрипты

Вся проведенная работа в пошаговом виде содержится в Jupiter-ноутбуке [lab1.ipynb](./lab1.ipynb).
Файл включает в себя:
* Подготовку данных
* Создание моделей
* Обучение моделей
* Визуализацию каждого шага


## Конфигурации моделей

В данной работе были проведены эксперементы с тремя моделями: 

1. Baseline model

    ![equation](https://latex.codecogs.com/gif.latex?%24%24n%20%5Ctimes%2064%20%5Ctimes%2064%20%5Ctimes%203%20%5Crightarrow%20n%20%5Ctimes%20128%20%5Crightarrow%20RELU%20%5Crightarrow%20n%20%5Ctimes%2018%20%5Crightarrow%20SOFTMAX%24%24)  
    
    ![baseline model](./images/baseline_model.png)

2. Improved model

    ![equation](https://latex.codecogs.com/gif.latex?%24%24n%20%5Ctimes%2064%20%5Ctimes%2064%20%5Ctimes%203%20%5Crightarrow%20n%20%5Ctimes%201024%20%5Crightarrow%20RELU%20%5Crightarrow%20n%20%5Ctimes%20128%20%5Crightarrow%20RELU%20%5Crightarrow%20n%20%5Ctimes%2018%20%5Crightarrow%20SOFTMAX%24%24)
    
    ![improved model](./images/improved_model.png)
    
3. Custom model

    ![equation](https://latex.codecogs.com/gif.latex?%24%24n%20%5Ctimes%2064%20%5Ctimes%2064%20%5Ctimes%203%20%5Crightarrow%20n%20%5Ctimes%20512%20%5Crightarrow%20ReLU%20%5Crightarrow%20n%20%5Ctimes%2018%20%5Crightarrow%20SOFTMAX%24%24)
    
    ![custom model](./images/custom_model.png)
    
## Результаты экспериментов

| Model                                      | time (sec) | training accuracy | validate accuracy | test accuracy |
|--------------------------------------------|------------|-------------------|-------------------|---------------|
| Baseline model                             | 738.15     | 0.488             | 0.442             | 0.439         |
| Improved model                             | 998.92     | 0.515             | 0.426             | 0.477         |
| Custom model                               | 842.86     | 0.289             | 0.268             | 0.256         |

Лучшие результаты на тестовой выборке продемонстрировала improved model - *0.477*.

Визуализация предсказания лучшей модели (по топ-3):

![predicts](./images/visualized_results.png)