---
Title: Выпуск журнала
weight: 2
---

{{< toc >}}

## Общая информация
Чтобы добавить выпуск журнала на сайт:
- подготовьте пакет файлов для загрузки
- загрузите изображения, PDF и таблицу с метаданными на сервер
- создайте новый материал типа "Журнал" на сайте и заполните его поля
- импортируйте статьи
- измените канонические ссылки для дублей статей (если дубли имеются)
- проверьте загруженные данные

## Подготовка пакета файлов
Состав пакета:
- таблицы с метаданными статей выпуска
- файлы с полными текстами статей
- файл с выпуском журнала целиком (только для спецвыпусков)
- изображения:
    - обложка журнала
    - миниатюры первых страниц статей

{{< button href="../files/journal_issue.zip" >}}Скачать пример пакета файлов{{< /button >}}

---

### Таблица с метаданными
- Формат: CSV (кодировка UTF-8)
- Название файла: **articles-import.csv**

### Файлы с полными текстами статей
- Формат: PDF
- Название файлов: **zzr-YYYY-NN-OOO.pdf**, где  
YYYY -- год издания журнала,  
NN -- номер журнала по порядку или код спецвыпуска (PT -- для выпуска по птицеводству, SK -- по скотоводству, SV -- по свиноводству),  
OOO -- номер статьи по порядку  
например, zzr-2020-02-003.pdf или zzr-2018-SV-010.pdf

### Файл с выпуском журнала
- Формат: PDF
- Название файла: **zzr-YYYY-NN.pdf**, где
YYYY -- год издания журнала,  
NN -- номер журнала по порядку или код спецвыпуска (PT -- для выпуска по птицеводству, SK -- по скотоводству, SV -- по свиноводству),  
например, zzr-2020-02.pdf или zzr-2018-SV.pdf

### Изображения
#### Обложка журнала
- Формат: JPG (расширение файла -- .jpg, не .jpeg!)
- Название файлов: **zzr-YYYY-NN.jpg**, где  
YYYY -- год издания журнала,  
NN -- номер журнала по порядку или код спецвыпуска (PT -- для выпуска по птицеводству, SK -- по скотоводству, SV -- по свиноводству),  
например, zzr-2020-02.jpg или zzr-2018-SV.jpg 

#### Миниатюры первых страниц статей 
- Формат: JPG (расширение файла -- .jpg, не .jpeg!)
- Название файлов: **zzr-YYYY-NN-OOO.jpg**, где  
YYYY -- год издания журнала,  
NN -- номер журнала по порядку или код спецвыпуска (PT -- для выпуска по птицеводству, SK -- по скотоводству, SV -- по свиноводству),  
OOO -- номер статьи по порядку  
например, zzr-2020-02-003.jpg или zzr-2018-SV-010.jpg 

{{<hint warning>}}
Регистр букв в названиях любых загружаемых файлов **важен**. Перед загрузкой проверьте, что:
- `zzr` в именах файлов в нижнем регистре (не `ZZR`)  
❌ ZZR-2020-02-003.jpg → ✅ zzr-2020-02-003.jpg
- буквы, обозначающие спецвыпуски -- в верхнем (напр. `SV`, а не `sv`)  
❌ zzr-2018-sv.pdf → ✅ zzr-2018-SV.pdf 
- расширение файла -- в нижнем (напр. `.pdf`, а не `.PDF`)  
❌ zzr-2020-02-003.PDF → ✅ zzr-2020-02-003.pdf 
{{</hint>}}

## Загрузка файлов на сервер
Данные для подключения к серверу запросите у администратора.

На сервер нужно загрузить:
- миниатюры первых страниц *всех* статей журнала -- в папку `article/thumbnails`
- PDF-версии *только открытых* статей журнала -- в папку `article/pdf`
- PDF-файл с выпуском журнала целиком (только для спецвыпусков) -- в папку `journal/pdf`
- таблицу с метаданнными -- в папку `feeds`

---

## Создание материала типа «Журнал»

1. [Авторизуйтесь](../auth) на сайте.

1. Нажмите на ссылку `Материалы -> Добавить матераил -> Журнал` в административном меню сверху.

