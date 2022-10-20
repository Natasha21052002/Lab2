# Lab2

Анализ данных с помощью описательных статистик и графиков

<img width="401" alt="image" src="https://user-images.githubusercontent.com/98012309/196930553-e33656a8-8408-448b-bc11-5c1e4afac1c5.png">

<img width="438" alt="image" src="https://user-images.githubusercontent.com/98012309/196930630-6d8e0d68-5c4a-4cfa-a59e-f73239ad2d99.png">

По графикам видно, что данные распеределены не по нормальному закону распределения

Корреляционная матрица по всем наблюдениям 

<img width="248" alt="image" src="https://user-images.githubusercontent.com/98012309/196932254-b597ae4c-25cc-4074-bd14-a0f4f19f9550.png">

Корреляционная матрица по классу частных университетов 

<img width="241" alt="image" src="https://user-images.githubusercontent.com/98012309/196932318-ffec708b-f96e-4a96-95ad-3af9f5fe8c86.png">

Корреляционная матрица по классу государственных университетов

<img width="242" alt="image" src="https://user-images.githubusercontent.com/98012309/196932366-f824e29e-e669-4786-9092-3a26cc0bcf80.png">


Проверка на нормальность Y

<img width="394" alt="image" src="https://user-images.githubusercontent.com/98012309/196924430-7363f6e9-f029-4f16-a912-13ee19f2768a.png">

Выяснили, что он распределен не по нормальному закону, прологарифмируем и проведем анализ взаимосвязи переменных

<img width="409" alt="image" src="https://user-images.githubusercontent.com/98012309/196925033-3bb0f8f6-aad1-4693-946b-321c0cc37638.png">

Можно увидеть, что после логарифмирования взаимосвязь между переменными изменилась

А также посмотрим как изменились корреляционные матрицы

1) по классу частных университетов

<img width="372" alt="image" src="https://user-images.githubusercontent.com/98012309/196926040-acce6121-7c30-4118-8e30-2b08baf929a5.png">

2) по классу государственных университетов

<img width="372" alt="image" src="https://user-images.githubusercontent.com/98012309/196926161-120b6fce-f235-444f-8e98-8c88534e5bf3.png">


Теперь составим все возможные спецификации моделей множественной регрессии. Проведем оценку параметров моделей

Сделаем перекрёстную проверку точности моделей по одному наблюдению:

<img width="269" alt="image" src="https://user-images.githubusercontent.com/98012309/196927004-7a344371-ea53-4623-a726-0453eebbcce6.png">

Самая точная из моделей для Y:

<img width="444" alt="image" src="https://user-images.githubusercontent.com/98012309/196927291-2c3af25d-0ded-4069-a8dd-8634a71b6914.png">

Самая точная из моделей для log(Y):

<img width="401" alt="image" src="https://user-images.githubusercontent.com/98012309/196927364-820b8711-e8c9-4ebd-a549-97a3dfb870f1.png">

Перекрёстная проверка по 10 блокам

<img width="428" alt="image" src="https://user-images.githubusercontent.com/98012309/196928263-6e8d5ed1-bf69-4389-bf92-8e91832c82bd.png">

Самая точная из моделей для Y и для log(Y):

<img width="394" alt="image" src="https://user-images.githubusercontent.com/98012309/196928484-a06168fb-92b8-406c-a5bd-4ed3787f34f6.png">


Прогноз на отложенных наблюдениях

<img width="389" alt="image" src="https://user-images.githubusercontent.com/98012309/196929027-bbbd3e13-f2ec-4102-9b41-b56bea60a30e.png">

Более точная модель для прогноза

<img width="325" alt="image" src="https://user-images.githubusercontent.com/98012309/196929236-b27d80a7-0bbf-426f-b486-03cbc009c270.png">





