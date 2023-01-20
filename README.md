# Javascript Math sin 

В этом уроке вы узнаете о методе JavaScript Math.sin() с помощью примеров.

>Метод `sin()` вычисляет тригонометрический синус заданного угла и возвращает его.
>  
>**Пример**
>```javascript
>// синус одного градуса
>var value1 = Math.sin(1);
>console.log(value1);    
>
>// Вывод: 0.8414709848078965
>```

-----------------
## sin() Syntax

Синтаксис метода `Math.sin()` следующий:
```javascript
Math.sin(angle)
```
Здесь `sin()` является статическим методом. Следовательно, мы обращаемся к методу, используя имя класса, `Math`.

----------
## sin() Параметр  
Метод `sin()` принимает один параметр:

* `angle` - в радианах, значение синуса которого должно быть вычислено
-----------
## sin() Возвращаемое значение
Метод `sin()` возвращает:

значение синуса заданного `angle` (в радианах).
NaN (Not a Number) для нечислового аргумента

-----------
## Пример 1: JavaScript Math.sin()
```javascript
// синус угла 5 
let value1 = Math.sin(5);
console.log(value1);    

// допускаются отрицательные углы
let value2 = Math.sin(-2);
console.log(value2);    

// Вывод:
// -0.9589242746631385
// -0.9092974268256817
```
В приведенном выше примере,

*`Math.sin(5)` - вычисляет значение синуса угла **5**  
*`Math.sin(-2)` - вычисляет значение синуса угла **-2**

-----------------
## Пример 2: Math.sin() с математическими константами
```javascript
// можно использовать математические константы
let value = Math.sin(Math.PI);
console.log(value);   

 // Вывод: 1.2246467991473532e-16
```
В приведенном выше примере мы использовали метод `sin()` для вычисления синуса математической константы `PI`.

Здесь выход **-1.2246467991473532e-16** представляет собой **-1.2246467991473532 * 10-16**

-------------
## Пример 3: Math.sin() с нечисловыми аргументами
```javascript
let string = "David"

// sin() со строкой в качестве аргумента
let value = Math.sin(string);
console.log(value);    
// Вывод: NaN
```
В приведенном выше примере мы пытались вычислить значение синуса строки `"David"`. Следовательно, на выходе мы получаем **NaN**.

----------
## Пример 4: Math.sin() с аргументом бесконечности
```javascript
// бесконечность как аргумент
let value1 = Math.sin(Infinity);
console.log(value1);

// отрицательная бесконечность как аргумент
let value2 = Math.sin(-Infinity);
console.log(value2);    

// Вывод: 
// NaN
// NaN 
```
Метод `sin()` не рассматривает бесконечность как число, поэтому метод возвращает **NaN** с этим аргументом.

Кроме того, синус бесконечного угла является неопределенным, что не может быть определено с помощью числа.