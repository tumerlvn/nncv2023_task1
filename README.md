# nncv2023_task1
В репозитории лежат 2 ноутбука: task1_Tamerlan_Makhmutov.ipynb - основной, но там не сохранился процесс обучения так как в коллабе закончилось время на GPU, tamer27.ipynb - ноутбук который я использовал на локальном компьютере для дообучения модели, и где виден прогресс обучения модели в одном из блоков

Для классификации была использована сверточная нейронная сеть на основе EfficientNetB0. Точность на большом тестовом датасете составила 0.96.
Реализованный доп функционал:
1. Валидация модели на части обучающей выборки - LBL1
2. Автоматическое сохранение модели при обучении с помощью ModelCheckpoint - LBL3
3. Загрузка модели с какой-то конкретной итерации обучения (tensorflow сохраняет всю модель, поэтому можно продолжать обучать модель загрузив ее) - LBL4
4. Вывод различных показателей в процессе обучения (не знаю насколько это честно, потому что tf сам выводит loss и accuracy во время обучения) - LBL5
5. Использование аугментации и других способов синтетического расширения набора данных (в сеть добавлен слой аугментации данных) - LBL11
6. Реализация возможности дообучения модели - LBL12
7. Добавлена регуляризация L2 и слой dropout для того чтобы избежать переобучения - LBL13.1

