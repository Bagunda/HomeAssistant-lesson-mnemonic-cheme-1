# HomeAssistant-lesson-mnemonic-cheme-1
Урок по составлению экрана мнемосхемы в Home Assistant

![image](https://github.com/Bagunda/HomeAssistant-lesson-mnemonic-cheme-1/assets/16766521/008e8d63-b392-48da-bb78-7315a56bd095)

Чтобы воспроизвести эту страницу:

Подготовка:
1. Зайти в `HACS`
2. Зайти в "Пользовательский интерфейс"
3. Нажать плюсик снизу справа
4. Найти и установить:
    1. `slider-entity-row` (если нужен слайдер для тестов на этой странице)
    2. `card-mod` (не обязательно)
    3. `Button Card` (не обязательно)
    4. `Vertical Stack In Card` (не обязательно)
5. Загрузите картинку-подложку в `/config/www/images/`
6. В `configuration.yaml` добавить сущность слайдера:
```
input_number:
  test1:
    min: 0
    max: 90
    step: 1
```

Сама суть:
1. надо добавить новую панель
2. Войти в режим редактирования (включив переключатель "начать с нуля" в появившемся окне "Получение контроля над панелью")
3. Нажать "получить контроль"
4. Нажать три точки вверху справа
5. Нажать "текстовый редактор"
6. Вставить код из файла [lovelace-dashboard.yaml](https://github.com/Bagunda/HomeAssistant-lesson-mnemonic-cheme-1/blob/main/lovelace-dashboard.yaml)
7. Изменить путь к вашей загруженной картике, которую мы загрзили в п.5 в Подготовке (`/local/images/my_picture.png`). Загружали мы в `/config/www/images/my_picture.png`, а путь указываем `/local/images/my_picture.png`
8. Нажать "Сохранить" сверху справа
9. Нажать крестик сверху слева
10. Нажать "Готово" сверху справа
