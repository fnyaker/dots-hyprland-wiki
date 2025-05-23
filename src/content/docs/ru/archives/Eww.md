---
title: Eww (multiple)
layout: /src/layouts/autonum.astro
sidebar:
  badge:
    text: Устарело
    variant: caution
lastUpdated: 2025-05-01
---

:::danger[Внимание]
Данные сборники конфигураций больше не поддерживаются. Мы не рекомендуем их использовать.
:::

# Описание
Несколько сборников конфигураций, такие как `windoes`, `hybrid` и `NovelKnock`, и т.д.
# Установка
- Зависимости: для каждой ветки свой список.
- Скопировать
    - `.config`, `.local` в вашу домашнюю директорию
    - Директории из `.local/share/icons` в `/usr/share/icons`
    - Опционально из папки `Import manually` по необходимости

 ## Производительность
|  ⌄  | Рекомендуется | Не рекомендуется | Заметки                 |
| --- | ------ | ----------- | ------------------------- |
| Ядро |     | cachyos, xanmod | Не злоупотребляйте средствами энергосбережения. Понятия не имею что я несу - это прсто из личного опыта. |
| Оболочка входа | bash/zsh | fish | Но в терминале fish использовать нормально - что end_4, собственно, и делает |

 ## Конфигурация
 - eww конфиги нормально работают только в `~/.config/eww`
 - Запускайте eww с помощью `eww daemon`
 - Чтобы открыть верхнюю панель: `eww open bar`
 - Чтобы открыть панель Windows: `eww open winbar` (ветки `windoes`/`hybrid`)
 - Чтобы открыть нижнюю строку: `eww open bottomline` (чтобы окно музыки открывалось, когда кликаете нижнюю границу экрана)
 - Откройте обозреватель (средняя кнопка мыши по рабочим пространствам) и подождите 10 секунд (чтобы сформировался кэш поиска приложений, иначе иконки буду неправильно отображаться)
 ## Использование
 - Управление музыкой: средняя кнопка мыши для Воспроизведения/Паузы, правая кнопка для перехода к следующему треку, колесико для изменения громкости
 - Обозреватель: средняя кнопка мыши по индикатору рабочих пространств или команда `eww open overview`
 - Набирайте текст в Обозревателе, чтобы искать приложения (больше информации ниже)
 ## Поиск
 - Набирайте текст для поиска приложений
 - Набирайте математические выражение (должны начинаться с чисел) чтобы получать результат с помощью `qalc`
 - `>save THEME`: Сохраняет текущую цветовую схему, где THEME будет вашим названием.
 - `>load THEME`: Загружает сохраненную тему. Доступные темы будут появляться по мере набора текста.
 - `>music`: Изъять цветовую схему из плашки проигрываемого материала
 - `>wall`: Изъять цветовую схему из обоев расположенных в `~/.config/eww/images/wallpaper/wallpaper`
 - `>light`: Использовать светлый режим в последующих цветовых схемах
 - `>dark`: Использовать темный режим в последующих цветовых схемах
 - `>one`: Использовать только один цвет для иконок на панели в последующих цветовых схемах
 - `>multi`: Использовать различные цвета для иконок на панели в последующих цветовых схемах
 - `>r`: Перезагрузка (закрывает и перезапускает eww со стандартной панелью)
