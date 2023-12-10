# Формат закодированного файла
## Общий принцип
Закодированный файл представляет собой бинарный файл, содержащий
закодированный текст. Файл начинается с метаданных, включающих информацию о
структуре дерева кодирования и расширение файла.


## Метаданные
**Расширение файла:** Сначала сохраняется расширение исходного файла, чтобы
восстановить его при декодировании.

**Структура Дерева:** Затем сохраняется структура дерева Хаффмана, включающая
символы и их коды в представлении дерева.


## Текстовая часть
После метаданных следует закодированный текст. Он содержит все символы
исходного текста, но записанные с помощью особого кода для каждого символа.
Соответствие кода символу выполняется на основании дерева Хаффмана.