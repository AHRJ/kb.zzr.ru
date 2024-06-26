---
Title: UTM-метки
weight: 2
---

{{< toc >}}

UTM-метка — это специальный формат разметки URL-адресов в виде кодов. По сути, это теги, которые вы добавляете к ссылке для учета статистики по переходам с рекламных площадок.

Когда пользователь делает клик на ссылке с метками, эти коды отправляются в Яндекс.Метрику и отображаются в отчетах, предоставляя дополнительную информацию об источниках трафика.


## Создание UTM-меток

1. Перейдите на страницу-генератор меток <a href="https://tilda.cc/ru/utm" target="_blank">Tильды</a>.
1. В поле "Адрес вашей страницы" выберите "https://" вместо "http://" и введите `zzr.ru` (или любую другую страницу на zzr.ru) в поле для адреса.
1. В поле "Источник кампании" введите адрес сайта, на котором размещается реклама (например, example.ru). Адрес нужно вводить без префиксов `http://` или `www`. 
1. В поле "Тип трафика" введите тип рекламы (например, `banner`). 
1. В поле "Название кампании" введите название рекламной кампании. Можно ввести `general`, если не предполагается ведение нескольких рекламных кампаний с указанной рекламной площадкой. 
1. При желании можно заполнить поля с необязательными параметрами: "Идентификатор объявления" и "Ключевое слово".
1. Скопируйте сгенерированную в поле "Результат" ссылку и передайте ее представителю компании, которая размещает рекламу. Статистика по переходам будет собираться в Яндекс-Метрике.
![](../img/utm-generator.png)



## Просмотр статистики по переходам
1. Зайдите в ["Яндекс-метрику"](../yametrika/). 
1. Перейдите на страницу "Метки UTM" (Боковое меню, пункт `Отчеты` → `Источники` → `Метки UTM`). 
![](../img/utm-stats.png)
