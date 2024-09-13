# index
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Сверстанная HTML 5 страница</title>
</head>
<body>
  <h1>Список гиперссылок</h1>
  <ul>
    <li><a href="https://kubsu.ru">Главная страница kubsu.ru (абсолютная)</a></li>
    <li><a href="https://kubsu.ru">Главная страница kubsu.ru (абсолютная, https)</a></li>
    <li><a href="https://kubsu.ru/images/logo.png"><img src="https://kubsu.ru/images/logo.png" alt="Логотип КубГУ"></a></li>
    <li><a href="about.html">Внутренняя страница (сокращенная)</a></li>
    <li><a href="/">Главная страница (сокращенная)</a></li>
    <li><a href="#footer">Фрагмент текущей страницы</a></li>
    <li><a href="https://kubsu.ru/news?page=1&category=science&sort=date">Ссылка с тремя параметрами в URL</a></li>
    <li><a href="https://kubsu.ru/news?id=123">Ссылка с параметром id в URL</a></li>
    <li><a href="about/index.html">Страница в текущем каталоге (относительная)</a></li>
    <li><a href="about/index.html">Страница в каталоге about (относительная)</a></li>
    <li><a href="../index.html">Страница в каталоге уровнем выше (относительная)</a></li>
    <li><a href="../../index.html">Страница в каталоге двумя уровнями выше (относительная)</a></li>
    <li>Контекстная ссылка в тексте абзаца: <a href="https://kubsu.ru/news">Новости КубГУ</a></li>
    <li><a href="https://yandex.ru#search">Фрагмент страницы стороннего сайта</a></li>
    <li>
      <map name="map">
        <area shape="rect" coords="0,0,100,100" href="https://kubsu.ru">
        <area shape="circle" coords="150,150,50" href="https://kubsu.ru/about">
      </map>
      <img src="map.png" usemap="#map" alt="Карта">
    </li>
    <li><a href="#">Ссылка с пустым href</a></li>
    <li><a>Ссылка без href</a></li>
    <li><a href="https://kubsu.ru" rel="nofollow">Ссылка, по которой запрещен переход поисковикам</a></li>
    <li><a href="https://kubsu.ru" rel="noindex">Ссылка, запрещенная для индексации поисковиками</a></li>
    <ol>
      <li><a href="https://kubsu.ru" title="Главная страница">Главная страница</a></li>
      <li><a href="https://kubsu.ru/news" title="Новости">Новости</a></li>
      <li><a href="https://kubsu.ru/about" title="О КубГУ">О КубГУ</a></li>
    </ol>
    <li><a href="ftp://user:password@ftp.kubsu.ru/file.txt">Ссылка на файл на сервере FTP с авторизацией</a></li>
  </ul>

  <h1>Форма</h1>
  <form action="submit.php" method="post">
    <label for="name">ФИО:</label>
    <input type="text" id="name" name="name" required>

    <label for="phone">Телефон:</label>
    <input type="tel" id="phone" name="phone" required>

    <label for="email">E-mail:</label>
    <input type="email" id="email" name="email" required>

    <label for="birthdate">Дата рождения:</label>
    <input type="date" id="birthdate" name="birthdate" required>

    <label for="gender">Пол:</label>
    <input type="radio" id="male" name="gender" value="male" required>
    <label for="male">Мужской</label>
    <input type="radio" id="female" name="gender" value="female" required>
    <label for="female">Женский</label>

    <label for="languages">Любимый язык программирования:</label>
    <select id="languages" name="languages" multiple required>
      <option value="pascal">Pascal</option>
      <option value="c">C</option>
      <option value="cpp">C++</option>
      <option value="javascript">JavaScript</option>
      <option value="php">PHP</option>
      <option value="python">Python</option>
      <option value="java">Java</option>
      <option value="haskell">Haskell</option>
      <option value="clojure">Clojure</option>
      <option value="prolog">Prolog</option>
      <option value="scala">Scala</option>
    </select>

    <label for="biography">Биография:</label>
    <textarea id="biography" name="biography" required></textarea>

    <label for="contract">С контрактом ознакомлен(а):</label>
    <input type="checkbox" id="contract" name="contract" required>

    <input type="submit" value="Сохранить">
  </form>

  <div id="footer">Футер</div>
</body>
</html>
