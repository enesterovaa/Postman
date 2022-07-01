# Homework 1 Postman


### Создать запросы в Postman 

> Protocol: http
> 
> IP: 162.55.220.72
> 
> Port: 5005



## EP_1


- Method: GET
 
- EndPoint: /get_method
 
- Request url params: 
 
  - name: str
 
  - age: int
 
- Response: 

       [
          “Str”,
    
          “Str”    
        ]

_1. К URL добавить EndPoint `get_method`_ 
http://162.55.220.72:5005/get_method 

_2. Во вкладке Params ввести key `name` , value `Ekaterina` ; key `age`, value `31`_

Response:

 ![image](https://user-images.githubusercontent.com/105673183/176777131-e6449af3-a4f4-4baf-8015-e0106b223574.png)




## EP_2

- Method: POST

- EndPoint: /user_info_3

- Request form data: 

  - name: str
 
  - age: int
 
  - salary: int

- Response: 

        {'name': name,
          'age': age,
          'salary': salary,          
          'family': {'children':          
          [['Alex', 24],
          ['Kate', 12]],       
           'u_salary_1_5_year': salary * 4}
           }

_1. К URL добавить EndPoint `user_info_3`_ 
http://162.55.220.72:5005/user_info_3

_2. Во вкладке Body выбрать form-data. Ввести key `name` , value `Ekaterina` ; key `age`, value `31`; key `salary`, value `1000`_

![image](https://user-images.githubusercontent.com/105673183/176781829-c5f2e95d-9adf-4b44-8a97-cb9a7ac6c334.png)

Response:

![image](https://user-images.githubusercontent.com/105673183/176781900-c5016284-7c00-4537-90a4-d5104637caf9.png)


## EP_3

- Method: GET

- EndPoint: /object_info_1

- Request url params: 
  - name: str
  - age: int
  - weight: int

- Response: 

      {'name': name,
          'age': age,
          'daily_food': weight * 0.012,
          'daily_sleep': weight * 2.5}

_1. К URL добавить EndPoint `object_info_1`_ 
http://162.55.220.72:5005/object_info_1 

_2. Во вкладке Params ввести key `name` , value `Ekaterina` ; key `age`, value `31` , key `weight` , value `53`_


![image](https://user-images.githubusercontent.com/105673183/176845616-c8c9c7a2-0b33-4f58-b339-f5d410effef2.png)



## EP_4

- Method: GET

- EndPoint: /object_info_2

- Request url params: 
  - name: str
  - age: int
  - salary: int

- Response: 

      {'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }

_1. К URL добавить EndPoint `object_info_2`_ 
http://162.55.220.72:5005/object_info_2 

_2. Во вкладке Params ввести key `name` , value `Ekaterina` ; key `age`, value `31`; key `salary`, value `1000`_

![image](https://user-images.githubusercontent.com/105673183/176874380-83691f1a-0456-42ab-81bc-5aac909db7de.png)

Response:

![image](https://user-images.githubusercontent.com/105673183/176875049-e492fa01-73c2-44b2-bfc2-c5453e13fff0.png)

---

## EP_5

- Method: GET

- EndPoint: /object_info_3

- Request url params: 
  
  - name: str

  - age: int

  - salary: int

- Response: 

      {'name': name,
          'age': age,
          'salary': salary,
          'family': {'children': [['Alex', 24], ['Kate', 12]],
                     'pets': {'cat':{'name':'Sunny',
                                     'age': 3},
                              'dog':{'name':'Luky',
                                     'age': 4}},
                     'u_salary_1_5_year': salary * 4}
          }

_1. К URL добавить EndPoint `object_info_3`_ 
http://162.55.220.72:5005/object_info_3 

_2. Во вкладке Params ввести key `name` , value `Ekaterina` ; key `age`, value `31`; key `salary`, value `1000`_

![image](https://user-images.githubusercontent.com/105673183/176876467-e7e10e85-f346-483d-bb56-e21738a7f59c.png)

Response:

![image](https://user-images.githubusercontent.com/105673183/176876630-af6b889f-c061-4085-a1ac-6a7f9c7942ae.png)


---

## EP_6

- Method: GET

- EndPoint: /object_info_4

- Request url params: 

  - name: str

  - age: int

  - salary: int

- Response: 

      {'name': name,
          'age': int(age),
          'salary': [salary, str(salary * 2), str(salary * 3)]}

_1. К URL добавить EndPoint `object_info_4`_ 
http://162.55.220.72:5005/object_info_4 

_2. Во вкладке Params ввести key `name` , value `Ekaterina` ; key `age`, value `31`; key `salary`, value `1000`_

Response:

![image](https://user-images.githubusercontent.com/105673183/176877076-5b8e0d15-253a-451c-9e65-486fce3a621d.png)


---

## EP_7

- Method: POST

- EndPoint: /user_info_2

- Request form data: 

  - name: str

  - age: int

  - salary: int

-Response: 

     {'start_qa_salary': salary,
          'qa_salary_after_6_months': salary * 2,
          'qa_salary_after_12_months': salary * 2.7,
          'qa_salary_after_1.5_year': salary * 3.3,
          'qa_salary_after_3.5_years': salary * 3.8,
          'person': {'u_name': [user_name, salary, age],
                     'u_age': age,
                     'u_salary_5_years': salary * 4.2}
          }

_1. К URL добавить EndPoint `user_info_2`_ 
http://162.55.220.72:5005/user_info_2 

_2. Во вкладке Params ввести key `name` , value `Ekaterina` ; key `age`, value `31`; key `salary`, value `1000`_

![image](https://user-images.githubusercontent.com/105673183/176878010-de4dfad8-37d4-4bbd-89f6-9bd3a232a8e0.png)

Response:

![image](https://user-images.githubusercontent.com/105673183/176878228-7d978b3b-a188-4161-984c-118756edd47e.png)
