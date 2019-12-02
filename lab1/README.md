# FCNN

## [Intro](../README.md)

## Разработанные скрипты

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