# Практика «TaxiOrder» v2

Перенесите в этот проект ваше решение задачи «TaxiOrder».

Ознакомьтесь с новым ключевым словом [record](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/record), появившимся в .NET 5.

1. Избавьтесь от `ValueType` и сделайте всех его наследников record'ами. Запустите тесты.


Помимо прочего, record'ы позволяют создавать иммутабельные типы. Иммутабельность гарантирует, что никакие свойства объекта не меняются в течение всего его времени жизни.
Основное назначение иммутабельных объектов - безопасность. Любое изменение приводит к созданию копии, поэтому ссылку на исходный объект можно сохранить в общедоступном
месте (например, в кэше) и не беспокоиться, что содержимое объекта изменится. Пример иммутабельного объекта - класс `string`.
Для record'ов доступен новый синтаксис `with`, ознакомьтесь с ним. Изучите, для чего нужен модификатор доступа `init`.

2. Сделайте все ваши record'ы иммутабельными. Добавьте в API метод `GetDriverAnonimousInfo`, аналогичный `GetDriverFullInfo`, но вместо персональных данных печатающий звёздочки.
Число звёздочек должно совпадать с длиной исходной строки. Под персональными данными понимаются имя, фамилия и номер автомобиля.
