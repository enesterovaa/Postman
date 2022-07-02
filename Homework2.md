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

8. Проверить, что name в ответе равно name из request (name забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176894353-4fad2c0d-ef5f-45f9-b47f-155a098d897d.png)

9. Проверить, что age в ответе равно age из request (age забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176894536-dc104a1d-3190-40c6-859c-decc5338eb97.png)

10. Проверить, что salary в ответе равно salary из request (salary забрать из request).

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

        let resp = pm.response.json();
        console.log("Response", resp);
        
![image](https://user-images.githubusercontent.com/105673183/176961020-83bf9155-1c4f-47ff-8eca-e0574cfd2107.png)
       

4. Спарсить request.

        let req = pm.request.url.query.toObject()  
        console.log("Request", req);
        
![image](https://user-images.githubusercontent.com/105673183/176961164-e4359d3a-3a55-4386-bfdf-07b6c7e0bf80.png)
        
5. Проверить, что name в ответе равно name в request (name забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176961389-4ae79e4f-fd88-4046-96b3-ce226a27499e.png)

6. Проверить, что age в ответе равно age в request (age забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176961445-ae13857a-74d3-4edf-8faa-d514de9bb7bd.png)

7. Проверить, что salary в ответе равно salary в request (salary забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176961526-9d1abca0-70b8-43ba-acc8-d3ed1da5ae7d.png)

8. Вывести в консоль параметр family из response.

        console.log("Family", resp.family);
        
![image](https://user-images.githubusercontent.com/105673183/176961714-b3ea0f40-c57c-4e87-b966-d4f99549c1bb.png)
        
9. Проверить, что у параметра dog есть параметры name.

![image](https://user-images.githubusercontent.com/105673183/176961802-6c18778c-a723-4f0a-8317-466e43a5ae38.png)

10. Проверить, что у параметра dog есть параметры age.

![image](https://user-images.githubusercontent.com/105673183/176961913-af25b180-6086-47ac-bfd9-56a4fca0fb5d.png)

11. Проверить, что параметр name имеет значение Luky.

![image](https://user-images.githubusercontent.com/105673183/176961961-de2ca3aa-8b2f-471d-ae15-b47f0e6bcbee.png)

12. Проверить, что параметр age имеет значение 4.

![image](https://user-images.githubusercontent.com/105673183/176962029-97e5a967-9594-4209-b80e-e72ecd3f5116.png)

---

## Endpoint 4 http://162.55.220.72:5005/object_info_4

1. Отправить запрос.

![image](https://user-images.githubusercontent.com/105673183/176962422-d98b684e-4a44-4728-b179-1c1555ceb4bc.png)

2. Статус код 200

Добавила код проверки 200-го  статуса в общие тесты коллекции.

![image](https://user-images.githubusercontent.com/105673183/176912258-126bad58-9cd1-4fa1-bd6b-b9de193a077f.png)

3. Спарсить response body в json.

        let resp = pm.response.json();
        console.log("Response", resp);

![image](https://user-images.githubusercontent.com/105673183/176962712-2aa6b242-84dc-4015-96a4-352075f3dbc0.png)

4. Спарсить request.

        let req = pm.request.url.query.toObject()  
        console.log("Request", req);

![image](https://user-images.githubusercontent.com/105673183/176962765-453dbdc1-c4ed-4507-8fff-278287eb9fc1.png)

5. Проверить, что name в ответе равно name из request (name забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176962883-d6f3ae71-c497-4995-a209-f634dcbc70ae.png)

6. Проверить, что age в ответе равно age из request (age забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176962997-a2a46a3f-4157-418e-853d-df2537137c3a.png)

7. Вывести в консоль параметр salary из request.

        console.log("Request salary ", req.salary);

8. Вывести в консоль параметр salary из response.

        console.log("Response salary ", resp.salary);

9. Вывести в консоль 0-й элемент параметра salary из response.

        console.log("Response salary [0] ", resp.salary[0]);

10. Вывести в консоль 1-й элемент параметра salary параметр salary из response.

        console.log("Response salary [1] ",resp.salary[1]);
        
11. Вывести в консоль 2-й элемент параметра salary параметр salary из response.

        console.log("Response salary [2] ",resp.salary[2]);
        
![image](https://user-images.githubusercontent.com/105673183/176963676-d66597fe-6b51-440f-9762-0b65eadb8d15.png)
        
12. Проверить, что 0-й элемент параметра salary равен salary из request (salary забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176963764-256936c3-3365-4b79-810c-e45e2dfe00f1.png)

13. Проверить, что 1-й элемент параметра salary равен salary*2 из request (salary забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176963900-1ab62c83-8025-47dd-838e-4124bc52d08c.png)

14. Проверить, что 2-й элемент параметра salary равен salary*3 из request (salary забрать из request).

![image](https://user-images.githubusercontent.com/105673183/176963954-71e50ec1-2275-4b73-9a3a-e13ee8df7692.png)

15. Создать в окружении переменную name

16. Создать в окружении переменную age

17. Создать в окружении переменную salary

Environments -> + -> HW_2 -> name; age; salary. Значения оставить пустыми.

18. Передать в окружение переменную name

        pm.environment.set("name", req.name);

19. Передать в окружение переменную age

        pm.environment.set("age", req.age);

20. Передать в окружение переменную salary

        pm.environment.set("salary", req.salary);

![image](https://user-images.githubusercontent.com/105673183/176964299-d941b2e2-81f9-4141-b77e-f40830ce3da6.png)

21. Написать цикл который выведет в консоль по порядку элементы списка из параметра salary.

        for (let i of resp.salary) {  
                console.log("Loop", i);  
        }
        
![image](https://user-images.githubusercontent.com/105673183/176964594-9119864e-36a2-4c1c-8e34-16dd5bc82b6a.png)

---

## Endpoint 5 http://162.55.220.72:5005/user_info_2

1. Вставить параметр salary из окружения в request

2. Вставить параметр age из окружения в request

3. Вставить параметр name из окружения в request

4. Отправить запрос.

![image](https://user-images.githubusercontent.com/105673183/176971270-d2dc520c-a1ad-467f-8f3e-56364c2ea0a8.png)

5. Статус код 200.

Добавила код проверки 200-го  статуса в общие тесты коллекции.

![image](https://user-images.githubusercontent.com/105673183/176912258-126bad58-9cd1-4fa1-bd6b-b9de193a077f.png)

6. Спарсить response body в json.

        let resp = pm.response.json();
        console.log("Response", resp);

![image](https://user-images.githubusercontent.com/105673183/176971416-41c695ec-649c-41f6-9b85-b3241f33b619.png)

7. Спарсить request.

        let req = request.data
        console.log("Request", req);

![image](https://user-images.githubusercontent.com/105673183/176971440-b95d4604-9d36-4343-879b-5b8cfc43f389.png)

8. Проверить, что json response имеет параметр start_qa_salary.

![image](https://user-images.githubusercontent.com/105673183/176971600-90c7c192-c60e-49d2-8220-e381d394b937.png)

9. Проверить, что json response имеет параметр qa_salary_after_6_months.

![image](https://user-images.githubusercontent.com/105673183/176971756-9412efa9-a954-40f9-ab78-994adb605c93.png)

10. Проверить, что json response имеет параметр qa_salary_after_12_months.

![image](https://user-images.githubusercontent.com/105673183/176971811-d446a559-7c9d-4aec-a2c1-22ffc59f1b9b.png)

11. Проверить, что json response имеет параметр qa_salary_after_1.5_year.

![image](https://user-images.githubusercontent.com/105673183/176971887-986095ab-6cd3-4800-a37a-bc2592047115.png)

12. Проверить, что json response имеет параметр qa_salary_after_3.5_years.

![image](https://user-images.githubusercontent.com/105673183/176971937-c2c2caee-4eaa-4d4c-9239-afbb2c6ad298.png)

13. Проверить, что json response имеет параметр person.

![image](https://user-images.githubusercontent.com/105673183/176972062-9ab8fced-bc1e-4b6d-8b54-bfe1cd066d3a.png)

14. Проверить, что параметр start_qa_salary равен salary из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/105673183/176973981-8063c057-757d-4f5b-9701-52773e7e2961.png)

15. Проверить, что параметр qa_salary_after_6_months равен salary*2 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/105673183/176974038-34f3753c-1f99-47d5-aa00-f0b57e442604.png)

16. Проверить, что параметр qa_salary_after_12_months равен salary*2.7 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/105673183/176974232-6ea6e066-18d7-4ec7-8c0b-4e014d2b2f28.png)

17. Проверить, что параметр qa_salary_after_1.5_year равен salary*3.3 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/105673183/176974297-fbd52cf1-cdcd-48c2-993f-8ad1bd0b1aaf.png)

18. Проверить, что параметр qa_salary_after_3.5_years равен salary*3.8 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/105673183/176974426-f6186474-cda8-408f-89e0-0e672f6d6929.png)

19. Проверить, что в параметре person, 1-й элемент из u_name равен salary из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/105673183/176974476-1b61acf3-794a-40d9-927a-e44e747f0c95.png)

20. Проверить, что что параметр u_age равен age из request (age забрать из request.)

![image](https://user-images.githubusercontent.com/105673183/176974507-0a62eaa8-0a55-4ccb-9fb5-7c6341e554b7.png)

21. Проверить, что параметр u_salary_5_years равен salary*4.2 из request (salary забрать из request.)

![image](https://user-images.githubusercontent.com/105673183/176974555-b3cdff98-a655-43e3-b4f1-f17e92df192d.png)

22. ***Написать цикл который выведет в консоль по порядку элементы списка из параметра person.

        for (let i in resp.person) {  
        console.log("Loop", i);  
	    }
            
![image](https://user-images.githubusercontent.com/105673183/176974762-dd2267c0-04aa-47ba-8b53-5939e7040c78.png)
            
