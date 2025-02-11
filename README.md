gRPC Client – Greetings Service 🚀
This repository contains an implementation of a gRPC client that communicates with the Greetings Service. The client connects to the gRPC server, sends a username, and receives a greeting message.

🔹 Technologies:
Java 17
gRPC
Protocol Buffers
Maven
🚀 Features:
✅ Establishes a connection with the gRPC server
✅ Sends a username as a request
✅ Receives a greeting response
✅ Closes the connection after processing the request

🛠 How to Run:
1. Build the project: mvn clean package


2. Run the client: java -jar target/grpc-client.jar


📌 Example Output:
After running, the client sends a request with the name "Neil" and receives a response from the server: message: "Hello from server, Neil!"

🛠 How to Modify the Request?
You can change the username in Client.java:

GreetingServiceOuterClass.HelloRequest request = GreetingServiceOuterClass.HelloRequest
        .newBuilder().setName("Dmitriy").build();
        
Now, the client will send "Hello, Dmitriy!" instead of "Hello, Neil!".

That's it! The client is now ready to send gRPC requests to the server. 🚀
==========================================================================
gRPC Client – Greetings Service 🚀
Этот репозиторий содержит реализацию gRPC-клиента, который взаимодействует с Greetings Service. Клиент подключается к gRPC-серверу, отправляет имя пользователя и получает приветственное сообщение.

🔹 Технологии:
Java 17
gRPC
Protocol Buffers
Maven
🚀 Функционал:
✅ Устанавливает соединение с gRPC-сервером
✅ Отправляет имя пользователя в виде запроса
✅ Получает ответ с приветствием
✅ Закрывает соединение после обработки запроса

🛠 Запуск:
1. Сборка проекта: mvn clean package

2. Запуск клиента: java -jar target/grpc-client.jar

📌 Пример работы:
После запуска клиент отправляет запрос с именем "Neil" и получает ответ от сервера: message: "Hello from server, Neil!"

🛠 Как изменить запрос?
В файле Client.java можно изменить имя пользователя:

GreetingServiceOuterClass.HelloRequest request = GreetingServiceOuterClass.HelloRequest
        .newBuilder().setName("Dmitriy").build();
После этого клиент отправит "Hello, Dmitriy!" вместо "Hello, Neil!".

Готово! Теперь клиент может отправлять gRPC-запросы к серверу. 🚀

