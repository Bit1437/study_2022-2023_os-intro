**Лабораторная работа №2 Первоначальна настройка git**

**Дисциплина Операционные системы**

Агарков Артём Сергеевич НПМбв-02-20" 
# Содержание" 
[Цель работы	1](#_toc162206555)

[Выполнение лабораторной работы	1](#_toc162206556)

[Настройка GIT	1](#_toc162206557)

[Создание рабочего пространства	5](#_toc162206558)

[Ответы на контрольные вопросы	6](#_toc162206559)

[Выводы	7](#_toc162206560)


# <a name="_toc162206555"></a><a name="цель-работы"></a>**Цель работы**
- Изучить применение средств контроля версий
- Освоить умения по работе с git'ом
# <a name="_toc162206556"></a><a name="выполнение-лабораторной-работы"></a>**Выполнение лабораторной работы**
## <a name="_toc162206557"></a><a name="настройка-git"></a>**Настройка GIT**
` `Сконфигурируем git и создадим SSH ключ

![](image/1.jpg)


` `Создадим PGP ключ

![](image/2.jpg)

С помощью команды gpg --armor --export <PGP Fingerprint> | xclip -sel clip скопируем PGP ключ.
И вставим в наш Github.

![](image/3.jpg)

Авторизируемся в Github с помощью комманды gh

## ![](image/4.jpg)
## <a name="_toc162206558"></a><a name="создание-рабочего-пространства"></a>**Создание рабочего пространства**


Склонируем репозиторий на локальную машину

![](image/5.jpg)
# <a name="_toc162206559"></a><a name="ответы-на-контрольные-вопросы"></a>**Ответы на контрольные вопросы**
#### <a name="x15d61d65c9e0e0d8d91a0789cab38cc43248442"></a>*Что такое системы контроля версий (VCS) и для решения каких задач они предназначаются?*
Системы контроля версий (VCS) предназначены для отслеживания изменений в программном коде и обеспечения коллективной разработки.
#### <a name="x95381528190b4689c5266eabfeb9026ffb037cc"></a>*Объясните следующие понятия VCS и их отношения: хранилище, commit, история, рабочая копия.*
Хранилище: Место, где хранятся все изменения и версии программного кода. 
Commit: Отдельное изменение или набор изменений в коде, зафиксированное в системе контроля версий. 
История: Последовательность коммитов, отображающая эволюцию кода. 
Рабочая копия: Локальная копия проекта, с которой работает разработчик.
#### <a name="xf8d2f18c16053925da22f10ffdf7b4f677e8615"></a>*Что представляют собой и чем отличаются централизованные и децентрализованные VCS? Приведите примеры VCS каждого вида.*
Децентрализованные VCS копируют всю историю изменений на каждый клиентский компьютер, в то время как централизованные VCS хранят все изменения на центральном сервере и клиенты получают только последние версии файлов. Примеры децентрализованных VCS: Git, Mercurial. Примеры централизованных VCS: Subversion, CVS.
#### <a name="x388b2fb17fbb83b15215a92f6fd692db711f2a1"></a>*Опишите действия с VCS при единоличной работе с хранилищем.*
При индивидуальной разработке пользователь клонирует проект на свой компьютер, вносит изменения и создает новые версии, коммитя их в системе контроля версий.
#### <a name="x9bfc7483828e01649bf89d262be16ae6a317b15"></a>*Опишите порядок работы с общим хранилищем VCS.*
Пользователь получает версию проекта из центрального хранилища, вносит изменения, коммитит их и отправляет обратно в хранилище.
#### <a name="x81e4f652505245c972fa3b3173659b213ddf161"></a>*Каковы основные задачи, решаемые инструментальным средством git?*
Git используется для разработки проектов в команде, контроля изменений в файлах и возможности сохранения нескольких состояний проекта.
#### <a name="xa039e66fdcc06b6c2d6a71bb77786172b98cb64"></a>*Назовите и дайте краткую характеристику командам git.*
git add - добавляет изменения для коммита.

git commit - сохраняет изменения в репозитории с названием.

git push - отправляет изменения на удаленный репозиторий.

git config - позволяет изменить настройки Git.
#### <a name="x0139e8a7aca32e0d83428cb741f7eb222e743c1"></a>*Приведите примеры использования при работе с локальным и удалённым репозиториями.*
В локальном репозитории разработчик может вносить изменения в код и коммитить их без доступа к сети. В удаленном репозитории команда разработчиков может совместно работать над проектом, обмениваясь изменениями через централизованный сервер.
#### <a name="x4a1eff98c561be46acfb21646ce811931cc2a99"></a>*Что такое и зачем могут быть нужны ветви (branches)?*
Ветви используются для параллельной разработки функций или исправлений, чтобы избежать конфликтов между изменениями и обеспечить безопасное тестирование нового кода.
#### <a name="xb8b3d4801c334334c57aa29fad1b59b687ed541"></a>*Как и зачем можно игнорировать некоторые файлы при commit?*
Файлы могут быть проигнорированы с помощью файла .gitignore, чтобы избежать загрязнения репозитория лишними или конфиденциальными файлами.
# <a name="_toc162206560"></a><a name="выводы"></a>**Выводы**
Мы изучили идеологию применения средств контроля версий и освоили базовые комманды git'а. 

