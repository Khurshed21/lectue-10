# Axios

Axios - это популярная библиотека для выполнения HTTP-запросов в браузере и на сервере. Она предоставляет удобный интерфейс для работы с сетевыми запросами и обещаниями (promises).
___

# Пример использования

``` Javascript
const axios = require('axios');

axios.get('https://api.example.com/users')
  .then(response => {
    console.log(response.data);
  })
  .catch(error => {
    console.error('Ошибка при выполнении запроса:', error);
  });
```
___

# Цикл событий (Event Loop) в JavaScript

Цикл событий (Event Loop) - это механизм в JavaScript, который позволяет обрабатывать события и выполнять асинхронный код. Он позволяет JavaScript быть однопоточным и все еще обрабатывать несколько задач.
___

# Принцип работы

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSJ01NZRzjo5y2uUA6IpQQfaZelL3R5Dwjd_DnAoNwi-RHOeOtAWZojYcBy-OaEYp5KG2Y&usqp=CAU)
___

``` JavaScript
let acc = 1;
console.log("Call 1:", acc);

acc++;
console.log("Call 2:", acc);

setTimeout(() => {
  acc++;
  console.log("Call 3:", acc);
}, 0);

let anotherAcc = acc;
console.log("Call 4:", anotherAcc, acc);


/* console.log

Call 1: 1
Call 2: 2
Call 4: 2 2
Call 3: 3
```
___

![](https://habrastorage.org/r/w1560/getpro/habr/upload_files/d0b/55a/66f/d0b55a66f050fbfe6668b7074a3bc539.png)

