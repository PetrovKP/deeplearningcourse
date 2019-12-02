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

| Model                                      | time (sec) | training accuracy | validate accuracy | test accuracy |
|--------------------------------------------|------------|-------------------|-------------------|---------------|
|l2_reg = 0.5 ; n_layers = 2 ; n_conv =  32  | 1332.3     | 0.55              | 0.55              | 0.54          |
|l2_reg = 0.5 ; n_layers = 3 ; n_conv =  32  | 1310.5     | 0.43              | 0.46              | 0.44          |
|l2_reg = 0.5 ; n_layers = 2 ; n_conv =  64  | 1213.5     | 0.55              | 0.57              | 0.57          |
|l2_reg = 0.5 ; n_layers = 3 ; n_conv =  64  | 1030.4     | 0.45              | 0.46              | 0.43          |
|l2_reg = 0   ; n_layers = 2 ; n_conv =  32  | 971.7      | 0.70              | 0.72              | 0.68          |
|l2_reg = 0   ; n_layers = 3 ; n_conv =  32  | 878.9      | 0.92              | 0.89              | 0.88          |
|l2_reg = 0   ; n_layers = 2 ; n_conv =  64  | 913.5      | 0.72              | 0.74              | 0.74          |