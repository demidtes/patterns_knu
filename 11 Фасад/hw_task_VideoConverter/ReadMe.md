# Кодування відео

Конвертування відео з одного формату в інший це багатокроковий процес,
що вимагає використання цілої серії допоміжних інструментів.

Замість цього можна реалізувати шаблон проєктування Фасад,
що надає користувачеві лише один простий метод, приховуючи за
собою цілу систему з відеокодеками, аудіомікшерами та
іншими, не менш складними об'єктами. 

Цей метод повинен приймати на вхід файл, який необхідно перекодувати 
та формат у який необхідно перетворити файл

```java
public VideoFile convert(VideoFile file, Codec codec) {
    ...
    return newVideoFile;
}
```

Проведіть рефакторинг коду із застосуванням шаблону проєктування
Фасад, щоб спростити роботу клієнта зі складною бібліотекою відеоконвертації.