1. Заполните поля (обязательные помечены звездочкой):

   - **ID**  
   Уникальный идентификатор выпуска журнала. Заполняется по схеме **zzr-YYYY-NN**, где YYYY - год выпуска журнала, NN - месяц выхода журнала или код спецвыпуска (PT -- для выпуска по птицеводству, SK -- по скотоводству, SV -- по свиноводству). Например, zzr-2019-04 или zzr-2018-PT

   - **Год выхода**

   - **Номер журнала / код спецвыпуска**  
   Выберите значение из выпадающего списка.

   - **Обложка**  
   Загрузите обложку журнала, подготовленную на предыдущем этапе.

   - **Партнеры**  
   Введите названия компаний-партнеров по одному на строку (нажмите `Добавить еще` для вставки пустой строки). Если партнера нет в списке партнеров, [добавьте его](../partner)

1. Нажмите `Сохранить` и убедитесь, что название, номер и год выпуска журнала верны.

---

## Импорт статей

1. Нажмите на ссылку `Материалы -> Потоки данных` в административном меню сверху.
1. Нажмите кнопку `Импортировать` напротив пункта **Импорт статей** в списке.
1. Нажмите синюю кнопку `Импортировать` и дождитесь окончания импорта.
1. Если при импорте возникли ошибки, проверьте имя загруженной на сервер таблицы с метаданными и корректность заполнения ячеек таблицы.

---

## Изменение канонических ссылок дублей статей  

Если в выкладываемом номере есть статьи, уже присутствующие на сайте (дубли), то для всех дублей нужно [изменить канонические ссылки](../article/metatags/#изменение-канонической-ссылки). Чаще всего дубли встречаются в спецвыпусках журналов и повторяют статьи из основных выпусков.

В качестве канонической ссылки нужно вставить конструкцию `[site:url]/<ID оригинальной статьи>`. 

{{< button href="../article/metatags/#изменение-канонической-ссылки" >}}Подробная инструкция по замене канонических ссылок{{< /button >}}

{{< hint title="Пример" >}}

Допустим, выкладывается спецвыпуск по свиноводству за 2019 год. В выпуске присутствует статья *"Ящур: профилактика и меры борьбы"*, которая уже есть на сайте в рамках апрельского номера за 2019 год (адрес статьи https://zzr.ru/zzr-2019-04-022, ID статьи -- `zzr-2019-04-022`).

Значит, после импорта статей для спецвыпуска нужно изменить каноническую ссылку у статьи **в спецвыпуске** на `[site:url]/zzr-2019-04-022`. В ранее выложенной статье ничего менять не нужно.

{{</ hint >}}

---

## Проверка данных

1. Нажмите на ссылку `Материалы` в административном меню сверху.
1. В выпадающем меню **Тип материала** выберите **Журнал** и нажмите на кнопку `Фильтр` .
1. В списке выберите размещаемый журнал.
1. Проверьте, что содержание номера загрузилось корректно.
1. Перейдите по каждой ссылке в содержании и убедитесь, что все данные (изображения, текст, ссылки на PDF-файлы) загрузились корректно.
1. Опубликуйте выпуск журнала.


## Публикация всех ПДФ-версий статей выпуска

Для того, чтобы посетителям были доступны все ПДФ-версии опубликованного ранее выпуска журнала:

1. Подготовьте все статьи выпуска в соответствии с [требованиями к файлам полных текстов статей](#файлы-с-полными-текстами-статей).
1. Загрузите подготовленные файлы в папку `article/pdf` на сервере.
1. [Авторизуйтесь](../auth) на сайте.
1. Нажмите на ссылку `Материалы` в административном меню сверху.
1. В меню "Тип материала" выберите "Журнальная статья", в поле "Год выхода" введите год выпуска, статьи которого планируется открыть, в поле "Номер журнала / Код спецвыпуска" выберите соответствующий выпуск.
1. Нажмите кнопку `Фильтр`.
1. Нажмите на квадратик рядом со словом "Заголовок" над списком материалов (выделятся все статьи).
1. В меню "Действие" выберите "Сохранить материал".
1. Нажмите кнопку "Применить к отмеченным позициям"

![](../img/publish_all_pdf.gif)
