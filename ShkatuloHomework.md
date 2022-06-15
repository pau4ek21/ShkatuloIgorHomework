# Инструкция по работe с Git


1. ___git --version___ = показывает версию приложения git
2. ___git init___ = начнет инициализацию данной **папке**. то есть начнет в ней работу
3. ___git status___ = показывает какие файлы есть и какие редактируются
4. ___git add___ = добавляет файл в работу
5. ___git commit - m “название сохранения”___ = зафиксировать изменения или сохранить текущий статус
6. ___git log___ = журнал изменений
7. ___git checkout (указать название commit целиком или первые 4 символа. БЕЗ СКОБОЧЕК) Так же переместиться между ветками дописав название ветки___
8. ___git checkout master___ = вернуться на актуальное состояние
9. ___git diff___ = показывает разницу между текущим состоянием файла и состоянием которое было сохранено
10. ___git branch___ = посмотреть в какой ветке находимся помечается “*” и посмотреть список всех веток в целом
11. ___git branch “имя новой ветки без ковычек”___ = добавление новой ветки
12. ___git branch -d “имя ветки которую хотим удалить”___ = удаление действующей ветки
13. ___git merge “ветку которую нужно добавить в ту где сейчас находишься”___ = слияние веток
14. ___создание файла .gitignore___ = сюда добавляем то что нам нужно проигнорировать. после внесения текста надо будет добавить файл в работу “git add” и закомитить “git commit - m “название сохранения””
15. ___git log —graph___ = иное отображение дерева commit ов
16. ___git clone “ссылка на проект в github”___ = создать клон проекта с гитхаб
17. ___cd название папки___ = перейти в другую папку
18. ___git clone ссылка на проект___ = позволяет сделать клон проекта с GitHub
19. ___git branch -M НазваниеГлавнойВетки___ = позволяет задать название главной ветки при создании репозитория. По стандарту главная ветка всегда называлась мастер. Но в данном случае могу назвать как хочу.
20. ___git remote add origin [https://github.com/pau4ek21/Lesson3.git](https://github.com/pau4ek21/Lesson3.git)___ = указывается ссылка на новый репозиторий. что бы их связать.
21. ___git push -u origin название ветки___  = направить репозиторий в интернет. (после сохранения изменений, если я хочу направить в интернет, то надо всегда вводить данную команду. После каждых изменений.)
22. ___git push___ = подгружает данные с локального репозитория в удаленный на GitHub
23. ___git pull___  = для того что бы подгрузить изменения с удаленного репозитория на локальный (так же данная команда производит слияние веток)

---

# Информация с прошлых занятий с Git

# 1. Добавление заголовков, жирного текста и пропусков.

С помощью знака "# " можно добавить большой заголовок

## А если сделать "## " то заголовок будет меньше и т.д.

**Что бы добавить жирный текст надо предложение обрамить ** ** с каждой стороны**

*Что бы текст сделать курсивом надо обрамить его по краям с каждой стороны символом* **. А если нужно добавить новый абзац то необходимо просто пропустить строку нажав кнопку Enter 

и все получится)

---

## 2. Добавляем нумерованные списки и списки

Нумерованные списки создаются с помощью "1. " (цифра, точка и пробел):
1. вот первый нумерованный список
2. второй нумерованный список 
3. и так далее...

Добавление списков производится с помощью "* ". Выглядит это следующим образом: 
* вот первый элемент списка
* второй элемент списка
* третий и так далее...

### 2.1 Добавили информацию про списки

По стандарту списки будут идти от 1 и дальше.

Например:
1. первый
4. четвертый
10. десятый

Но видим мы что они идут по порядку как 1. 2. 3.

Число перед первым пунктом показывает с чего нужно начинать нумеровать элементы списка, поэтому если в Markdown поставить 99., 1., 2., то в итоговой разметки пункты будут стоять под номерами 99, 100, 101.

Например: 

99. 99 и видим.
1. а дальше идет 100 хотя поставили цифру 1.
1. еще раз 1
1. еще раз 1
1. пункты увеличиваются в значении вне зависимости от того какую цифру ставить
    1. а подпункт идет с цифры 1.
    22. если бы я поставил цифру не 1 в начале а например 11. то подпункт бы не активировался.
    50000. подпункты можно добавлять через (Tab)

1. а дальше ппойдет все так же по списку как 104 пункт.

Тут ввели какой то текст и снова попытаемя сделать пункт.

500. а вот и пункт
1. получилось! 
502. То есть нумерация после очередного обычного текста начинается заного.



---

