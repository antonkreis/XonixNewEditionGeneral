<h1>Требования к проекту “Xonix New Edition”</h1>
<h2>1 Введение</h2>
<p align = "justify">Проект направлен на разработку сетевой многопользовательской игры под названием “Xonix New Edition”. Два пользователя будут иметь возможность подключаться к общей игре и играть в режиме реального времени. Оформление игры двухмерное. Тематика игры напоминает классическую игру "Xonix".</p>
<h2>2 Требования пользователя</h2>
<h3>2.1 Программные интерфейсы</h3>
<p align = "justify">Разработка будет вестись с использованием языка программирования Java. Будут задействованы как стандартные библиотеки, так и сторонние, например, LibGDX. Разработка будет вестись в Intellij Idea. В Таблице 1 собраны сведения об основных программных продуктах, которые будут использоваться в процессе разработки.</p>

Таблица 1 - Используемое в разработке стороннее ПО
<table align="center">
  <tr>
    <td>Название</td>
    <td>Oracle Java SE Development Kit 11</td>
    <td>libGDX</td>
    <td>JetBrains IntelliJ IDEA Community Edition </td>
  </tr>
    <tr>
    <td>Мнемоника</td>
    <td>Java</td>
    <td>libGDX</td>
    <td>IntelliJ IDEA</td>
  </tr>
    <tr>
    <td>Версия</td>
    <td>11.0.5</td>
    <td>1.9.10</td>
    <td>2019.3.5+</td>
  </tr>
</table>
<h3>2.2 Интерфейс пользователя</h3>
<p align = "justify">Создаваемый программный продукт будет иметь классический графический пользовательский интерфейс. При запуске пользователю предоставлено меню, в котором он сможет ввести свой Никнейм, данные для локального соединения с другим игроком, а также сможет выбрать пункт “Настройки” или “Помощь”. В пунтке "Помощь" пользователь может получить информацию о правилах игры и как установить соединение с соперником. Оформление меню и самой игры минималистичное, на фоне допускаются картинки, соответсвующие общему оформлению игры. На рисунке 1 представлен набросок меню.
<p align="center">
<img src="images/image_1_new2.png" alt="Меню игры">
</p>
<p align = "center">Рисунок 1 - Меню игры</p>
<p align = "justify">Перед началом игрового процесса пользователь, создающий игру, может выбрать ее длительность и количество захваченных территорий, необходимых для досрочного выигрыша. (рис. 3)</p>
<p align="center">
<img src="images/image_4_new.png" alt="Настройка партии">
</p> 
<p align = "center">Рисунок 2 - Настройка партии</p>
<p align = "justify">После установления соединения с другим игроком пользователь включается в игровой процесс. На игровом поле будет происходить непосредственно игровой процесс (завоевание территорий игроками и т.д.), справа на информационном поле будет размещена прочая информация (например, текущие достижения игроков, пункты управления и т.д.). На рисунке 2 представлена разметка и игрового процесса.</p>
<p align="center">
<img src="images/image_2_new.png" alt="Разметка игрового процесса">
</p> 
<p align = "center">Рисунок 3 - Разметка игрового процесса</p>
<p align = "justify">В конце игры пользователю будет предоставлена статистика о завершенном сеансе. В ней будет содержаться информация о количестве захваченных территорий, о затраченном на сеанс времени и т.д. (рис. 4)</p> 
<p align="center">
<img src="images/image_3_new.png" alt="Статистика сеанса">
</p>
<p align = "center">Рисунок 4 - Статистика сеанса</p>
<h3>2.3 Характеристики пользователей</h3>
<p align = "justify">Программный продукт нацелен на рядового пользователя, обладающего стандарными компьютерными навыками и имеющим опыт в многопользовательских играх. Он должен уметь устанавливать соединение по локальной сети.</p>
<h3>2.4 Предположения и зависимости</h3>
<p align = "justify">На перечисленные в данном документе требования к создаваемому программному продукту могут влиять сроки, отведенные для разработки, а также новые идеи.</p>
<h2>3 Системные требования</h2>
<h3>3.1 Функциональные требования</h3>
<ul>
 <li><p align = "justify">Качественное оформление приложения, включающее в себя понятный пользовательский интерфейс, красивые текстуры и анимацию;</p></li>
 <li><p align = "justify">Возможность ввода пользовательского имени (Nickname) с проверкой на корректность ввода;</p></li>
 <li><p align = "justify">Наличие многопользовательского режима, с возможностью как создать собственный игровой сеанс, так и подключиться к существующему. Игрок, создавший и настроивший сеанс, ждет подключения своего соперника;</p></li>
 <li><p align = "justify">После установки соединения между компьютерами игроков начинается непосредственно игровой процесс. Игроки стремятся отрезать себе наибольший кусок территорий, мешая друг другу подобно тому, как вражеские точки (или мячики) мешают игроку захватить территории в оригинальной игре "Xonix". На игровом поле будут находится различные бонусы/антибонусы. Будет происходить счет времени и захваченных территорий. Победителем будет признан тот игрок, который захватил определенное количество территорий или захватил больше территорий за ограниченный промежуток времени. По окончании игры пользователям будет предоставлена статистика прошедшей партии, содержащая данные о времени, количестве набранных очков, количестве захваченных территорий. Будет предложен выход в главное меню.</p></li>
 <li><p align = "justify">Адекватная реакция приложения на различные ненормальные ситуации, такие как потеря сетевого подключения, различные сбои в работе приложения;</p></li>
 <li><p align = "justify">(В перспективе) поддержка другими платформами (напр., Android).</p></li>
</ul>
<h3>3.2 Нефункциональные требования</h3>
<h4>3.2.1 Атрибуты качества</h4>
<p align = "justify">Для создаваемого продукта необходимы такие атрибуты, как стабильность работы многопользовательского режима, невысокая требовательность к ресурсам компьютера. Это должно обеспечить приятный игровой процесс, не сопровождающийся перегревом компьютера и сбоями в игре. Приложение не будет требовать никаких личных данных пользователя во избежание несанкционированного доступа к ним.</p>
