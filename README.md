# goit-markup-hw-03

- Критерии приёма работы наставником === Проект ===
- «A1» В корне проекта есть папка images с изображениями.

- «A2» В корне проекта есть папка css с файлами стилей.

- «A3» Все стили написаны в одном файле styles.css, который находится в папке
  css.

- «A4» В названиях файлов нет заглавных букв, пробелов и транслита, только буквы
  и слова английского языка.

- «A5» Исходный код отформатирован при помощи Prettier.

- «A6» Все изображения и текстовый контент взяты из макета.

- «A7» На всех HTML-страницах подключен нормализатор стилей modern-nomalize.

- «A7» Код написан следуя руководству.

==== Оформление ====

- «B1» Допускается глобальный сброс стилей по селектору тега для элементов
  <h1>...<h6>, <p> и <ul>.

- «B2» У элементов нет внешних отступов (свойство margin) «пробивающих»
  родительский элемент.

«B3» В однострочных коллекциях элементов очищен крайний левый или правый margin
элементов (если он есть).

- «B4» Для отступов между двумя соседними элементами используется свойство
  margin.

- «B5» Для зазора между границей родителя и его ребёнком используется свойство
  padding.

- «B6» Размеры внешних отступов (свойство margin) и внутренних полей (свойство
  padding) элементов заданы точно по макету.

- «B7» Создан общий вспомогательный класс .container для центрирования и
  ограничения контента по ширине.

- «B8» Ширина «контейнера» соответствует макету и равна 1200px.

- «B9» «Контейнер» оборачивает контент хедера, футера и секций. То есть
  находится внутри них.

- «B10» Для расположения элементов используется Flexbox, но только там, где это
  необходимо. Например в шапке, навигации, списках в секциях и так далее, то
  есть там, где расположить элементы горизонтально по другому невозможно.

- «B11» Финальные размеры блоков в браузере соответствуют макету.

- «B12» У элементов нет фиксированной высоты, она определяется их контентом.

- «B13» У хедера есть нижняя рамка, необходимо сильно приблизить макет чтобы
  увидеть её.

- «B14» Секции расположены друг под другом как стопка книг, без внешних
  отступов.

«B15» Для всех секций используется один класс .section, заданы верхние и нижние
падинги по 94px, отодвигающие контент внутрь секции.

«B16» Для построения сеток используется техника описанная в конспекте и
видео-мастерской.

«B17» В карточках на странице Портфолио есть рамка (свойство border), но только
в нижней части карточки.

Немного напутствия, для выполнения третьего ДЗ:

1. Хедер,секции и футер ставятся друг на друга, как кирпичики. Между ними нет
   отступов. Цельная обоина, грубо говоря. $

2. Контейнер (это негласное правило так называть) - один для всего сайта. Он
   всегда внутри секции. Его основная цель - ограничить по ширине и
   горизонтально выровнять контент. Верхних и нижних маржинов/паддингов как
   правило ему не задают.

3. Хедер - большой смысловой элемент, как и секция. В ней есть небольшая
   особенность. Есть практика, когда высоту его задает паддинги ссылок. Просто
   принято ссылки оформлять как кнопки. Да, и увеличив площадь ссылки мы только
   увеличиваем шанс, что юзер кликнет в нее без проблем, мы упрощаем это для
   него.

4. Секция - независимый смысловой блок. ВСЕГДА на 100% ширины экрана. Именно ей
   задаются паддинги верхние и нижние. Мы создаем границы для контента. Именно
   секции задается фон, так как он всегда на 100% ширины экрана. Ограничения по
   ширине имеют картинки.
5. Маржины использовать внутри родительских блоков. Не распираем родителя.
   Родителю задаете паддинги, а дети между собой отодвигаются маржинами. Для
   использования маржинов старайтесь придерживаться направления по потоку -
   правый и нижний. Это не конкретный устав. Так просто проще запомнить на
   начальном этапе. И проще фиксить и искать неточности визуально, максимально
   быстро находя их в девтулзах.

И ещё немного:

1.  Ссылочкам в хедере уместно задавать вертикальные паддинги, чтобы увеличить
    кликабельную область.
2.  Марджинов между секциями на макете НЕТ. Отступы по 94рх – это ПАДДИНГИ.
3.  Содержимое хедера, футера и каждой из секций должно быть обернуто в
    див-контейнер с шириной 1200рх и горизонтальными паддингами по 15рх.

4.  Не забывайте задавать элементам списков в секциях ширину. При этом вместо
    свойства justify-content: space-between более надежным вариантом будет
    задать отступы между элементами (li) с помощью марджинов (крайние отступы не
    забываем обнулять).

5.  Для тега img задаем свойство display: block.

6.  Элементам, для которых это требуется, задаем бордеры (к примеру, хедеру,
    карточкам с секции портфолио).

7.  Нижнюю часть карточек с членами команды и карточек портфолио (элементы под
    изображением) уместно обернуть в див, которому задать паддинги со всех
    сторон.

8.  Фиксированную высоту (свойство height) элементам НЕ задаем.:exclamation:

9.  У некоторых элементом могут быть дефолтные, примененные браузером, марджины
    и паддинги, которые визуально похожи по размерам на те, которые вам нужно (к
    примеру, у заголовков или абзацев). Но на это надеяться не стоит: все, что
    по дефолту, обнуляем, и задаем отступы явно - в тех случаях и в том размере,
    в каких и в каком нам нужно.

10. Ну и, разумеется, внимательно читаем т/з, в частности: · у дочерних
    элементов нет внешних отступов margin пробивающих родителя; · расположение
    элементов, позиционирование которых используя стандартный поток документа
    невозможно, сделано с помощью Flexbox. То есть флексы используем ТОЛЬКО там,
    где в них действительно есть необходимость – повсеместно расставлять их не
    нужно. Все кто внимательно изучил данную информацию и применил её на
    практике, сдадут работу с первого раза
