+++
date = "2016-03-20T14:43:32+03:00"
title = "Первый прототип"
description = "Как выбрать платформу для блогов? CMS или статические генераторы?"
step = "2"
+++

Я продолжаю создание [иерархической платформы для блогов по методологии Lean](https://lis.press/lispress/1-hypothesis/).

Я хотел запустить сайт как можно быстрее и начал искать платформу среди популярных CMS, хотел просто установить красивую стандартную тему и начать писать статьи.

Но меня ждало разочарование: у Wordpress и Ghost есть стандартные шаблоны, но для того, чтобы отступить от них и сделать нехронологический блог (об этом я рассказывал на [первом шаге](https://lis.press/lispress/1-hypothesis/)), нужно разбираться либо в плагинах, либо в архитектуре платформы. Мне это показалось слишком сложным, и я сдался, отказался от CMS, выбрал генератор статических сайтов и не пожалел. Но обо всём по порядку.

## Ghost

У меня был бесплатный [студенческий набор от Github](https://edu.github.com/). Я его внимательно изучил и понял, что мне может пригодиться платформа [Bitnami](https://bitnami.com/). Она хранит предустановленные образы с популярными сервисами и позволяет быстро создать собственный сайт на их основе.

Меня очень обрадовала эта простота, я никогда до этого не имел дела с серверами и только смутно представлял, как всё устроенно на самом деле. <mark>За 3 часа</mark> мне удалось развернуть первую версию блога включая регистрацию во всех сервисах, покупку домена, SSL-сертификата и настройку сервера. Об этом я подробнее рассказал в [статье про настройку Ghost](https://lis.press/lispress/2.1-ghost/).

Но меня ждало разочарование. Оказалось, что картинка в шапке темы не сжимается, и мне нужно было либо пожертвовать качеством (а у меня MacBook Pro Retina, и я так не могу), либо скоростью загрузки на телефонах. Я не хотел идти на компромисс и заглянул в багтрекер Ghost. В нём я увидел, что с 2014 года (я делал сайт в 2016 году) висит задача на добавление responsive-картинок, по ней были обсуждения, была какая-то работа, но не похоже, что в ближайшее время её доделают. Ещё я увидел там много пул реквестов, висящих уже пару лет, и это оказалось последней каплей.

Я убедился, что ghost — всё ещё сырая платформа, но её простота и удобство меня приятно удивили. Если кто-то готов мириться с небольшими проблемами вроде несжимаемых картинок, то имеет смысл попробовать Ghost — он очень удобный и достаточно красивый.


## Wordpress

Но я не был готов с этим мириться. Я не поверил, что в мире блоггинга всё может быть так грустно, и решил перейти к самой зрелой платформе. Я сразу нашёл много плагинов, которые делают всё, что мне нужно. Но потом начались страдания. Плагины начали конфликтовать между собой, я перестал находить в админке нужные функции. Редактор для статей мне казался неудобным, комментарии и регистрация казались сырыми по сравнению с тем, что предлагают SaaS сервисы. И, в общем, я не испытывал удовольствия от использования Wordpress.

Я уж было собрался писать свой собственный движок. Но решил сделать шаг назад, умерить свою гордость и попросить совета у знающих людей. Я пошёл на Toster и [задал вопрос](https://toster.ru/q/298193), описав основные возможности, которые мне нужны для комфортного написания статей. Ответил мне WordPress Evangelist, что я просто не умею готовить WordPress, и дал мне отличные советы по его настройке.

### Второй шанс Wordpress

Я решил дать WordPress ещё один шанс. К тому времени я уже начал думать о том, какой должна быть главная страница. Поэтому я решил, что, просто создав новую тему, я смогу сделать свой блог лучше. Но подходящий шаблон среди бесплатных мне найти так и не удалось. Поэтому я пошёл на Youtube смотреть, как опытные люди создают собственные темы. Там я нашёл базовую тему ([Underscores](http://underscores.me/)) и [плейлист на ютубе](https://www.youtube.com/watch?v=Wna3T3NM9Hw&list=PL6qJ-RZM6C5TUoOt3NLkgfZS1OIks0wPN), в котором рассказывали, как сделать из неё конфетку.

Я дошёл до половины этого плейлиста, сделал первую версию дизайна безо всяких оптимизаций и плюшек и понял, что конфетки у меня не получается. Точнее, я не представлял, что конкретно нужно изменить, чтобы получился простой иерархический дизайн. _Зато я увидел, как классно можно использовать золотое сечение в веб дизайне. Можно притащить переменную фи в SASS и соблюдать пропорции золотого сечения. Время было потрачено не впустую._

## Hugo и статические генераторы сайтов

Я поговорил со своими коллегами, и они сказали, что имеет смысл найти что-то более аккуратное и что я просто плохо искал. И я решил подойти к поиску блогов с другой стороны. Я начал искать платформы, написанные на близком мне языке. И тут я натолкнулся на список [генераторов статических сайтов](https://www.staticgen.com/). 

И вдруг я понял, что абсолютно не рассматривал генераторы статических сайтов как альтернативу для создания блогов. Никакой базы, никакой админки, только Markdown, шаблоны и Html. Меня очень привлекла простота этого решения, я пробежался глазами по списку и зацепился за Hugo. Меня порадовало, что он написан на Go, и мне понравилась страница с его документацией. Я прочитал его сравнение с другими статическими генераторами. Оказалось, что основные его <mark>достоинства</mark> — простота работы и скорость, а основной <mark>недостаток</mark> — недостаточная гибкость, то есть отсутствие возможности вставлять серверный код в шаблон страницы.

Тем не менее, я выбрал Hugo и создал свой сайт на нём. Больше технических деталей можно узнать в [отдельной статье](https://lis.press/lispress/2.2-hugo/).

## Нужна ли блогам гибкость?

До этого я искал многофункциональный комбайн, который умеет делать всё, но решение разработчиков сократить гибкость сайта в Hugo мне показалось очень близким. На самом деле, оно очень современное и подталкивает к созданию микросервисной архитектуры, в которой сервисы хорошо выполняют свою работу.

Если мне нужна аналитика — я могу использовать для этого сервис для аналитики.

Если мне нужно сплит-тестирование — я могу использовать для этого сервис для сплит-тестирования. Он может интегрироваться с сервисом для аналитики.

Если мне нужны email-рассылки... Ну вы поняли логику.

Таким образом, блог может быть просто одним из сервисов в этой инфраструктуре. Тогда он может быть простым, и создателям не придётся идти на компромиссы. Я сторонник такого подхода, и я выбрал статический генератор сайтов вместо CMS.

Если вам интересно больше технических подробностей, прочитайте статью, в которой я рассказываю об установке [Ghost](https://lis.press/lispress/2.1-ghost/) и [Hugo](https://lis.press/lispress/2.2-hugo/).
Если вам интересно, зачем нужен ещё один технический блог и чем меня не устроил Хабр, прочитайте статью о том, [ради чего я делаю этот сайт](https://lis.press/lispress/1-hypothesis/).