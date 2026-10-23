---
publish: true
title: Черепашка. Урок 1. Конспект
description: Черепашка. Урок 1. Конспект
created: 2026-10-23
modified: 2026-10-23
tags:
  - 9класс
  - уроки
  - школа
  - черепашка
  - turtle
---

<h3>Шаг 1</h3>
<p>Откройте редактор Python на компьютере - например, программу PyCharm.
  Создайте при необходимости новый проект и отдельный файл с расширением .py
  внутри него. Теперь в этом файле мы будем писать код.</p>
<h3>Шаг 2</h3>
<p>Сначала мы скопируем в наш пустой файл несколько строчек кода:</p>
<pre class="language-python"><code>import turtle
turtle.shape('turtle')
turtle.color('brown', 'lime')
# в этой строке и далее будет Ваш код

turtle.mainloop()</code></pre>

<p>Теперь обсудим каждую строчку. Запишите в тетрадь каждую команду и пояснение
  к ней:</p>
<pre class="language-python"><code>import turtle</code></pre>
<p>импортировать в программу модуль с командами для черепашки. Модуль
  называется <strong>turtle</strong> (англ. черепаха).</p>
<pre class="language-python"><code>turtle.shape('turtle')</code></pre>
<p>задать черепахе форму (в данном случае форму "черепахи", но можно и другие:
  <em>'arrow'</em> - стрелочка, <em>'square'</em> - квадрат, <em>'circle'</em> -
  кружок).</p>
<pre class="language-python"><code>turtle.color('brown', 'lime')</code></pre>
<p>задать черепашке цвет линии и цвет заливки.</p>
<pre class="language-python"><code>turtle.mainloop()</code></pre>
<p>запустить бесконечный цикл, который оставит окно с черепашкой на экране, пока
  его не закроют. Все наши команды должны быть написаны ДО вот этой последней.
</p>
<p>Если запустить программу, то на экране появится черепашка, которая пока что
  никуда не двигается:</p>
<p><img class="img-fluid" role="presentation"
    src="https://edu-admin.skolca.ru/draftfile.php/11572/user/draft/516105166/image.png?1764703388037"
    alt="" width="500" height="349"></p>
<h3>Шаг 3</h3>
<p>Теперь нам надо, чтобы черепаха пошла вперед. Для этого есть команда forward,
  и в скобках мы можем указать количество шагов.
  Например <strong>forward(100)</strong>.<br>Написать команду надо через точку -
  так же, как и предыдущие команды, которыми мы задавали черепашке цвет и
  форму.<br>Обратите внимание, что команду мы пишем ДО бесконечного цикла
  mainloop - иначе черепашка никуда не побежит:</p>
<pre class="language-python"><code># в этой строке и далее будет Ваш код
turtle.forward(100)</code></pre>
<p>Запустите программу. Ура, ваша черепашка прошла вперед!<br>Почему она пошла
  именно туда? С чем это перекликается из математики?</p>
<p><img class="img-fluid" role="presentation"
    src="https://edu-admin.skolca.ru/draftfile.php/11572/user/draft/516105166/image%20%281%29.png?1764703845058"
    alt="" width="500" height="186"></p>
<h3>Шаг 4</h3>
<p>Можно заметить, что черепаха двинулась горизонтально вправо, т.е., если
  вспомнить математику, по оси X в положительную сторону. При этом стартовая
  точка совпадает с началом координат - <strong>(0, 0)</strong>.<br>Черепаха
  умеет ходить только вперед - <strong>forward()</strong> или назад
  - <strong>backward()</strong>. Причем шаги в скобках можно указать как
  положительные, так и отрицательные.
  Т.е. <strong>forward(-50)</strong> и <strong>backward(50)</strong> - это одно
  и то же (проверьте!)<br>Обратите внимание, что черепаха оставляет за собой
  след. Этот след она рисует пером. Перо можно поднять -
  <strong>penup()</strong> и опустить - <strong>pendown()</strong>. Не забывайте
  ставить скобки - без них черепашка не поймет, что это за
  команды!<br><br>Попробуем написать последовательно несколько команд:</p>
<pre class="language-python"><code>turtle.forward(100)
turtle.penup()
turtle.forward(100)
turtle.pendown()
turtle.forward(100)</code></pre>
<p>Каждая команда должна быть написана на отдельной строчке. <strong>Конец
    строки - признак того, что команда закончена</strong>.</p>
<p>Должно получиться вот так:</p>
<p><img class="img-fluid" role="presentation"
    src="https://edu-admin.skolca.ru/draftfile.php/11572/user/draft/516105166/image%20%282%29.png?1764704467024"
    alt="" width="500" height="128"></p>
<h3>Шаг 5</h3>
<p>Чтобы черепашка пошла вниз или вверх, ей надо повернуться. Для этого ей можно
  дать команду <strong>right()</strong> или <strong>left()</strong>. В скобках
  надо указать количество градусов, на которые надо повернуться.<br><br>Давайте
  изменим нашу программу, и вместо<strong> t.penup()</strong> повернем черепашку
  направо, а вместо <strong>t.pendown()</strong> - налево:</p>
<pre class="language-python"><code>turtle.forward(100)
turtle.right(90)
turtle.forward(100)
turtle.left(90)
turtle.forward(100)</code></pre>
<p>Выполнив нашу программу, черепашка должна нарисовать ступеньку:</p>
<p><img class="img-fluid" role="presentation"
    src="https://edu-admin.skolca.ru/draftfile.php/11572/user/draft/516105166/image%20%283%29.png?1764704609406"
    alt="" width="500" height="199"></p>
<h3>Шаг 6</h3>
<p>Не забывайте записывать в тетрадь описание каждой новой команды. На данный
  момент мы уже знаем такие:</p>
<pre class="language-python"><code>import turtle
turtle.shape('turtle')
turtle.color('brown', 'lime')
turtle.forward(100)
turtle.backward(100)
turtle.penup()
turtle.pendown()
turtle.right(90)
turtle.left(90)
turtle.mainloop()</code></pre>
<h3>Шаг 7</h3>
<p>Теперь вы знаете все, чтобы приказать черепашке нарисовать квадрат со
  стороной 100 шагов.<br>Поэкспериментируйте с разными фигурами. Вспомните
  геометрию, чтобы нарисовать правильный треугольник, правильный шестиугольник и
  т.п.<br>Попробуйте дать черепашке команду <strong>circle()</strong>. Как вы
  думаете, что нужно указать в скобках? Какой есть самый главный параметр у
  окружности?</p>
<p></p>
<p></p>
