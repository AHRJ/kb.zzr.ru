---
title: Анонс журнала
weight: 2
---

{{< toc >}}

**Анонс журнала** -- шаблон письма с анонсами и ссылками на статьи свежевышедшего номера журнала "Животноводство".
Пример готового анонса журнала можно посмотреть <a href="../issue_announcement_example.html" target="_blank">здесь</a>.


## Создание анонса журнала

1. [Авторизуйтесь](../../auth) в генераторе рассылок.
1. Кликните на ссылку `Добавить` рядом с пунктом `Анонсы журнала`. ![](../img/issue_announcement_create.png)
1. Заполните поля:
    - **Журнал**: выпуск журнала, для которого готовится анонс (список журналов подгружается автоматически с сайта zzr.ru при создании нового анонса).
    - **Тема письма**: обычно это что-то в духе "Животноводство России - Июль 2022"
    - **Приветствие**: небольшой (около 300 знаков с пробелами) текст от главного редактора. Для форматирования текста используйте [Маркдаун](https://paulradzkov.com/2014/markdown_cheatsheet/).
    - **Рекламный блок**: предварительно сверстанный в HTML-формате блок (как правило, ссылки на соцсети ИД). Размещается после 4-го анонса статьи из журнала.
    - **Рекламный баннер**: изображение со ссылкой на сайт. Рекламные баннеры можно [добавлять самостоятельно](../../entities/ad_banner#добавление-рекламного-баннера). Размещается после 4-го анонса статьи из журнала.
    - **Дата отправки**: дата и время, в которое [рассылочный сервис](../../../sendpulse) отправит рассылку. Не может быть меньше текущей.
    - **Адресные книги**: группы емейлов, по которым может проводиться рассылка. По-умолчанию выбрана книга "Общая база", то есть рассылка будет проводится по всем существующим адресатам. Если нужно разослать письмо по более узкой группе, можно выбрать ее в списке (например, "Хозяйства"). Можно выбрать более одной адресной книги, если зажать клавишу Ctrl и кликнуть мышкой по несколькним книгам. Адресные книги формируются и хранятся в [рассылочном сервисе](../../sendpulse), но могут быть [подгружены](../address_books) в генератор рассылок.
    - **Статьи с анонсом**: блок с подробной информацией по каждой статье (изображение, заголовок, анонс). Статьи автоматически подгружаются с сайта zzr.ru в момент создания Анонса номера, загруженную информацию можно [отредактировать](../entities/article).
    - **Другие статьи**: блок с заголовками-ссылками на другие статьи номера.
1. Нажмите `Сохранить`. После нажатия будет виден список всех анонсов журнала.


## Просмотр и редактирование анонса журнала
См. [просмотр и редактирование новостного дайждеста](../news_digest#просмотр-и-редактирование-новостного-дайджеста)



## Планирование к отправке и отмена отправки анонса журнала
См. [планирование к отправке и отмена отправки новостного дайджеста](../news_digest#планирование-к-отправке-и-отмена-отправки-новостного-дайджеста)


## Удаление анонса журнала
См. [удаление новостного дайджеста](../news_digest#удаление-новостного-дайджеста)

{{< hint type="warning">}}
Если удалить *запланированный* анонс, то он все равно будет отправлен. Если вы удалили запланированный анонс, и нужно отменить его отправку, обратитесь к администратору сайта.
{{< /hint >}}