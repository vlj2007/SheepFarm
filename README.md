# Сценарий овцефермы
Есть виртуальная овцеферма, нужно создать несколько овец со схожими характеристиками. Вместо того, чтобы создавать каждую овцу с нуля, вы можете использовать шаблон Prototype для клонирования существующих овец. Каждая клонированная овца сохранит общие атрибуты, но при этом она поддерживает индивидуальную настройку.

### 1. Определите интерфейс прототипа
### 2. Реализация конкретных прототипов
### 3. Клиентский код: использование Прототипа

## Объяснение

* Прототип: Интерфейс Prototype определяет метод clone, который будет использоваться для создания копий объектов.
* Конкретные прототипы: Классы ConcretePrototypeA и ConcretePrototypeB являются реализациями интерфейса Prototype. Они реализуют метод clone, чтобы вернуть новые экземпляры самих себя, копируя необходимые поля.
* Клиентский код: В методе main создаются объекты-прототипы, которые затем клонируются. Оригиналы и клонированные объекты выводятся в консоль, чтобы продемонстрировать, что клонирование прошло успешно.

## Где использовать паттерн Prototype:

* Когда создание новых экземпляров объектов через конструкцию является затратным: Если создание объектов требует много времени или ресурсов, клонирование может быть более эффективным.
* Когда речь идет об объектах с сложной конфигурацией: Если объект имеет множество параметров, использование прототипов может облегчить создание новых экземпляров.
* Когда необходимо иметь возможность динамически настраивать или изменять объекты: С помощью клонирования можно легко создавать новые объекты с измененными свойствами, особенно если эти свойства зависят от времени или контекста.
* Когда объекты имеют одинаковую структуру, но разные свойства: Можно создать общий прототип и клонить его, изменяя только некоторые параметры.

Паттерн Prototype предоставляет гибкий способ создания объектов, что особенно полезно в системах, где множество экземпляров имеют схожую структуру, но отличаются параметрами.
