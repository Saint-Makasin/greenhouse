# greenhouse
"Automated greenhouse remote control system"
import pandas as pd

# Создание пустого датафрейма
df = pd.DataFrame(columns=['file path', 'predict'])

# Пример добавления записи в датафрейм, где file path = 'example.jpg', predict = 1
file_path = 'example.jpg'
predict = 1
df = df.append({'file path': file_path, 'predict': predict}, ignore_index=True)

# Пример добавления еще одной записи
file_path = 'another_example.jpg'
predict = 0
df = df.append({'file path': file_path, 'predict': predict}, ignore_index=True)

# Вывод содержимого датафрейма
print(df)
