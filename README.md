<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sidebar Test</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
    }

    /* Sidebar */
    .sidebar {
      height: 100%;
      width: 0;
      position: fixed;
      top: 0;
      left: 0;
      background-color: #111;
      overflow-x: hidden;
      transition: 0.3s;
      padding-top: 60px;
    }

    .sidebar a {
      padding: 10px 20px;
      text-decoration: none;
      font-size: 18px;
      color: #f1f1f1;
      display: block;
      transition: 0.2s;
    }

    .sidebar a:hover {
      background: #575757;
    }

    .sidebar .closebtn {
      position: absolute;
      top: 15px;
      right: 20px;
      font-size: 28px;
      cursor: pointer;
      color: white;
    }

    /* Open button */
    .openbtn {
      font-size: 18px;
      cursor: pointer;
      background-color: #111;
      color: white;
      padding: 10px 15px;
      border: none;
      position: fixed;
      top: 15px;
      left: 15px;
      border-radius: 5px;
    }

    .openbtn:hover {
      background-color: #444;
    }

    /* Content */
    .content {
      margin: 20px;
    }
  </style>
</head>
<body>

  <!-- Sidebar -->
  <div id="mySidebar" class="sidebar">
    <span class="closebtn" onclick="closeNav()">×</span>
    <a href="#">Homepage</a>
    <a href="#">Publications</a>
    <a href="#">Qualification</a>
  </div>

  <!-- Open Button -->
  <button class="openbtn" onclick="openNav()">☰ </button>

  <!-- Page Content -->
  <div class="content">
    <h1>Hello World</h1>
    <p>This is a minimal test page with a sidebar.</p>
  </div>

  <script>
    function openNav() {
      document.getElementById("mySidebar").style.width = "250px";
    }
    function closeNav() {
      document.getElementById("mySidebar").style.width = "0";
    }
  </script>
</body>
</html>

<div class="topnav">
  <a href="#">Home</a>
  <a href="#">Docs</a>
  <a href="#">Projects</a>
  <a href="#">Contact</a>
</div>

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Sidebar + Top Navbar</title>
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
    }

    /* Top horizontal navbar */
    .topnav {
      overflow: hidden;
      background-color: #333;
    }

    .topnav a {
      float: left;
      display: block;
      color: #f2f2f2;
      text-align: center;
      padding: 14px 20px;
      text-decoration: none;
    }

    .topnav a:hover {
      background-color: #575757;
      color: white;
    }

    /* Sidebar */
    .sidebar {
      height: 100%;
      width: 0;
      position: fixed;
      top: 0;
      left: 0;
      background-color: #111;
      overflow-x: hidden;
      transition: 0.3s;
      padding-top: 60px;
    }

    .sidebar a {
      padding: 10px 20px;
      text-decoration: none;
      font-size: 18px;
      color: #f1f1f1;
      display: block;
      transition: 0.2s;
    }

    .sidebar a:hover {
      background: #575757;
    }

    .sidebar .closebtn {
      position: absolute;
      top: 15px;
      right: 20px;
      font-size: 28px;
      cursor: pointer;
      color: white;
    }

    /* Sidebar open button */
    .openbtn {
      font-size: 18px;
      cursor: pointer;
      background-color: #111;
      color: white;
      padding: 10px 15px;
      border: none;
      position: fixed;
      top: 15px;
      left: 15px;
      border-radius: 5px;
    }

    .openbtn:hover {
      background-color: #444;
    }

    /* Page content */
    .content {
      margin: 20px;
    }
  </style>
</head>
<body>

  <!-- Horizontal Navbar -->
  <div class="topnav">
    <a href="#">Home</a>
    <a href="#">Docs</a>
    <a href="#">Projects</a>
    <a href="#">Contact</a>
  </div>

  <!-- Sidebar -->
  <div id="mySidebar" class="sidebar">
    <span class="closebtn" onclick="closeNav()">×</span>
    <a href="#">Extra 1</a>
    <a href="#">Extra 2</a>
    <a href="#">Extra 3</a>
  </div>

  <!-- Open Sidebar Button -->
  <button class="openbtn" onclick="openNav()">☰ Menu</button>

  <!-- Page Content -->
  <div class="content">
    <h1>Hello World</h1>
    <p>This is a page with both a top horizontal navbar and a sidebar.</p>
  </div>

  <script>
    function openNav() {
      document.getElementById("mySidebar").style.width = "250px";
    }
    function closeNav() {
      document.getElementById("mySidebar").style.width = "0";
    }
  </script>
</body>
</html>

