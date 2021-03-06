---
Title: Метатеги статьи 
weight: 7
---

{{< toc >}}

У каждой статьи на сайте кроме основного текста есть т.н. "метаинформация". Эта информация обычно не видна пользовалетям и используется для поисковой оптимизации. Данный раздел описывает некоторые из метатегов.

## Метатег `title`

Метатег title — это базовый элемент HTML-разметки, который в лаконичной форме демонстрирует пользователям и поисковым роботам основную смысловую и тематическую нагрузку страницы.

### Изменение метатега `title`

1. [Авторизуйтесь](../../auth) на сайте.
1. Выберите статью, для которой нужно изменить метатег `title` и нажмите `Редактировать`.
1. В правой части окна раскройте пункт **Metatags**, в нем подпункт **Основные теги** и найдите пункт **Заголовок страницы**. По-умолчанию он содержит текст `[node:title]`.
![](../img/page_title_metatag.png)
1. Текст в поле замените на любой требуемый.
1. Нажмите кнопку `Сохранить` внизу страницы.


## Каноническая ссылка статьи

Каноническим называется адрес страницы, которую поисковые роботы считают главной среди нескольких ее вариантов сайте. Например, если одна и та же страница размещена по нескольким адресам, таким как example.com?dress=1234 и example.com/dresses/1234, одна из версий будет выбрана в качестве канонической.

### Изменение канонической ссылки

1. [Авторизуйтесь](../../auth) на сайте.
1. Выберите статью, для которой нужно изменить каноническую ссылку и нажмите `Редактировать`.
1. В правой части окна раскройте пункт **Metatags**, в нем подпункт **Расширенные** и найдите пункт **Канонический URL**. По-умолчанию он содержит текст `[node:url]`.
![](../img/page_canonical_url.png)
1. Замените текст по-умолчанию на `[site:url]<ссылка на каноническую страницу>`, например `[site:url]zzr-2017-07-009`
1. Нажмите кнопку `Сохранить` внизу страницы.
