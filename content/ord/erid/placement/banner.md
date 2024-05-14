---
title: Размещение токена для баннера
weight: 2
bookToc: false
---

ERID-токен дописывается к ссылке для баннера (по определенным правилам, см. ниже). Для размещения токена добавьте его в поле `Ссылка к баннеру`:
   ![](../img/zzr_banner_link_field.png)

## Правила добавления токена к ссылке

- Если изначальная ссылка для баннера _не содержит параметров_ (в ней нет знака `?`), то в конец ссылки нужно добавить `?erid=xxxxxxx`, где `xxxxxxx` -- ERID-токен

{{<hint title="Примеры">}}
- https://example.com → https://example.com?erid=2SDnjc2d4Tb
- https://example.com/page → https://example.com/page?erid=2SDnjc2d4Tb
{{</hint>}}

- Если изначальная ссылка для баннера _содержит параметры_ (в ней есть один знак `?`), то в конец ссылки нужно добавить `&erid=xxxxxxx`, где `xxxxxxx` -- ERID-токен

{{<hint title="Примеры">}}
- https://example.com?utm_source=zzr → https://example.com?utm_source=zzr&erid=2SDnjc2d4Tb
- https://example.com/page?utm_source=zzr → https://example.com/page?utm_source=zzr&erid=2SDnjc2d4Tb
- https://example.com?utm_source=zzr&utm_campaign=test → https://example.com?utm_source=zzr&utm_campaign=test&erid=2SDnjc2d4Tb
{{</hint>}}