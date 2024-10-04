kubectl exec -ti <pod-name> -- ls -ld /opt/naumen/nauphone/log - проверка директории
kubectl exec -ti <pod-name> -- whoami - проверка пользователя внутри контейнера
kubectl exec -ti <pod-name> -- touch /opt/naumen/nauphone/log/test.log - создать файл внутри контейнера в данной директории, чтобы проверить права на запись
kubectl get pod <pod-name> -o jsonpath='{.spec.containers[*].name}' - проверка всех контейнеров в поде
kubectl exec -ti <pod-name> -c <имя_вашего_контейнера> -- whoami - просмотр пользователя в конкретном контейнере
kubectl describe pod <pod-name> - получение подробной информации о поде
kubectl logs <pod-name> -c <имя_вашего_контейнера> - логи контейнера
kubectl logs <pod-name> -c <имя_контейнера> --previous - получение логов предыдущей попытки запуска

