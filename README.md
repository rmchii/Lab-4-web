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
 ![Screenshot (249)](https://github.com/user-attachments/assets/b7e69670-7bee-4be2-b4f7-ee1378819294)

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
![Screenshot (250)](https://github.com/user-attachments/assets/b8b0ff35-3990-4947-8560-cc02b05cc465)

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
![Screenshot (251)](https://github.com/user-attachments/assets/8ced60c9-2098-49fd-a38e-f8e895e1a833)

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
![Screenshot (253)](https://github.com/user-attachments/assets/46af9e30-0675-4eaf-ba1d-6bab46ccb70b)

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
![Screenshot (254)](https://github.com/user-attachments/assets/d5c1b05e-3426-4272-ab52-f4c24673b952)

5. Membuat Sidebar Widget
   <div class="sidebar">
            <div class="widget">
                <div class="widget-header">Widget Header</div>
                <div class="widget-content">
                    <a href="#" class="widget-link">Widget Link</a>
                    <a href="#" class="widget-link">Widget Link</a>
                    <a href="#" class="widget-link">Widget Link</a>
                    <a href="#" class="widget-link">Widget Link</a>
                    <a href="#" class="widget-link">Widget Link</a>
                </div>
            </div>
            <div class="widget">
                <div class="widget-header">Widget Text</div>
                <div class="widget-content">
                    <p class="widget-text">Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
                </div>
            </div>
   CSS 
   .sidebar {
  width: 250px;
  float: right;
  margin-top: 20px;
}

.widget {
  border: 1px solid #ccc;
  margin-bottom: 20px;
}

.widget-header {
  background-color: #0078d7;
  color: #fff;
  padding: 10px;
  font-weight: bold;
  font-size: 16px;
  text-align: center;
}

.widget-content {
  padding: 10px;
}

.widget-link {
  display: block;
  padding: 8px 10px;
  color: #0078d7;
  text-decoration: none;
  border-bottom: 1px solid #ccc;
}

.widget-link:last-child {
  border-bottom: none;
}

.widget-link:hover {
  background-color: #e6f3ff;
}

.widget-text {
  color: #333;
  line-height: 1.5;
}

.clearfix::after {
  content: "";
  display: table;
  clear: both;
}
Mengatur footer
footer {
  clear: both;
  background-color: #1d1d1d;
  padding: 20px;
  color: #eee;
}
![Screenshot (257)](https://github.com/user-attachments/assets/d17e641c-8750-4e63-835f-3975d9e9f545)

6. Menambahkan Elemen lainnya pada Main Content
   <section id="main">
            <div class="row">
                <div class="box">
                    <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
        class="image-circle">
        <h3>Heading</h3>
        <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis euismod.</p>
        <a href="#" class="btn btn-default">View detail</a>
        </div>
            <div class="box">
                <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""class="image-circle">
                <h3>Heading</h3>
                <p>Donec sed odio dui. Etiam porta sem malesuada magna molliseuismod.</p>
                <a href="#" class="btn btn-default">View detail</a>
                </div>
                <div class="box">
                <img src="https://dummyimage.com/120/71e6d4/fff.png" alt=""
                class="image-circle">
                <h3>Heading</h3>
                <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
                euismod.</p>
                <a href="#" class="btn btn-default">View detail</a>
                </div>
                </div>
        </section>
   CSS
   .box {
  display:block;
  float:left;
  width:33.333333%;
  box-sizing:border-box;
  -moz-box-sizing:border-box;
  -webkit-box-sizing:border-box;
  padding:0 10px;
text-align:center;
}
.box h3 {
margin: 15px 0;
}
.box p {
line-height: 20px;
font-size: 14px;
margin-bottom: 15px;
}
box img {
border: 0;
vertical-align: middle;
}
.image-circle {
border-radius: 50%;
}
.row {
margin: 0 -10px;
box-sizing: border-box;
-moz-box-sizing: border-box;
-webkit-box-sizing: border-box;
}
.row:after, .row:before,
.entry:after, .entry:before {
content:'';
display:table;
}
.row:after,
.entry:after {
clear:both;
}
![Screenshot (269)](https://github.com/user-attachments/assets/7fed3e29-b371-45db-a8d2-7fd2dee0d201)

7. Menambahkan Content Artikel
   <hr class="divider" />
        <article class="entry">
            <h2>First featurette heading.</h2>
            <img src="https://dummyimage.com/150/7b8a70/fff.png" alt="">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
        </article>
        <hr class="divider" />
        <article class="entry">
            <h2>First featurette heading.</h2>
            <img src="https://dummyimage.com/150/7b8a70/fff.png" alt=""
            class="right-img">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc pretium ac.</p>
        </article>
   CSS
   .divider {
  border:0;
  border-top:1px solid #eeeeee;
  margin:40px 0;
  }
  .entry {
  margin: 15px 0;
  }
  .entry h2 {
  margin-bottom: 20px;
  }
  .entry p {
    line-height: 25px;
    }
    .entry img {
    float: left;
    border-radius: 5px;
    margin-right: 15px;
    }
    .entry .right-img {
    float: right;
    }
   ![Screenshot (270)](https://github.com/user-attachments/assets/1597025c-358d-413e-807a-4fe448536290)

Pertanyaan dan Tugas
1. Tambahkan Layout untuk menu About
=> buat single layout yang berisi deskripsi, portfolio, dll
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>About</title>
    <link rel="stylesheet" type="text/css" href="layout.css">
</head>
<body>
    <div class="container">
        <header>
            <h1>About</h1>
        </header>
        <section class="about-description">
            <h2>Our Story</h2>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla nec eros vitae lacus ultricies sodales. Curabitur ac felis non lorem cursus suscipit ut a libero.</p>
        </section>
        <section class="portfolio">
            <h2>Portfolio</h2>
            <div class="portfolio-items">
                <div class="portfolio-item">
                    <img src="https://dummyimage.com/200x150/db7d25/fff.png" alt="Project 1">
                    <h3>Project 1</h3>
                    <p>Description of Project 1</p>
                </div>
                <div class="portfolio-item">
                    <img src="https://dummyimage.com/200x150/3e73e6/fff.png" alt="Project 2">
                    <h3>Project 2</h3>
                    <p>Description of Project 2</p>
                </div>
                <div class="portfolio-item">
                    <img src="https://dummyimage.com/200x150/71e6d4/fff.png" alt="Project 3">
                    <h3>Project 3</h3>
                    <p>Description of Project 3</p>
                </div>
            </div>
        </section>
    </div>
</body>
</html>
CSS
.container {
      width: 80%;
      margin: 0 auto;
  }
  
  .about-description, .portfolio {
      margin-bottom: 30px;
  }
  
  .portfolio-items {
      display: flex;
      gap: 20px;
  }
  
  .portfolio-item {
      width: 30%;
      text-align: center;
  }

  ![Screenshot (264)](https://github.com/user-attachments/assets/ae8119a5-7cbf-4324-858c-8f4a5811fb4d)

3. Tambahkan layout untuk menu Contact
=> yang berisi form isian: nama, email, message, dll
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kontak</title>
    <link rel="stylesheet" type="text/css" href="layout.css">
</head>
<body>
    <div class="container">
        <header>
            <h1>Kontak</h1>
        </header>
        
        <section class="contact-form">
            <h2>Get in Touch</h2>
            <form action="submit_contact.php" method="POST">
                <label for="name">Nama:</label>
                <input type="text" id="name" name="name" required>
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="5" required></textarea>

                <button type="submit">Send Message</button>
            </form>
        </section>
    </div>
</body>
</html>
CSS 
.contact-form {
    width: 50%;
    margin: 0 auto;
}

.contact-form label {
    display: block;
    margin-top: 15px;
    font-weight: bold;
}

.contact-form input, .contact-form textarea {
    width: 100%;
    padding: 10px;
    margin-top: 5px;
    border: 1px solid #ccc;
    border-radius: 5px;
}

.contact-form button {
    margin-top: 15px;
    padding: 10px 20px;
    background-color: #0078d7;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

.contact-form button:hover {
    background-color: #005fa3;
}

![Screenshot (263)](https://github.com/user-attachments/assets/54d74b08-6afd-4c4a-b2bb-c2f77a512527)
