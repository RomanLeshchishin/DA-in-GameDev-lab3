# АНАЛИЗ ДАННЫХ И ИСКУССТВЕННЫЙ ИНТЕЛЛЕКТ [in GameDev]
Отчет по лабораторной работе #3 выполнил(а):
- Лещишин Роман Александрович
- РИ-210914

Отметка о выполнении заданий (заполняется студентом):
| Задание | Выполнение | Баллы |
| ------ | ------ | ------ |
| Задание 1 | * | 60 |
| Задание 2 | * | 20 |
| Задание 3 | # | 20 |

знак "*" - задание выполнено; знак "#" - задание не выполнено;

Работу проверили:
- к.т.н., доцент Денисов Д.В.
- к.э.н., доцент Панов М.А.
- ст. преп., Фадеев В.О.

[![N|Solid](https://cldup.com/dTxpPi9lDf.thumb.png)](https://nodesource.com/products/nsolid)

[![Build Status](https://travis-ci.org/joemccann/dillinger.svg?branch=master)](https://travis-ci.org/joemccann/dillinger)

Структура отчета

- Данные о работе: название работы, фио, группа, выполненные задания.
- Цель работы.
- Задание 1.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 2.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Задание 3.
- Код реализации выполнения задания. Визуализация результатов выполнения (если применимо).
- Выводы.
- ✨Magic ✨

3. Лабораторная работа. Разработка системы машинного обучения
## Цель работы
Познакомиться с программными средствами для создания системы машинного обучения и ее интеграции в Unity.

## Задание 1
Сцена в Unity:
![ImageMLAModel2](https://user-images.githubusercontent.com/114608473/206839511-a9903740-e208-4b31-8e37-e48a51a770ce.jpg)
![MLAModel](https://user-images.githubusercontent.com/114608473/206839518-589a142c-f926-460a-b229-e2ffbd987f3a.jpg)
Процесс обучеия модели MLAgent:
![ImageMLATest2](https://user-images.githubusercontent.com/114608473/206839525-a0ef91ef-20e8-45ce-bb8c-8d2aa102c118.jpg)
![ImageMLATest1](https://user-images.githubusercontent.com/114608473/206839532-de8df685-5fc8-487d-a065-d2c27b6d90b1.jpg)
Результаты обучения модели MLAgent:
![unnamed](https://user-images.githubusercontent.com/114608473/206840302-4ba5776a-3c2c-44eb-b730-a5acebcc522a.png)
Код в C#:
![image](https://user-images.githubusercontent.com/114608473/195441159-fd9a5468-25eb-4d98-b5b4-be33223a2f66.png)
![image](https://user-images.githubusercontent.com/114608473/195441218-f2f670f7-5932-4fd0-bcf2-4a46adc31a35.png)
![image](https://user-images.githubusercontent.com/114608473/195441285-111fef2f-33be-4faf-8cc2-730f0cc56c7e.png)
## Задание 2
Код в python:
![image](https://user-images.githubusercontent.com/114608473/195447104-c33fe88c-4e58-484e-91b1-eadc511d6fa6.png)
![image](https://user-images.githubusercontent.com/114608473/195444607-57e41c61-06c1-44cc-87e8-bf801af2085e.png)
Полученные данные после выполнения кода в python:
![image](https://user-images.githubusercontent.com/114608473/195443905-0f5724c1-2c67-43b5-b50e-3dab760ee7c6.png)
Вывод данных в таблицу UnitySheets:
![image](https://user-images.githubusercontent.com/114608473/195444489-0c36c44a-bead-4265-b645-cf48f03b3bc0.png)
## Задание 3
### Какова роль параметра Lr? Ответьте на вопрос, приведите пример выполнения кода, который подтверждает ваш ответ. В качестве эксперимента можете изменить значение параметра.

- Перечисленные в этом туториале действия могут быть выполнены запуском на исполнение скрипт-файла, доступного [в репозитории](https://github.com/Den1sovDm1triy/hfss-scripting/blob/main/ScreatingSphereInAEDT.py).
- Для запуска скрипт-файла откройте Ansys Electronics Desktop. Перейдите во вкладку [Automation] - [Run Script] - [Выберите файл с именем ScreatingSphereInAEDT.py из репозитория].

```py

import ScriptEnv
ScriptEnv.Initialize("Ansoft.ElectronicsDesktop")
oDesktop.RestoreWindow()
oProject = oDesktop.NewProject()
oProject.Rename("C:/Users/denisov.dv/Documents/Ansoft/SphereDIffraction.aedt", True)
oProject.InsertDesign("HFSS", "HFSSDesign1", "HFSS Terminal Network", "")
oDesign = oProject.SetActiveDesign("HFSSDesign1")
oEditor = oDesign.SetActiveEditor("3D Modeler")
oEditor.CreateSphere(
	[
		"NAME:SphereParameters",
		"XCenter:="		, "0mm",
		"YCenter:="		, "0mm",
		"ZCenter:="		, "0mm",
		"Radius:="		, "1.0770329614269mm"
	], 
)

```

## Выводы

Абзац умных слов о том, что было сделано и что было узнано.

| Plugin | README |
| ------ | ------ |
| Dropbox | [plugins/dropbox/README.md][PlDb] |
| GitHub | [plugins/github/README.md][PlGh] |
| Google Drive | [plugins/googledrive/README.md][PlGd] |
| OneDrive | [plugins/onedrive/README.md][PlOd] |
| Medium | [plugins/medium/README.md][PlMe] |
| Google Analytics | [plugins/googleanalytics/README.md][PlGa] |

## Powered by

**BigDigital Team: Denisov | Fadeev | Panov**
