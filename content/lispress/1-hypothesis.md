+++
date = "2016-03-13T10:45:44+03:00"
title = "Гипотезы"
description = "Для чего нужна ещё одна платформа для блогов?"
step = "1"

+++

Я программист. В свободное время я создаю небольшие проекты, чтобы изучать что-то новое. Недавно я принял участие в [проекте Codex](https://ifmo.su). Мы создали собственную платформу для блогов и наполнили её статьями.

В самом начале я не понимал, зачем нужна ещё одна платформа для хранения статей, почему мы не используем для этого [хабр](http://habrahabr.ru) или другие профильные ресурсы. Этот вопрос не давал мне покоя. И я захотел найти способ сделать блог чем-то более удобным, чем просто список статей.

В этом проекте я занимался развитием эффективности [жизненного цикла разработки](https://ifmo.su/article/18). Меня вдохновила возможность писать о граблях и удачных решениях _после каждой задачи_. И я пришёл к выводу, что написание статьи должно стать частью жизненного цикла задачи. Это позволило по-другому взглянуть на статьи. Если мы пишем о том, как мы чему-то научились, то кто угодно, прочитав наши статьи сможет создать похожий проект и даже сделать его лучше. И **блог может помочь в этом читателям**.

Но обычная линейная структура блога [для этого не подходит](https://ifmo.su/article/21). В этом проекте я буду создавать иерархическую структуру блога, то есть разные статьи будут публиковаться в разных разделах, а одинаковые — объединяться в одну большую историю. 

В этом эксперименте я буду учиться <mark>business-aware разработке</mark> и пользоваться методологией <mark>Lean Startup</mark>. Постараюсь показать её во всей красе и делать только то, что реально может понадобиться пользователям.

## Теория

Lean Startup — это методология бережливого создания продукта. Она очень похожа на методологии гибкой разработки (XP, agile и тому подобное), только учитывает ещё и аспекты бизнеса и потребности клиентов. То есть, задача заканчивается не в тот момент, когда написан код и даже не в тот момент, когда он оттестирован и работает в production. Она заканчивается только после того, как доказана её необходимость и полезность.

Доказать или опровергнуть полезность задачи необходимо как можно быстрее, исходя из этого должен разрабатываться продукт. И если в него добавляется только функционал необходимый для быстрой проверки гипотез, такой продукт называется <mark>MVP</mark> (Minimal Viable Product).

Быстрая проверка гипотез роста и ценности — приоритетная задача для продукта во время его первого контакта с миром. Гипотезы важнее, чем планы или дальнейшая разработка, поэтому этот эксперимент я начинаю именно с них.

<!-- TODO было бы прикольно сделать эту штуку плашкой. -->
## Гипотезы

<mark>Гипотеза ценности</mark> — я думаю, что программистам будет интересно читать об идеях, граблях и успехах на пути к их реализации в рамках большого проекта в реальном времени.

<mark>Гипотеза роста</mark> — я думаю, что программисты готовы репостить сообщения в твиттере и делиться информацией об этом проекте.


## Как я узнаю, что гипотезы сработали?

То, что пользователю <mark>интересно читать</mark>, можно определить, зная, сколько страниц он просмотрел на сайте. Если пользователь попал на сайт впервые, скорее всего, он ничего не знает о проекте и попал на описание конкретного этапа разработки. В конце статьи, описывающей этот этап, должна быть ссылка на следующий этап (если он существует) и на дорожную карту (описание общего видения проекта). У заинтересованного пользователя должна быть возможность быстро переходить между этапами разработки и читать то, что им интересно.

Эта часть гипотезы будет подтверждена, если 50% новых пользователей будут просматривать на сайте три статьи или более.

То, что пользователю интересно <mark>следить за блогом</mark> в реальном времени, можно узнать по количеству возвратов пользователей. Вряд ли пользователи будут возвращаться на сайт по ссылке ради того, чтобы читать о новом эксперименте раз в неделю, поэтому имеет смысл выбрать другой канал возврата пользователей. Наиболее логичным для этого кажется электронная почта, RSS и Twitter.

Наиболее сложным для моего понимания является гипотеза роста. Чтобы пользователи делились информацией об экспериментах, нужны либо громкие заявления, либо хорошие вопросы. Этот пункт мне кажется наиболее интересным и наименее ясным. Но я готов принять этот вызов и обязательно расскажу вам о результатах =)

В [следующей статье](https://lis.press/lispress/2-blog-engine/) я расскажу о создании первой версии сайта.

## Источники вдохновения и идей
- Бизнес с нуля, Эрик Рис, [Альпина Паблишер](http://www.alpinabook.ru/), 2015;
- [Почему блог вредит статьям?](https://ifmo.su/article/21);
- [Жизненный цикл задач Codex](https://ifmo.su/article/18);
- [Советы начинающему блогеру](http://lifehacker.ru/2016/03/01/sovety-blogeru/);
- [Советы Дизайн-бюро Артёма Горбунова](http://artgorbunov.ru/bb/soviet/);
- Процесс разработки в [студии Артемия Лебедева](http://www.artlebedev.ru/) ([пример](http://www.artlebedev.ru/everything/type/alumna/process/)) и в [Дизайн-бюро Артёма Горбунова](http://artgorbunov.ru/) ([пример](http://artgorbunov.ru/projects/sensum-wayfinding/recycled/)).