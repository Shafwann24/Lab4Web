<h2>1. Membuatlab4_box.htm</h2>

         <!DOCTYPE html>
    <html lang="en">
    <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Box Element</title>
    </head>
    <body>
     <header>
     <h1>Box Element</h1>
     </header>
    </body>
    </html>
   
![image](https://github.com/user-attachments/assets/72ecbc2c-dc85-4ca5-a847-cfa0ce42b73c)
<br>

<h2>2. Membuat Box Element</h2>

    <section>
     <div class="div1">Div 1</div>
     <div class="div2">Div 2</div>
     <div class="div3">Div 3</div>
    </section>

<h2>Menambahkan CSS Float Property</h2>

    <style>
     div {
     float:left;
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
    </style>

  ![image](https://github.com/user-attachments/assets/fa2ee7d6-a86b-4e22-a20b-e5eb46502ff7)
<br>

<h2>3. Mengatur Clearfix Element</h2>

    <section>
     <div class="div1">Div 1</div>
     <div class="div2">Div 2</div>
     <div class="div3">Div 3</div>
     <div class="div4">Div 4</div>
    </section>

  ![image](https://github.com/user-attachments/assets/004d0e28-c3a3-4087-9eba-5f4667aacbc8)
<br>

<h2>Membuat Layout Sederhana</h2>

    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Layout Sederhana</title>
        <link rel="stylesheet" href="style.css">
    </head>
    <body>
        <div id="container">
    
        
    </body>
    </html>

<h2>Kemudian buat kerangka layout dengan semantics element seperti berikut</h2>

    <header>
     <h1>Layout Sederhana</h1>
    </header>
    <nav>
     <a href="home.html" class="active">Home</a>
     <a href="artikel.html">Artikel</a>
     <a href="about.html">About</a>
     <a href="kontak.html">Kontak</a>
    </nav>
    <section id="hero"></section>
    <section id="wrapper">
     <section id="main"></section>
     <aside id="sidebar"></aside>
    </section>
    <footer>
     <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>

![image](https://github.com/user-attachments/assets/08961990-f277-4bd1-9cf9-7b125a255737)

<h2>Kemudian tambahkan kode CSS untuk membuat layoutnya</h2>

    /* import google font */
    @import
    url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400
    ;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
    @import
    url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0
    ,300;0,700;1,300&display=swap');
    /* Reset CSS */
    * {
     margin: 0;
     padding: 0;
    }
    body {
     line-height:1;
     font-size:100%;
     font-family:'Open Sans', sans-serif;
     color:#5a5a5a;
    }
    #container {
     width: 980px;
     margin: 0 auto;
     box-shadow: 0 0 1em #cccccc;
    }
    /* header */
    header {
     padding: 20px;
    }
    header h1 {
     margin: 20px 10px;
     color: #b5b5b5;
    }

![image](https://github.com/user-attachments/assets/1af52861-0671-4859-85d4-e5dbf6797d02)

<h2>Membuat Navigasi</h2>

    /* navigasi */
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

![image](https://github.com/user-attachments/assets/61662287-40dc-41ba-805e-8f33ff11b16c)

<h2>Membuat Hero Panel</h2>

    <section id="hero">
     <h1>Hello World!</h1>
     <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vestibulum lorem
    elit, iaculis innisl volutpat, malesuada tincidunt arcu. Proin in leo fringilla,
    vestibulum mi porta, faucibus felis. Integer pharetra est nunc, nec pretium nunc
    pretium ac.</p>
     <a href="home.html" class="btn btn-large">Learn more &raquo;</a>
    </section>

CSS

    /* Hero Panel */
    #hero {
     background-color: #e4e4e5;
     padding: 50px 20px;
     margin-bottom: 20px;
    }
    #hero h1 {
     margin-bottom: 20px;
     font-size: 35px;
    }
    #hero p {
     margin-bottom: 20px;
     font-size: 18px;
     line-height: 25px;
    }


![image](https://github.com/user-attachments/assets/efdb94ec-5725-4083-a9af-fe711d246482)

<br>

<h2>Mengatur Layout Main dan Sidebar</h2>

    /* main content */
    #wrapper {
     margin: 0;
    }
    #main {
     float: left;
     width: 640px;
     padding: 20px;
    }
    /* sidebar area */
    #sidebar {
     float: left;
     width: 260px;
     padding: 20px;
    }


<h2>Membuat Sidebar Widget</h2>

    <aside id="sidebar">
      <div class="widget-box">
        <h3 class="title">Widget Header</h3>
        <ul>
          <li><a href="#">Widget Link</a></li>
          <li><a href="#">Widget Link</a></li>
          <li><a href="#">Widget Link</a></li>
          <li><a href="#">Widget Link</a></li>
          <li><a href="#">Widget Link</a></li>
        </ul>
      </div>
      <div class="widget-box">
        <h3 class="title">Widget Text</h3>
        <p>Vestibulum lorem elit, iaculis in nisl volutpat, malesuada tincidunt
        arcu. Proin in leo fringilla, vestibulum mi porta, faucibus felis. Integer
        pharetra est nunc, nec pretium nunc pretium ac.</p>
      </div>
    </aside>
    
<h2>Menambahkan CSS</h2>


    /* widget */
    .widget-box {
     border:1px solid #eee;
     margin-bottom:20px;
    }
    .widget-box .title {
     padding:10px 16px;
     background-color:#428bca;
     color:#fff;
    }
    .widget-box ul {
     list-style-type:none;
    }
    .widget-box li {
     border-bottom:1px solid #eee;
    
    
![image](https://github.com/user-attachments/assets/b386ea1c-2807-4050-a0f6-c1fa45550595)


<h2>Mengatur Footer</h2>


    /* footer */
    footer {
     clear:both;
     background-color:#1d1d1d;
     padding:20px;
     color:#eee;
    }

  ![image](https://github.com/user-attachments/assets/7653cef7-0018-4ee8-aa2c-59fafdae5c19)


  <h2>Menambahkan Elemen lainnya pada Main Content</h2>

      <section id="main">
     <div class="row">
     <div class="box">
     <img src="https://dummyimage.com/120/db7d25/fff.png" alt=""
    class="image-circle">
     <h3>Heading</h3>
     <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
    euismod.</p>
     <a href="#" class="btn btn-default">View detail</a>
     </div>
     <div class="box">
     <img src="https://dummyimage.com/120/3e73e6/fff.png" alt=""
    class="image-circle">
     <h3>Heading</h3>
     <p>Donec sed odio dui. Etiam porta sem malesuada magna mollis
    euismod.</p>
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

    /* box */
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
    
![image](https://github.com/user-attachments/assets/8376802a-bc8d-49ec-9123-fa24aee11c2a)




