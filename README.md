# Яндекс Практикум

Во время обучения в Яндекс Практикуме (ссылка на платформу https://practicum.yandex.ru/qa-engineer/) мною было протестировано 6 приложений Яндекса.<br />

Здесь я расскажу про самый масштабный проект - это тестрирование веб- и мобильной версии, а также API приложения Яндекс Самокат. Я спроектировала и выполнила проверки приложения Яндекс Самокат, оформила баг-репорты (раздел 1, раздел 2, раздел 4). Тестирование API приложения я проводила, используя инструмент Postman (раздел 3). Работу в Charles я покажу при тестировании фичи, которую реализовали только во фронтенде, а бэкенд ещё не был готов (раздел 5).
В приложении Яндекс Самокат было обнаружено порядка 50 багов. Примеры оформления баг-репортов в YouTrack можно посмотреть по [ссылке](https://elena-s.youtrack.cloud/issues?q=тег:%20Диплом)<br />

## Описание проекта:

Приложение Яндекс Самокат - это сервис, который позволяет арендовать электрический самокат на несколько дней.<br />

**1. Тест-анализ** <br />
Задача: Декомпозировать и визуализировать требования, исключить серые зоны<br />
Инструменты: Figma, draw.io<br />
Результат: Построение mindmap для формы заказа самоката<br />

Прежде чем проектировать проверки, необходимо определить, что предстоить тестировать, проанализировать требования и макеты, составить список объектов тестирования. Для проведения тестирования веб-приложения Яндекс Самокат макеты были представлены в Figma. Далее каждый объект тестирования необходимо декомпозировать и визуализировать, а затем найти серые зоны.<br />

Декомпозицию и визуализацию требований я покажу на примере формы заказа самоката. Для формы заказа самоката, используя инструмент draw.io, я разработала mindmap, где отобразила логику работы веб-приложения и вёрстку.<br />

Mindmap можно посмотреть по [ссылке](https://drive.google.com/file/d/102bFT7mJ7DYv8sHS6mkDK7q1Ih9zg3TV/view?usp=sharing) <br />

Декомпозируя требования до атомарного уровня, мне удалось закрыть много серых зон.

**2. Тест-дизайн** <br />
После проведения тест-анализа переходим к проектированию тестовой документации. Техники тест-дизайна, которые я применяла: разбиение по классам эквивалентности и выделение граничных значений.

*2.1 Составление чек-листов* <br />

Пример составления чек-листа для формы "Статус заказа" [здесь](https://docs.google.com/spreadsheets/d/18hV4HR-UZvtfX5aoAEnhuhZeLBvwdoAAsKLePHcO2uA/edit?usp=sharing)<br />

Применение техник тест-дизайна хорошо видно при составлении проверок на валидацию полей для формы заказа самоката. Посмотреть, как я применяла техники тест-дизайна можно, перейдя по [ссылке](https://docs.google.com/spreadsheets/d/18hV4HR-UZvtfX5aoAEnhuhZeLBvwdoAAsKLePHcO2uA/edit?usp=sharing)<br />

*2.2 Составление тест-кейсов* <br />

Пример составления тест-кейса очень хорошо представлен при тестировании мобильной версии приложения Яндекс Самокат.<br /> [Здесь](https://docs.google.com/spreadsheets/d/18hV4HR-UZvtfX5aoAEnhuhZeLBvwdoAAsKLePHcO2uA/edit?usp=sharing) можно посмотреть тест-кейсы, составленные при тестировании нотификации и отсутствии интернет-соединения.<br />

**3. Тестирование API** <br />
Документация к API была представлена в Apidoc (https://github.com/Shvarikova-Elena/first-project/blob/main/pics/Apidoc.jpg). Тестирование API проводила через Postman.



