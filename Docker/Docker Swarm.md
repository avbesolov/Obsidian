Docker Swarm — **это оркестратор от компании Docker, который позволяет объединять несколько Docker-хостов в единый кластер и автоматически управлять запуском и масштабированием контейнеров.**

С помощью данного инструмента компания может с лёгкостью развёртывать требуемые службы, управлять ими, масштабировать в процессе развития и мониторить стабильность и производительность.

В Docker Swarm есть 2 основных типа узлов:

1. **Управляющие узлы (Managers)**. Они отвечают за принятие решений и координацию действий в кластере.
    
2. **Рабочие узлы (Workers)**. Выполняют задачи, сформированные управляющими узлами.

### Установка Docker Swarm
```
curl -ssl https://get.docker.com | bash
```

_**Прим. перев.**: в Docker версий 1.12.0+ ничего дополнительно устанавливать не требуется, т.к. Docker Swarm встроен в Docker Engine в виде специального режима (Swarm mode)._  

### Инициализация Swarm
```
docker swarm init --advertise-addr 192.168.10.1
```


### Подключение рабочего узла (worker) к Swarm
```
docker swarm join-token worker
```

  
### Подключение управляющего узла (manager) к Swarm
```
docker swarm join-token manager
```

  
### Список сервисов
```
docker service ls
```

  
### Список узлов
```
docker node ls
```

  
### Создание сервиса
```
docker service create --name vote -p 8080:80 instavote/vote
```

  
### Список заданий Swarm
```
docker service ps
```

  
### Масштабирование сервиса
```
docker service scale vote=3
```

  
### Обновление сервиса
```
docker service update --image instavote/vote:movies vote
```


```
docker service update --force --update-parallelism 1 --update-delay 30s nginx
```


```
docker service update --update-parallelism 5--update-delay 2s --image instavote/vote:indent vote
```


```
docker service update --limit-cpu 2 nginx
```

  
```
docker service update --replicas=5 nginx
```

Оригинал. статья - https://github.com/eon01/DockerCheatSheet