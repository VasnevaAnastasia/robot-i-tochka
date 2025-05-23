# Описание эндпоинтов

### 1. Аутентификация и регистрация пользователя
| **Endpoint**                  | **Описание**                        |
| :---------------------------- | :---------------------------------- |
| **`POST`** /users/send-code   | Отправка кода подтверждения         |
| **`POST`** /users/verify-code | Подтверждение кода                  |
| **`POST`** /users             | Создание нового пользователя        |
| **`POST`** /users/login       | Авторизация пользователя            |
| **`GET`** /users/{userId}     | Получение информации о пользователе |
| **`PATCH`** /users/{userId}   | Редактирование профиля              |

### 2. Работа с меню и блюдами
| **Endpoint**                        | **Описание**                    |
| :---------------------------------- | :------------------------------ |
| **`GET`** /categories               | Получение списка категорий меню |
| **`GET`** /dishes                   | Получение списка блюд           |
| **`GET`** /dishes/{dishId}          | Получение данных о блюде        |
| **`POST`** /dishes/{dishId}/reviews | Добавление отзыва о блюде       |

### 3. Работа с корзиной
| **Endpoint**                     | **Описание**                   |
| :------------------------------- | :----------------------------- |
| **`POST`** /cart/items           | Добавление блюда в корзину     |
| **`GET`** /cart/items            | Просмотр корзины               |
| **`PATCH`** /cart/items/{itemId} | Редактирование блюда в корзине |

### 4. Оформление и доставка заказа
| **Endpoint**                   | **Описание**        |
| :----------------------------- | :------------------ |
| **`POST`** /orders             | Оформление заказа   |
| **`POST`** /delivery-addresses | Оформление доставки |

### 5. Оплата
| **Endpoint**                          | **Описание**            |
| :------------------------------------ | :---------------------- |
| **`POST`** /orders/payment            | Оплата заказа картой    |
| **`POST`** /orders/{orderId}/pay-cash | Оплата заказа наличными |

### 6. Заказы и статус
| **Endpoint**                       | **Описание**              |
| :--------------------------------- | :------------------------ |
| **`GET`** /orders                  | Просмотр истории заказов  |
| **`GET`** /orders/{orderId}        | Получение данных о заказе |
| **`GET`** /orders/{orderId}/status | Получение статуса заказа  |
| **`PATCH`** /orders/{orderId}      | Отмена заказа             |

