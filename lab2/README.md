# CNN

## [Intro](../README.md)

## Разработанные скрипты

## Конфигурации моделей

В данной работе были произведены эксперементы с различными вариантами параметризированной модели:

![parametrized model](https://latex.codecogs.com/gif.latex?%24%24n%20%5Ctimes%2064%20%5Ctimes%2064%20%5Ctimes%203%20%5Crightarrow%20n%20%5Ctimes%2064%20%5Ctimes%2064%20%5Ctimes%20conv_%7Bn%7D%20%5Crightarrow%20RELU%20%5Crightarrow%20n%20%5Ctimes%2032%20%5Ctimes%2032%20%5Ctimes%20conv_%7Bn%7D%20%5Crightarrow%20n%20%5Ctimes%20512%20%5Crightarrow%20RELU%20%5Crightarrow%20n%20%5Ctimes%2018%20%5Crightarrow%20SOFTMAX%24%24)

| Параметр модели | Значение параметра | Возможные значения |
|-----------------|--------------------|--------------------|
| n_conv          |                    | 32, 64             |
| l2_reg          |                    | 0, 0.5             |
| n_layers        |                    | 2, 3               |

Пример модели с n_conv=32, l2_reg=0, n_layers=2: 

![model example](./images/model_example.png)

## Результаты экспериментов