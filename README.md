# ci_test_env
ci_test_env



Приветствую

https://github.com/futureisrise/ci_test_env 


Тут находиться ядро и полный пример класса 
И собственно site.com/tests/get_last_news 

Чтобы запустить над залить бы дамп Mysql и прописать конфиг, 
и может какие то мелочи могут не работать ( починю после фидбека что сломано) 
Возможно путь к папкам ( system , application ) не верный, его надо поправить 

public/index.php : Изменить

application folder path
system folder path



-----------------------------------------------------------------------------------------

Техническое задание (backend)
Задание должно быть выполнено с использованием: (PHP 7.0 MySQL)

Приветствуется:
Vue.js

-----------------------------------------------------------------------------------------

Новости:

Главная страница : 
Вывести 3 последние новости, либо закрепленные новости, не больше трех. (картинка, заголовок, дата публикации, сокращенный текст новости до 300 символов)

ОСНОВНАЯ ЗАДАЧА:
!!Реализовать!!: Лайки, Комментарии;

Страница одной новости: 

Блок с данной новостью (картинка, заголовок, дата публикации, текст новости)

Статистика данной новости (количество просмотров, лайков, комментариев)

Блок с комментариями (текст комментария, лайки комментария)

Блок с популярными новостями (больше всего лайков и просмотров) (2-3 новости)




Функционал страницы с новостью:

Поставить лайк (первый раз ставит, второй раз отменяет)

Написать комментарий

Лайкнуть комментарий (первый раз ставит, второй раз отменяет)

===== Дополнительная задача( будет большим плюсом ) ======

Архив новостей: 

Все новости подряд, с маленькой картинкой, сокращенным описанием и ссылкой на новость. 

Админка:
Список всех новостей (со ссылками на редактирование и новость на сайте)

Страница редактирования новости (текст, заголовок, картинка)

Страница создания новости (текст, заголовок, картинка)

===== Дополнительная задача( будет большим плюсом ) ======

Оформление всех страниц может быть произвольным (только для визуализации результата).

Можно создавать view файлы и через контроллер выводить данные с минимальной версткой, или же как JSON API ответ 

Приветствуется грамотное построение связей таблиц базы данных, полное использование ООП и правильное построение зависимостей между классами.



Пример использования который может быть реализован:
$comment = News_comments_model::create((int)$this->input->post('news_id'),clear_str($this->input->post('comment')), User::get_user_id());


