#### systemd
это **программный пакет, который предоставляет множество системных компонентов для операционных систем Linux**. Основная цель - унифицировать конфигурацию и поведение сервиса во всех дистрибутивах Linux. Его основным компонентом является "system and service manager" – система инициализации, используемая для начальной загрузки пользовательского пространства и управления пользовательскими процессами.

Подсистема инициализации и управления службами в Linux[https://habr.com/ru/companies/slurm/articles/255845/](https://habr.com/ru/companies/slurm/articles/255845/)

Вот некоторые основные команды systemd:
1. **systemctl start name.service** — запуск сервиса.
2. **systemctl stop name.service** — остановка сервиса.
3. **systemctl restart name.service** — перезапуск сервиса.
4. **systemctl try-restart name.service** — перезапуск сервиса только, если он запущен.
5. **systemctl reload name.service** — перезагрузка конфигурации сервиса.
6. **systemctl status name.service** — проверка, запущен ли сервис с детальным выводом состояния сервиса.
7. **systemctl is-active name.service** — проверка, запущен ли сервис с простым ответом: active или inactive.
8. **systemctl list-units --type service --all** — отображение статуса всех сервисов.
9. **systemctl enable name.service** — активирует сервис (позволяет стартовать во время запуска системы).
10. **systemctl disable name.service** — деактивирует сервис.