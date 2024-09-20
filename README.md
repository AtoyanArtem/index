<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Гиперссылки и формы</title>
</head>
<body>
  <h1>Гиперссылки</h1>
  <ul>
    <li><a href="https://kubsu.ru">Абсолютная ссылка на главную страницу kubsu.ru</a></li>
    <li><a href="https://kubsu.ru">Абсолютная ссылка на главную страницу kubsu.ru в протоколе https</a></li>
    <li><a href="https://kubsu.ru"><img src="logo.png" alt="Логотип КубГУ"></a></li>
    <li><a href="about.html">Сокращенная ссылка на внутреннюю страницу</a></li>
    <li><a href="/">Сокращенная ссылка на главную страницу</a></li>
    <li><a href="#footer">Ссылка на фрагмент текущей страницы</a></li>
    <li><a href="https://kubsu.ru/news?year=2023&month=09&day=15">Ссылка с тремя параметрами в URL</a></li>
    <li><a href="https://kubsu.ru/news?id=123">Ссылка с параметром id в URL</a></li>
    <li><a href="about/index.html">Относительная ссылка на страницу в текущем каталоге</a></li>
    <li><a href="../about/index.html">Относительная ссылка на страницу в каталоге about</a></li>
    <li><a href="../../index.html">Относительная ссылка на страницу в каталоге уровнем выше текущего</a></li>
    <li><a href="../../../index.html">Относительная ссылка на страницу в каталоге двумя уровнями выше</a></li>
    <li>Контекстная ссылка в тексте абзаца: <a href="https://kubsu.ru/news">новости КубГУ</a></li>
    <li><a href="https://example.com/page#fragment">Ссылка на фрагмент страницы стороннего сайта</a></li>
    <li>
      <map name="image-map">
        <area shape="rect" coords="0,0,100,100" href="https://kubsu.ru">
        <area shape="circle" coords="150,50,50" href="https://kubsu.ru/about">
      </map>
      <img src="image.png" alt="Карта ссылок" usemap="#image-map">
    </li>
    <li><a href="#">Ссылка с пустым href</a></li>
    <li><a>Ссылка без href</a></li>
    <li><a href="https://kubsu.ru" rel="nofollow">Ссылка, по которой запрещен переход поисковикам</a></li>
    <li><a href="https://kubsu.ru" rel="noindex">Запрещенная для индексации поисковиками</a></li>
  </ul>

  <h1>Форма</h1>
  <form action="submit.php" method="post">
    <label for="name">ФИО:</label>
    <input type="text" id="name" name="name">

    <label for="phone">Телефон:</label>
    <input type="tel" id="phone" name="phone">

    <label for="email">E-mail:</label>
    <input type="email" id="email" name="email">

    <label for="birthdate">Дата рождения:</label>
    <input type="date" id="birthdate" name="birthdate">

    <label for="gender">Пол:</label>
    <input type="radio" id="male" name="gender" value="male">
    <label for="male">Мужской</label>
    <input type="radio" id="female" name="gender" value="female">
    <label for="female">Женский</label>

    <label for="languages">Любимый язык программирования:</label>
    <select multiple id="languages" name="languages">
      <option value="pascal">Pascal</option>
      <option value="c">C</option>
      <option value="c++">C++</option>
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
    <textarea id="biography" name="biography"></textarea>

    <label for="contract">С контрактом ознакомлен(а):</label>
    <input type="checkbox" id="contract" name="contract">

    <input type="submit" value="Сохранить">
  </form>

  <ol>
    <li><a href="https://kubsu.ru" title="Главная страница КубГУ">Главная страница КубГУ</a></li>
    <li><a href="https://kubsu.ru/news" title="Новости КубГУ">Новости КубГУ</a></li>
    <li><a href="https://kubsu.ru/about" title="О КубГУ">О КубГУ</a></li>
  </ol>

  <a href="ftp://user:password@example.com/file.txt">Ссылка на файл на сервере FTP с авторизацией</a>

  <footer id="footer">
    <p>Подвал страницы</p>
  </footer>
</body>
</html>
