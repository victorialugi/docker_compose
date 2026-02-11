# Домашнее задание к занятию "`Оркестрация группой Docker контейнеров на примере Docker Compose.`" - `Лугинина Виктория`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!
   
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

### Задание 1

(https://hub.docker.com/repository/docker/victorialugi/custom-nginx/general)


---

### Задание 2

![task_2.png](https://github.com/victorialugi/docker_compose/blob/main/task_2.png)
![task_2.1.png](https://github.com/victorialugi/docker_compose/blob/main/task_2.1.png)

---

### Задание 3

`3. Контейнер остановился, потому что я нажала Ctrl+C в режиме docker attach.
Это отправило сигнал SIGINT в основной процесс контейнера nginx, и он завершился.
По умолчанию nginx не настроен на graceful shutdown при SIGINT, поэтому контейнер вышел с кодом ошибки (Exited).`

![task_3.png](https://github.com/victorialugi/docker_compose/blob/main/task_3.png)

`10. Снаружи на хосте я стучусь на 127.0.0.1:8080 и Docker перенаправляет трафик внутрь контейнера на порт 80.
Но внутри контейнера nginx больше не слушает 80, ведь он слушает 81.
Поэтому соединение обрывается.
Изменения конфига nginx не влияют на настройки Docker-порта.`

![task_3.1.png](https://github.com/victorialugi/docker_compose/blob/main/task_3.1.png)

### Задание 4

![task_4.png](https://github.com/victorialugi/docker_compose/blob/main/task_4.png)
![task_4.1.png](https://github.com/victorialugi/docker_compose/blob/main/task_4.1.png)

### Задание 5

`Docker Compose запустил файл compose.yaml, потому что при наличии нескольких файлов с поддерживаемыми именами (compose.yaml и docker-compose.yaml) приоритет отдаётся файлу compose.yaml (без префикса "docker-").`

![task_5.1.png](https://github.com/victorialugi/docker_compose/blob/main/task_5.1.png)
![task_5.2.png](https://github.com/victorialugi/docker_compose/blob/main/task_5.2.png)
![task_5.3.png](https://github.com/victorialugi/docker_compose/blob/main/task_5.3.png)
![task_5.4.png](https://github.com/victorialugi/docker_compose/blob/main/task_5.4.png)
![task_5.5.png](https://github.com/victorialugi/docker_compose/blob/main/task_5.5.png)
![task_5.6.png](https://github.com/victorialugi/docker_compose/blob/main/task_5.6.png)

`все контейнеры удалены одной командой docker compose down осталсся только контейнер задеплоенный через Portainer`

![task_5.7.png](https://github.com/victorialugi/docker_compose/blob/main/task_5.7.png)
