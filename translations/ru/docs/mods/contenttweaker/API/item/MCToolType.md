# MCToolType

Тип инструментов используется для определения того, какие блоки может быть мой инструмент, или инвертированно, какой инструмент необходим для добычи заданного блока.

Этот класс был добавлен модом с мод-id `contenttweaker`. Так что если вы хотите использовать эту функцию, вам нужно установить этот мод.

## Импорт класса
Вам может потребоваться импортировать пакет, если вы столкнетесь с какими-либо проблемами (например, с заливкой массива), так что лучше быть в безопасности, чем извиняться и добавлять импорт.
```zenscript
mods.contenttweaker.item.MCToolType
```

## Реализованные интерфейсы
MCToolType реализует следующие интерфейсы. Следовательно, методы из них доступны в этом классе.
- [crafttweaker.api.brackets.CommandStringDisplayable](/vanilla/api/brackets/CommandStringDisplayable)

## Конструкторы
Построит объект типа инструмента. Если кто-то с таким именем уже существует, то он будет внутренне указывать на тот же тип инструмента. В противном случае, создается новый с именем (то же самое относится и к скобкам!)
```zenscript
new mods.contenttweaker.item.MCToolType(name as String);
new mods.contenttweaker.item.MCToolType("кирка");
```
| Параметр | Тип    | Описание              |
| -------- | ------ | --------------------- |
| имя      | String | Имя для использования |



## Методы
### getName

Получает имя этого типа инструмента. Имя — это то, что используется в выражении скобки после `<типа инструмента:`

Тип возврата: строка

```zenscript
<tooltype:pickaxe>.getName();
```

### hashCode

Возвращает хэш объекта

Тип возврата: int

```zenscript
<tooltype:pickaxe>.hashCode();
```

### toString

Получить строковое представление этого типа. Это отличается от командной строки!

Тип возврата: строка

```zenscript
<tooltype:pickaxe>.toString();
```


## Свойства

| Название         | Тип    | Имеет Getter | Имеет Setter |
| ---------------- | ------ | ------------ | ------------ |
| командная строка | String | true         | false        |
| имя              | String | true         | false        |

## Операторы
### EQUALS

Сравнивать, если два объекта MCToolType одинаковы

```zenscript
<tooltype:pickaxe> == o как объект
<tooltype:pickaxe> == новый MCToolType("кирка")
```

| Параметр | Тип    | Описание      |
| -------- | ------ | ------------- |
| о        | Объект | Другой объект |

## Утилиты

| Тип результата | Является неявным |
| -------------- | ---------------- |
| String         | false            |
