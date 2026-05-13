<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Мой Магазин</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background: #f4f4f4;
        }
        header {
            background: #333;
            color: #fff;
            padding: 15px;
            text-align: center;
        }
        nav {
            background: #444;
            display: flex;
            justify-content: center;
            gap: 15px;
            padding: 10px;
        }
        nav a { color: white; text-decoration: none; }

        /* Сетка товаров */
        .container {
            display: grid;
            /* Делает колонки, которые подстраиваются под ширину экрана */
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            padding: 20px;
        }

        /* Карточка товара */
        .product-card {
            background: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            display: flex;
            flex-direction: column; /* Элементы внутри (текст, кнопка) идут вниз */
        }

        /* КАРТИНКА: Главный блок */
        .product-card img {
            width: 100%;
            /* Если хочешь, чтобы интерфейс СЪЕЗЖАЛ в зависимости от высоты фото: */
            height: auto; 
            display: block;
            
            /* Если хочешь, чтобы все картинки были ОДНОЙ высоты (например, 250px), 
               но НЕ сплющивались, расскомментируй это: */
            /* height: 250px; 
               object-fit: cover; */
        }

        .product-info {
            padding: 15px;
            display: flex;
            flex-direction: column;
            flex-grow: 1; /* Позволяет блоку занимать всё свободное место */
        }

        .product-card h3 { margin: 0 0 10px 0; font-size: 18px; }
        .product-card p { color: #555; flex-grow: 1; margin-bottom: 15px; }
        
        .price {
            font-weight: bold;
            font-size: 20px;
            color: #e91e63;
            margin-bottom: 15px;
        }

        .btn {
            background: #e91e63;
            color: white;
            padding: 12px;
            text-align: center;
            border-radius: 4px;
            text-decoration: none;
            transition: 0.3s;
        }
        .btn:hover { background: #c2185b; }

        footer { background: #333; color: white; text-align: center; padding: 20px; margin-top: 40px; }
    </style>
</head>
<body>

<header><h1>Мой Интернет-Магазин</h1></header>

<nav>
    <a href="#">Главная</a>
    <a href="#">Каталог</a>
    <a href="#">О нас</a>
</nav>

<main class="container">
    <!-- Карточка 1 -->
    <div class="product-card">
        <img src="godo.png" alt="Товар 1">
        <div class="product-info">
            <h3>Товар 1</h3>
            <p>«В ожидании Годо» представляет собой трагедию, в которой «ничего не происходит, никто не приходит, никто не уходит». Произведение сосредоточено на изображении состояния человеческой психики, процесса психической деятельности и её нарушений. Персонажи пьесы не обладают ярко выраженными характерами, а сюжет лишён последовательного развития. «В ожидании Годо» является подлинным новаторством в истории театра и первой успешно поставленной пьесой театра абсурда </p>
            <div class="price">1 500 ₽</div>
            <a href="#" class="btn">В корзину</a>
        </div>
    </div>

    <!-- Карточка 2 -->
    <div class="product-card">
        <img src="listia.jpg" alt="Товар 2">
        <div class="product-info">
            <h3>Товар 2</h3>
            <p>"Дом листьев" — это роман, который сочетает в себе элементы ужасов, любви, сатиры и исследовательских работ. Он рассказывает о стремительно расширяющемся доме, который становится объектом интереса и исследований, включая фундаментальное исследование о фильме, которого не существует, сделанное слепым стариком. Роман также исследует записки из лабиринтов подсознания и сентиментальное блуждание по инфернальным кругам жизни. "Дом листьев" стал известным благодаря своей необычной структуре и формам изложения, которые делают его ярким примером эргодической литературы. </p>
            <div class="price">2 500 ₽</div>
            <a href="#" class="btn">В корзину</a>
        </div>
    </div>
    <div class="product-card">
        <img src="piknik.jpg" alt="Товар 2">
        <div class="product-info">
            <h3>Товар 2</h3>
            <p>Пикник на обочине
фантастическая повесть братьев Стругацких, впервые изданная в 1972 году. Действие повести происходит на Земле предположительно в 1970-е годы в городке Хармонт, в выдуманной англоязычной стране. Одна из основных тем — нравственный выбор тех, в чьи руки попадают артефакты Зоны, то, как ими воспользуется человечество, которое, строго говоря, плохо понимает, в чём предназначение этих опасных вещей, неизвестно зачем оставленных пришельцами.</p>
            <div class="price">2 500 ₽</div>
            <a href="#" class="btn">В корзину</a>
        </div>
    </div>
</main>

<footer>&copy; 2026 Мой Магазин</footer>

</body>
</html>
