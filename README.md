# Ex.07 Restaurant Website
## Date:

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
### index.html
```
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <title>LITTLE LEMON</title>
    <meta name="description" content="Little Lemon is a restaurant that serves the best lemonade in town.">
    <meta name="author" content="Little Lemon">
    
    <link rel="stylesheet" href="style.css">

    <link rel="icon" href="favicon.png" type="image/png">
    <link rel="apple-touch-icon" href="favicon.png">
    <link rel="shortcut icon" href="favicon.png" type="image/png">

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
    <link href="https://fonts.googleapis.com/css2?family=Markazi+Text:wght@400;600;700&display=swap" rel="stylesheet">
</head>

<body>
    <header>
        <img src="assets/img/logo.png" alt="logo">
    </header>
    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="menu.html">Menu</a></li>
            <li><a href="book.html">Book</a></li>
            <li><a href="about.html">About</a></li>
        </ul>
    </nav>
    <main>
        <div class="promote-row">
            <article>
                <h2>30% Off This Weekend</h2>
                <p>Little Lemon is a restaurant that serves the best lemonade in town. We have a variety of lemonades that you can choose from. We also have a variety of food that you can enjoy with your lemonade. We are open from 10am to 10pm every day. Come and visit us today!</p>
            </article>
        </div>
        <div class="row">
            <article>
                <h3>Our New Menu</h3>
                <img src="assets/img/home/new_menu.jpg" alt="Our new menu">
                <p>Little Lemon is a restaurant that serves the best lemonade in town. We have a variety of lemonades that you can choose from. We also have a variety of food that you can enjoy with your lemonade. We are open from 10am to 10pm every day. Come and visit us today!</p>
                <a href="menu.html">See our new menu</a>
            </article>
            <article>
                <h3>Book a table</h3>
                <img src="assets/img/home/book_table.jpg" alt="Book a table">
                <p>Little Lemon is a restaurant that serves the best lemonade in town. We have a variety of lemonades that you can choose from. We also have a variety of food that you can enjoy with your lemonade. We are open from 10am to 10pm every day. Come and visit us today!</p>
                <a href="book.html">See our new menu</a>
            </article>
            <article>
                <h3>Opening Hours</h3>
                <img src="assets/img/home/opening_hours.jpg" alt="Opening Hours">
                <p>Little Lemon is a restaurant that serves the best lemonade in town. We have a variety of lemonades that you can choose from.</p>
                <ul>
                    <li>Mon - Fri: 2pm - 10pm</li>
                    <li>Sat: 2pm - 11pm</li>
                    <li>Sun: 2pm - 9pm</li>
                </ul>
            </article>
        </div>
    </main>
    <footer>
        <div>
            <img src="assets/img/logo_footer.png" alt="">
        </div>
        <div>
            <p>&copy; 2024 Little Lemon</p>
        </div>
    </footer>
</body>
</html>
```
### style.css
```
/*! minireset.css v0.0.6 | MIT License | github.com/jgthms/minireset.css */html,body,p,ol,ul,li,dl,dt,dd,blockquote,figure,fieldset,legend,textarea,pre,iframe,hr,h1,h2,h3,h4,h5,h6{margin:0;padding:0}h1,h2,h3,h4,h5,h6{font-size:100%;font-weight:normal}ul{list-style:none}button,input,select{margin:0}html{box-sizing:border-box}*,*::before,*::after{box-sizing:inherit}img,video{height:auto;max-width:100%}iframe{border:0}table{border-collapse:collapse;border-spacing:0}td,th{padding:0}

body {
    background-color: #EDEFEE;
    font-family: 'Markazi Text', sans-serif;
    margin: 3rem 5% 3rem 5%;
}

/* Header */
header {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;    
}

header > img {
    max-width: 50%;
    height: auto;
}

/* Nav */
nav {
    margin: 2rem 0;

}

nav a {
    color: #EDEFEE;
    text-decoration: none;
}

nav ul {
    text-align: center;
    background-color: #333;
    border-radius: 10px;
    padding: 0.5rem;
    font-size: 1.2rem;
    letter-spacing: 0.1rem;
}

nav li {
    display: inline-block;
    margin: 0 2.5%;
}

/* Main */
main {
    display: grid;
    grid-template-rows: auto 1fr;
    width: 100%; 
    row-gap: 1rem;
}

main h2 {
    font-size: 3rem;
    text-shadow: 5px 5px 10px #000B11;
}

main h3 {
    font-size: 2rem;
    padding: 1rem 0;
}

main article {
    border-radius: 25px;
    padding: 1rem;
}

main p {
    padding: 1rem 0;
}

main img {
    transition: filter 0.3s ease;
}

main img:hover {
    filter: grayscale(100%);
}

main .row {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr; 
    gap: 1rem; 
}

main .row article {
    background-color: #F4E5D6;
}

main ul {
    padding-left: 2rem;
}

main .promote-row {
    grid-column: 1 / -1;
}

main .promote-row article {
    background-image: url('assets/img/home/discount_banner.jpg');
    background-color: #000B11;
    background-repeat: no-repeat;
    background-position: top center;
    background-size: 100% auto;
    color: white;
}

/* Footer */
footer {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 1rem;
    padding: 1rem;
}

footer img {
    max-width: 10%;
    height: auto;
}

footer > div:last-child { /* Copyright */
    text-align: right;
    border-top: 1px solid #333;
    margin-top: 1rem;;
}

```

## OUTPUT:
<img width="1680" alt="Restaurant_Code" src="https://github.com/user-attachments/assets/8b67e0b6-e88a-4d5c-b691-e087001803d0">
<img width="1680" alt="Restaurant(1)" src="https://github.com/user-attachments/assets/f6a3e940-bde1-4116-9f53-866eb3f85913">

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
