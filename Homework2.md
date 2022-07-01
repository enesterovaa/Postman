# Homework 2 Postman


## Создать запросы в Postman 

> Protocol: http
> 
> IP: 162.55.220.72
> 
> Port: 5005

---

## Endpoint 1 http://162.55.220.72:5005/first

1. Отправить запрос.

![image](https://user-images.githubusercontent.com/105673183/176884076-fe5e800a-5c1d-4fad-bfe7-bf66c941bcec.png)

2. Статус код 200

![image](https://user-images.githubusercontent.com/105673183/176892264-298037a8-8d10-4c78-8a12-219912fe0274.png)

3. Проверить, что в body приходит правильный string.

![image](https://user-images.githubusercontent.com/105673183/176891962-99ab8070-8e17-44a7-91fb-b029d50dc3d3.png)

---

## Endpoint 2 http://162.55.220.72:5005/user_info_3

1. Отправить запрос.
2. Статус код 200.

![image](https://user-images.githubusercontent.com/105673183/176892868-327b7d4b-e6ce-4417-b806-dbe067570008.png)

3. Спарсить response body в json.

        let resp = pm.response.json();
        console.log("Response body", resp);

![image](https://user-images.githubusercontent.com/105673183/176893292-48065c4e-2587-4ef5-85ea-5205a9b39c6d.png)

4. Проверить, что name в ответе равно name в request (name вбить руками).

![image](https://user-images.githubusercontent.com/105673183/176893424-cbb67353-7c86-4afa-a2f9-8f4292413f3d.png)

5. Проверить, что age в ответе равно age в request (age вбить руками).

![image](https://user-images.githubusercontent.com/105673183/176893646-662630d2-d633-4216-9167-14bfbd30a30a.png)

6. Проверить, что salary в ответе равно salary в request (salary вбить руками).

![image](https://user-images.githubusercontent.com/105673183/176893924-a87cb01a-2f2a-4e5e-a5ae-8ea05e9a1ac4.png)

7. Спарсить request.

        let req = request.data;
        console.log("Request", req);

![image](https://user-images.githubusercontent.com/105673183/176894175-65bb93c3-a985-4b5a-98a9-cf210465cc62.png)

8. Проверить, что name в ответе равно name в request (name забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176894353-4fad2c0d-ef5f-45f9-b47f-155a098d897d.png)

9. Проверить, что age в ответе равно age в request (age забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176894536-dc104a1d-3190-40c6-859c-decc5338eb97.png)

10. Проверить, что salary в ответе равно salary в request (salary забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176894669-98221c9f-5e80-4996-9a96-44d5780cfc76.png)

11. Вывести в консоль параметр family из response.

        console.log("Family", resp.family);

![image](https://user-images.githubusercontent.com/105673183/176894865-22e200db-a1b4-4b52-a5e1-29143c123a4b.png)

12. Проверить что u_salary_1_5_year в ответе равно salary*4 (salary забрать из request)

![image](https://user-images.githubusercontent.com/105673183/176895091-a671b462-9c91-42a7-a0e5-55b6679cf121.png)

---

## Endpoint 3 http://162.55.220.72:5005/object_info_3

1. Отправить запрос.

![image](https://user-images.githubusercontent.com/105673183/176905517-4aa06316-6e10-4030-99d3-4c5d917334d9.png)

2. Статус код 200.
Добавила код проверки 200-го  статуса в общие тесты коллекции.

![image](https://user-images.githubusercontent.com/105673183/176912258-126bad58-9cd1-4fa1-bd6b-b9de193a077f.png)

3. Спарсить response body в json.

4. Спарсить request.

5. Проверить, что name в ответе равно name s request (name забрать из request.)

6. Проверить, что age в ответе равно age s request (age забрать из request.)

7. Проверить, что salary в ответе равно salary s request (salary забрать из request.)

8. Вывести в консоль параметр family из response.

9. Проверить, что у параметра dog есть параметры name.
11. Проверить, что у параметра dog есть параметры age.
12. Проверить, что параметр name имеет значение Luky.
13. Проверить, что параметр age имеет значение 4.

http://162.55.220.72:5005/object_info_4
1. Отправить запрос.
2. Статус код 200
3. Спарсить response body в json.
4. Спарсить request.
5. Проверить, что name в ответе равно name s request (name забрать из request.)
6. Проверить, что age в ответе равно age из request (age забрать из request.)
7. Вывести в консоль параметр salary из request.
8. Вывести в консоль параметр salary из response.
9. Вывести в консоль 0-й элемент параметра salary из response.
10. Вывести в консоль 1-й элемент параметра salary параметр salary из response.
11. Вывести в консоль 2-й элемент параметра salary параметр salary из response.
12. Проверить, что 0-й элемент параметра salary равен salary из request (salary забрать из request.)
13. Проверить, что 1-й элемент параметра salary равен salary*2 из request (salary забрать из request.)
14. Проверить, что 2-й элемент параметра salary равен salary*3 из request (salary забрать из request.)
15. Создать в окружении переменную name
16. Создать в окружении переменную age
17. Создать в окружении переменную salary
18. Передать в окружение переменную name
19. Передать в окружение переменную age
20. Передать в окружение переменную salary
21. Написать цикл который выведет в консоль по порядку элементы списка из параметра salary.
