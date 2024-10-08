# Explorer

# CODE:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EXPLORER</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            background-color: #f4f4f4;
            color: black;
        }
        header {
            background-color: #fff;
            padding: 10px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid #ddd;
        }
        header .logo {
            font-size: 24px;
            font-weight: bold;
            color: black;
        }
        header nav ul {
            list-style: none;
            display: flex;
            gap: 20px;
        }
        header nav ul li a {
            text-decoration: none;
            color: black;
            font-weight: bold;
        }
        .hero {
            background: url('hero-image.jpg') no-repeat center center/cover;
            color: white;
            padding: 100px 20px;
            text-align: center;
        }
        .hero h1 {
            font-size: 36px;
            margin-bottom: 20px;
        }
        .hero .highlight {
            color: skyblue;
        }
        .hero .hero-content {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 20px;
        }
        .hero .search-container {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        .hero .search-bar input {
            padding: 10px;
            width: 300px;
            border-radius: 5px;
            border: none;
        }
        .hero .search-bar button {
            padding: 10px 20px;
            background-color: skyblue;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .hero img {
            width: 600px;
            height: auto;
            border-radius: 10px;
        }
        .destinations {
            padding: 50px 20px;
            background-color: #fff;
        }
        .destinations h2 {
            text-align: center;
            margin-bottom: 40px;
            font-size: 32px;
        }
        .destination-grid {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }
        .destination-item {
            background-color: #f4f4f4;
            padding: 20px;
            border-radius: 5px;
            text-align: center;
        }
        .destination-item img {
            width: 100%;
            height: 150px;
            object-fit: cover;
            border-radius: 5px;
            margin-bottom: 20px;
        }
        .destination-item h3 {
            font-size: 18px;
            margin-bottom: 10px;
        }
        .destination-item p {
            font-size: 14px;
            color: #666;
            margin-bottom: 20px;
        }
        .destination-item .read-more {
            text-decoration: none;
            background-color: skyblue;
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
        }
        .contact {
            padding: 50px 20px;
            background-color: #fff;
            text-align: center;
        }
        .contact h2 {
            margin-bottom: 40px;
            font-size: 32px;
        }
        .contact form {
            display: grid;
            gap: 20px;
            max-width: 500px;
            margin: 0 auto;
        }
        .contact form label {
            text-align: left;
            font-weight: bold;
        }
        .contact form input {
            padding: 10px;
            border-radius: 5px;
            border: 1px solid #ddd;
            width: 100%;
        }
        .contact form button {
            padding: 10px;
            background-color: skyblue;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">Locale Explorer Guide</div>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Destinations</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </nav>
    </header>
    <section class="hero">
        <div class="hero-content">
            <div class="search-container">
                <div class="search-bar">
                    <input type="text" placeholder="Search">
                    <button>Explore</button>
                </div>
                <img src="img/plane.webp" alt="Adventure">
            </div>
        </div>
    </section>
    <section class="destinations">
        <h2>Destinations</h2>
        <div class="destination-grid">
            <div class="destination-item">
                <img src="img/bali.jpg" alt="Temple">
                <h3>Beaches, temples, culture, art, tranquility</h3>
                <p><b>Bali</b></p>
                <a href="#" class="read-more">Read More</a>
            </div>
            <div class="destination-item">
                <img src="img/egypt.jpeg" alt="Pyramid">
                <h3>Pyramids, Sphinx, Nile, temples, desert</h3>
                <p><b>Egypt</b></p>
                <a href="#" class="read-more">Read More</a>
            </div>
            <div class="destination-item">
                <img src="img/paris.jpg" alt="Tower">
                <h3>Eiffel Tower, romance, art, fashion</h3>
                <p><b>paris</b></p>
                <a href="#" class="read-more">Read More</a>
            </div>
            <div class="destination-item">
                <img src="img/rio.jpeg" alt="Jesus">
                <h3>Carnival, beaches, samba, Christ the Redeemer</h3>
                <p><b>Rio de Janeiro</b></p>
                <a href="#" class="read-more">Read More</a>
            </div>
            <div class="destination-item">
                <img src="img/rome.jpeg" alt="Pope">
                <h3>Colosseum, history, Vatican, architecture</h3>
                <p><b>Rome</b></p>
                <a href="#" class="read-more">Read More</a>
            </div>
            <div class="destination-item">
                <img src="img/venice.jpg" alt="Love">
                <h3> Canals, gondolas, romance, architecture</h3>
                <p><b>Venice</b></p>
                <a href="#" class="read-more">Read More</a>
            </div>
        </div>
    </section>
    <section class="contact">
        <h2>Contact Us</h2>
        <form>
            <label for="name">Your Name:</label>
            <input type="text" id="name" name="name">

            <label for="hometown">Your Home Town:</label>
            <input type="text" id="hometown" name="hometown">

            <label for="destination">Where would you like to go?</label>
            <input type="text" id="destination" name="destination">

            <label for="contact">Contact Number:</label>
            <input type="text" id="contact" name="contact">

            <button type="submit">Submit</button>
        </form>
    </section>
</body>
</html>