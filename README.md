# 🤖 Telegram quiz-bot for learning python 🤖

![image](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
![image](https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white)
![image](https://img.shields.io/badge/Docker-2CA5E0?style=for-the-badge&logo=docker&logoColor=white)

#### _My Telegram bot for python learning._

> ___Bot is available on https://t.me/Seemann_ng_bot___

----

## 💾 Installation: 💾

- __Insert Your bot token into field "BOT_TOKEN" in `credentials.py`.__

- __Run `docker engine`.__

- __Run the following commands from the project directory:__

  - __Build a docker image of the bot with:__

    ```bash
      docker image build . -t IMAGE-NAME
    ```
  
  - __Run a docker container with the bot with:__

    ```bash
      docker container run -d --restart always --name CONTAINER_NAME IMAGE-NAME
    ```

----

## 📠 Interaction with the bot: 📠

### ⌨️ _Commands:_ ⌨️

`/start` __- Start chat.__
 
`/question` __- Get a question from the bot.__
 
💡 ___Once the question is answered, bot will provide a link to the article on the topic of the question\
by appending it to the message with the quiz.___
 
__⚠️ When one of the commands above is used, if there is an unanswered question in the chat, bot will forward this question instead of sending a new one.__

`/my_score` __- Show your score.__
 
`/clear_my_score` __- Remove your score from the bot's memory.__

__⚠️ For debug purpose, there is hidden `/clear` command,️ which removes active questions sent to the User 
from the bot's memory.__

----

## 🚢 Docker commands: 🚢

### 📝 _Build an image:_

```bash
docker build . -t image_name
```

### 📦 _Build and run a new container:_

```bash
docker run -d --restart always --name container_name image_name
```

### ▶️ _Run the existing container:_

```bash
docker start container_name
```

### ⏸ _Stop the container:_

```bash
docker stop container_name
```

### 🗑  _Delete the container:_

```bash
docker rm container_name
```

___or___

```bash
docker container rm container_name
```

#### ⛔️ You have _NOT_ to delete an old _IMAGE_ when creating a new one with the same name.

#### ⚠️ You _HAVE TO DELETE_ an old _CONTAINER_ when creating a new one with the same name.

### 🛂 _List of running containers:_

```bash
docker ps
```

### 🛅 _List of all containers:_

```bash
docker ps -a
```

### 🛃 _List of all images:_

```bash
docker image ls or docker images
```
