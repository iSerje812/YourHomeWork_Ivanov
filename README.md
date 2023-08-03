# YourHomeWork

## Друзья, всем добрый день! 
Общий план работы:
1. Делаем fork репозитория;
2. Клонируем репозиторий и открываем в VSCode;
3. Создаем побочную ветку;
4. В побочной ветке создаем отдельный файл с конспектом по 3 семинару.
5. Делаем push вашей ветки;
6. Оформляем pull request и делаем скрин;
7. Profit!

# 28.07.23 Конспект семинара3. Введение в контроль версий -> Работа с удалёнными репозиториями

## Создание удаленного репозитория

### На сайте github.com создается новый удаленный репо
{Publik - всегда. Иначе никто не смождет получить доступ к нашему репо, даже при наличии ссылки. (В дальнейшем возможно потребуются закрытые репо. Статус можно менять в последствии)}

И далее 2 варианта:
* Создание нового локал репо и дальнейшая его привязка к github*
* Подключение существующего локального акка к удаленному репо

Эти пункты выполняются уже на локал компе в локальном репозитории, через VScode.
(Команды копируются из GitHub в Git).
#### команда git branch -M branchname:
* M - большая. - Создание и присвоение статуса "основной" ветки, ветки с названием "branchname"*
#### команда remote and origin <ссылка>
* remote - "подвязать" удаленный репо
* origin - оригинальная ветка удаленного репо, всегда при работе с удаленным репо
* ссылка - состоит из github/имя пользователя/название удаленного репозитория .git
#### команда git push -u origin <branchname>
* git push - отправка текущего состояния локал репо в удаленный репо
* -u - только впервый раз. Доп команда к git push - upstrim - дать разрешение отправки в удаленный репо изменений сделанных в локо репо и наоборот. 
* origin - оригинальная ветка удаленного репо, всегда при работе с удаленным репо
* branchname - название ветки в удаленном репо, которое должно совпадать с оригинальнорй веткой локального репо на локал компе.

### Работа в команде. Создание копии удаленного репо.

#### *Github* gпредоставляет возможность совместной работы над проектами и дальнейшее предоставление своей актуальной версии "руководителю проекта"

#### Имея ссылку на ПУБЛИЧНЫЙ удаленный репозиторий, мы можем сделать его копию. 
Кнопка *FORK* - создание копии удаленного репо другого пользователя, в своем акке, работа с этой копией(создание альтернативной версии) и возможность предложить свою версию путем запроса на слияния - *pull request*

* Рекомендуется оставить галочку Cope the master branch only. Это создает копию только ветки master те той ветки, которая уже утверждена(bild которой был подтвержден);
* В версии Fork, есть отсылка к оригинальной версии, которая была скопирована;

#####  Командой git clone или удобной функцией в VScode делаем копию удаленного репо у себя в локальном репо

* далее при работе в локальной версии рекомендуется сразу создать и работать в отдельной ветке. И уже она подгружается на github, после проделанной работы;
* git push - с выдачей ошибки, где git нам подсказывае, что такой ветки на githube еще нет и предлагает команду для ее создания и отправки
* после этого в github появляется уже 2 ветки, как и в локал репо. И возможность отправить запрос на слияние. Отправлять запрос непосредственно из побочной ветки, в которой мы проделали работу.

