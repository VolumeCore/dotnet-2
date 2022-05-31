
# Приложение Канбан-доска

**Доска для мониторинга задач и распределения их по статусам**
*Тепечин Роман, гр. 6312-100503D*

| Связь со мной | 👀 |
| ------ | ------ |
| Telegram | [VolumeCore](https://t.me/volumecore) |
| Discord | VolumeCore⚡#2116 |

С помощью канбан-доски можно добавлять задачи с определением её категории,
а при необходимости менять статус задачи, перетаскивая её из одной ячейки в другую

> Демонстрация работы канбан-доски
![Alt text](https://psv4.vkuseraudio.net/s/v1/d/uNlF6390yc2tlwSiKylpmj71gltwlEijn9-wttYw9mXSRbGl_V34OH0vZSE9FULjDpZO-Bn7r6eB8TexMO96l4CQdj-qU1f5me4fFx9QrOLkbW5hpEgODw/wer1.gif)

> Демонстрация работы CRUD операция с категориями / задачами
![Alt text](https://sun7-14.userapi.com/s/v1/d/DkM7SmqCLDuCwRs9uXsCjEfVSB22glM7XhkQjU_mP5aXg83iL6z-s2YlRtq6h-A1PX1KXa-rWnHtthQpwrrK3hKN8u6v_N6vHAh20yDhR7rDF_68crhvKQ/wer2.gif)
## Сервер

- Наличие CRUD операций для статусов задач и самих задач
- xUnit тесты для репозиториев задач и статусов
- Использован ASP.NET Core Web-API
- Хранение всех данных происходит путём сериализации всех данных в XML формат
- Сервер способен работать с веб-приложением

## Клиент

- Реализован на Angular
- Для создания Drag and Drop использован Angular CDK
- Большинство стилей взято из Angular Material
- Возможность добавлять / удалять / редактировать задачи и категории

## Установка и запуск
1. Склонировать репозиторий
2. Запустить сервер в Visual Studio из папки `Kanban-board`
3. Открыть папку `Kanban-board-client`
4. В этой папке открыть терминал и установить зависимости
4.1 При необходимости поменять адрес сервера в `src/app/services/data.service.ts`
```sh
npm i
ng serve
```