## 3. Добавим зачеркнутый текст
Что бы добавить зачеркнутый текст надо обрамить с каждоый стороны текст двойным символом ~~ - тильда и должно получиться:

~~тут был нормальный текст но его кто то зачеркнул.~~ ~~редиска~~

---

## 4. Пробуем добавить картинку
![beautiful fox](https://oir.mobi/uploads/posts/2021-04/1619640716_44-oir_mobi-p-krasivaya-lisa-zhivotnie-krasivo-foto-47.jpg)

*Что бы добавить картинку надо использовать команду "!", сразу ставим квадратные скобки, где в квадратных скобках <[альтернативнй текст]> указывается альтернативный текст а дпльше сразу ставим круглые скобки. <(где указывается ссылка на картинку)>.*

---

## 5. Пробуем добавить цитату

> Через 20 лет вы будете больше разочарованы теми вещами,
>, которые вы не делали, чем теми, которые вы сделали.
> Так отчальте от тихой пристани. Почувствуйте попутный ветер в вашем парусе.
>Двигайтесь вперед, действуйте, открывайте!
>
>*-Марк Твен*

Цитата добавляется с помощью символа ">", таких символов можно поставить сколько угодно в кадой новой строке, но текст будет идти все ровно в 1 строчку. Так же можно поставить пропуск если после символа > снова нажать Enter.

---

## 6. Пробуем добавить ссылку

Привет, [GeekBrains](https://gb.ru/ "Платформа для старта в сфере IT")!

При добавлении ссылки сначала например пишем текст, потом когда решили в определенное слово вставить ссылку то это слово берем в <[квадратные скобки]> дальше открываем круглые скобки <(вставляем сразу ссылку на тот ресурс куда хотите и через пробел открываем ковычки "сюда пишем текст который будет высвечиваться как только наводим мышку на этот текст")>, ну и в конце например можем дописать что то еще уже вне ссылки или же поставить точку и закончить предложение.

---

## 7. Горизонтальный разделитель

Такой разделитель ставиться с помощью "---" в пустой строке, и так же что бы сверху от разделителя и снизу от него строки были пустые иначе он просто выделит текст как заголовок.

---

## Параграф
Подряд идущие строчки будут склеены в одну, если не добавить жёсткий перенос. Существует несколько способов, как это можно сделать:

добавить два (или больше) пробелов в конце строки <пробел><пробел>;
добавить обратную косую черту в конце строки \;
добавить HTML-тег переноса строки <(br)> - без скобочек внутри.

Например:
1. Привет,  
мир! (тут мы добавили 2 пробела после "привет,") и строка была перенесена.

2. Добавляется обратную косую черту\
в конце строки.

3. Добавляем br <br>
и строка снова перенесена, ура!
 
---

## Таблицы

Что бы добавить таблицу нужно использовать элемент (|) и обрамить им каждое слово которое необходимо вывести в таблицу после чего нажать кнопку __Enter__ и снова добавить (|). А еще добавить разделитель (---------) между (|). тогда получиться следующее:  


|участники |очки       |место|
|----------|-----------|-----|
|Котики    |     123   | 1   |
|Черепашки |     121   |   2 |
|Уточки    |     107   |3    |


Так же можно сделать так, что бы в таблице слова были оцентрованы по середине с помощью (:). Данный знак "двоеточие" нужно добавлять внутри таблицы примерно вот так: (|:----:|:----:|). Тогда должно получиться следующее:


|участники  |очки         |место  |
|:---------:|:-----------:|:-----:|
|Котики     |     123     |1      |
|Черепашки  |     121     |2      |
|Уточки     |     107     |3      |

---

## Список задач

Для создания списка задач используется синтаксис маркированного списка, но с добавлением чекбоксов ([ ] или [x]) после маркеров.

Например:  
- [x] Выйти на улицу
- [x] Зайти в магазин
- [ ] Купить продукты
  - [x] Молоко
      - [x] Хлеб
          - [ ] Помидоры
- [ ] Вернуться домой

Так же можно делать отступы через Табуляцию (Tab) и сноски будут меняться. 

---

## Спойлер

Если после символа цитирования поставить восклицательный знак (>!), то цитата выведется свёрнутой, и развернуть её пользователь сможет, кликнув по ней.

Например:  
Тут идет обычный текст
>! тут он должен быть свернутый, но что то пошло не так...
Видимо это идет с каким то расширением и строка сворачивается. Но у меня не вышло.

---


## Заключение

Могу добавить что пользовался ресурсом [Дока](https://doka.guide/tools/markdown/#kratko "Изучение языка Markdown")!