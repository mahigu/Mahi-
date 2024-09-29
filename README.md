<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <title>Travel With Us</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #3498db;
            color: white;
            padding: 10px 0;
            text-align: center;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        nav ul {
            list-style: none;
            padding: 0;
        }
        nav ul li {
            display: inline-block;
            margin-right: 15px;
        }
        nav ul li a {
            text-decoration: none;
            color: white;
            font-weight: bold;
        }
        .container {
            padding: 20px;
        }
        .banner {
            background-image: url('travel-banner.jpg');
            background-size: cover;
            height: 300px;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
        }
        .banner h2 {
            font-size: 3em;
            margin: 0;
        }
        .destinations, .services {
            margin-top: 20px;
        }
        .destinations h3, .services h3 {
            text-align: center;
            margin-bottom: 20px;
            font-size: 2em;
        }
        .destination-list, .service-list {
            display: flex;
            justify-content: space-around;
        }
        .destination-list div, .service-list div {
            background-color: #fff;
            padding: 15px;
            width: 30%;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
            text-align: center;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            margin-top: 20px;
        }
        form {
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            background-color: white;
            box-shadow: 0 0 10px rgba(0,0,0,0.1);
        }
        form input, form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
        }
        form input[type="submit"] {
            background-color: #3498db;
            color: white;
            border: none;
            cursor: pointer;
        }
        form input[type="submit"]:hover {
            background-color: #2980b9;
        }
    </style>
</head>
<body>

<header>
    <h1>Travel With Us</h1>
    <nav>
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#destinations">Destinations</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>
<div class="banner" id="home">
    <h2>Explore the World</h2>
</div>

<div class="container">
    <section class="destinations" id="destinations">
        <h3>Popular Destinations</h3>
        <div class="destination-list">
            <div>
                <h4>Paris</h4>
                <p>Experience the romance and charm of the city of lights.</p>
            </div>
            <div>
                <h4>Bali</h4>
                <p>Relax on the pristine beaches and explore the vibrant culture.</p>
            </div>
            <div>
                <h4>New York</h4>
                <p>Feel the energy of the city that never sleeps.</p>
            </div>
        </div>
    </section>

    <section class="services" id="services">
        <h3>Our Services</h3>
        <div class="service-list">
            <div>
                <h4>Flight Bookings</h4>
                <p>We provide hassle-free flight bookings with the best deals.</p>
            </div>
            <div>
                <h4>Hotel Reservations</h4>
                <p>Stay at the best hotels at affordable prices.</p>
            </div>
            <div>
                <h4>Tour Packages</h4>
                <p>Explore various destinations with our curated tour packages.</p>
            </div>
        </div>
    </section>

    <section id="contact">
        <h3>Contact Us</h3>
        <form action="submit_form.php" method="POST">
            <input type="text" name="name" placeholder="Your Name" required>
            <input type="email" name="email" placeholder="Your Email" required>
            <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
            <input type="submit" value="Send Message">
        </form>
    </section>
</div>

<footer>
    <p>&copy; 2024 Travel With Us. All Rights Reserved.</p>
</footer>

</body>
</html>
