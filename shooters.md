```js
// Если запустить, выведется '10' десять раз
// Нужно сделать так, чтобы вывелось '0', '1', '2'...
// А почему вообще у меня выводится '10' десять раз ? Все же вроде норм..

var shooters = [];
for (var i = 0; i < 10; i++) {
  shooters.push(() => {
    console.log(i);
  });
}

shooters.forEach((shooter) => shooter());
```