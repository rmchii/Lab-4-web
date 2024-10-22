# Lab-4-web

1. Membuat box element
   <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTP-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
</head>
<body>
    <header>
        <h1>Box Element</h1>
        <link rel="stylesheet" type="text/css" href="style.css">
    </header>
    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
    </section>
    
</body>
</html>
  css float property
  div {
    float: left;
    padding: 10px;
 }
 .div1 {
    background: red;
 }
 .div2 {
    background: yellow;
 }
 .div3 {
    background: green;
 }
2. Mengatur Clearfix element
  <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
        <div class="div4">Div 4</div>
    </section>
   css 
   .div4 {
   background-color: blue;
   clear: left;
   float: none;
 }

 3. Membuat layout sederhana
    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTP-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>layout Sederhana</title>
    <link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
    <div id="container">

    </div>
    <header>
        <h1>layout Sederhana</h1>
    </header>
    <nav>
        <a href="home.html" class="active">home</a>
        <a href="artkel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html">Kontak</a>
    </nav>
    <section id="hero" ></section>
    <section id="wrapper">
        <section id="main"></section>
        <aside id="sidebar"></aside>
    </section>
    <footer>
        <p>&copy; 2021 - Universiras Pelita Bangsa</p>
    </footer>
</body>
CSS

@import 
url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import 
url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');

* {
  margin: 0;
  padding: 0;
}

body {
  line-height: 1;
  font-size: 100%;
  font-family: 'Open Sans', sans-serif;
  color: #5a5a5a;
}
#container {
  width: 980px;
  margin: 0 auto;
  box-shadow: 0 0 1em #cccccc;
}
header {
  padding: 20px;

}
header h1 {
  margin: 20px 10px;
  color: #b5b5b5;
}
Membuat navigasi
nav {
    display: block;
    background-color: #1f5faa;
}
nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
}
nav a.active,
nav a:hover {
    background-color: #2b83ea;
}
4. membuat hero panel
<section id="hero" >
        <h1>Hello World!</h1>
        <p>Lorem, ipsum dolor sit amet consectetur adipisicing elit. Vestibulum lorem elit, iaculis volutpat, malesuada tincidunt arcu. proin in leo fringilla, Vestibulum mi porta, faucibus felis. integer pharetra est nunc, nec pretium nunc pretium ac.</p>
        <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
    </section>
    CSS 

    #hero {
    background-color: #e4e4e5;
    padding: 50px 20px;
    margin-bottom: 20px;
}
#hero h1 {
    margin-bottom: 20px;
    font-size: 35px;
}

#hero p{
    margin-bottom: 20px;
    font-size: 18px;
    line-height: 25px;
}
