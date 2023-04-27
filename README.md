### Задание 1

1.  Установите **eCryptfs**.  
2.  Добавьте пользователя cryptouser.  
3.  Зашифруйте домашний каталог пользователя с помощью eCryptfs.  

_В качестве ответа пришлите снимки экрана домашнего каталога пользователя с исходными и зашифрованными данными._  

Вывод ls -la после создания пользователя billy   
![1pic](https://github.com/RSafin12/13.2-Host-protection/blob/main/1.png)  

Логинимся под пользователем billy и создаем файл test с содержанием   
![2pic](https://github.com/RSafin12/13.2-Host-protection/blob/main/2.png)  

Выходим из-под пользователя billy и проверяем его домашний каталог - тестового файла нет. Для проверки сразу логинимся обратно  и для пользователя billy тестовый файл есть   
![3pic](https://github.com/RSafin12/13.2-Host-protection/blob/main/3.png)  

### Задание 2  

1.  Установите поддержку **LUKS**.  
2.  Создайте небольшой раздел, например, 100 Мб.  
3.  Зашифруйте созданный раздел с помощью LUKS.  

_В качестве ответа пришлите снимки экрана с поэтапным выполнением задания._  

Исходные данные  
![21pic](https://github.com/RSafin12/13.2-Host-protection/blob/main/21.png)   
Шифруем раздел  
![22pic](https://github.com/RSafin12/13.2-Host-protection/blob/main/22.png)  
Открываем зашифрованный раздел, проверяем статус  
![23pic](https://github.com/RSafin12/13.2-Host-protection/blob/main/23.png)  
Перезаписываем раздел 0  
![24pic](https://github.com/RSafin12/13.2-Host-protection/blob/main/24.png)  
Создаем файловую систему  
![25pic](https://github.com/RSafin12/13.2-Host-protection/blob/main/25.png)  
Монтируем, создаем тестовый файл  
![26pic](https://github.com/RSafin12/13.2-Host-protection/blob/main/26.png)  
Перепроверяем - размонтируем и монтируем заново. Работает =)  
![27pic](https://github.com/RSafin12/13.2-Host-protection/blob/main/27.png)  


