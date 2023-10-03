<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gildia ZABKA</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            margin: 0;
            padding: 0;
        }

        header {
            background-color: #000;
            color: #fff;
            text-align: center;
            padding: 20px;
        }

        nav {
            background-color: #777;
            color: #fff;
            text-align: center;
            padding: 10px;
        }

        nav ul {
            list-style-type: none;
            margin: 0;
            padding: 0;
        }

        nav ul li {
            display: inline;
            margin-right: 20px;
        }

        main {
            padding: 20px;
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 10px;
        }

        .tabs {
            display: flex;
            justify-content: center;
        }

        .tab-button {
            background-color: #333;
            color: #fff;
            padding: 10px 20px;
            margin: 5px;
            cursor: pointer;
        }

        .tab-content {
            display: none;
        }
    </style>
</head>
<body>
    <header>
        <h1>Gildia ZABKA</h1>
    </header>
    <nav>
        <ul>
            <li><a href="#">Oferujemy </a></li>
            <li><a href="#">O Nas</a></li>
            <li><a href="#">Awanse </a></li>
        </ul>
    </nav>
    <main>
        <div class="tabs">
            <button class="tab-button" onclick="openTab(event, 'tab1')">Oferujemy</button>
            <button class="tab-button" onclick="openTab(event, 'tab2')">O Nas</button>
            <button class="tab-button" onclick="openTab(event, 'tab3')">Awanse</button>
        </div>
        <div id="tab1" class="tab-content">
            <h2>Oferujemy</h2>
            <p>Miła atmosfere, wspulne przebijanie, klepy, full cuboid dobre zabezpieczenia i wiele wiecej  </p>
        </div>
        <div id="tab2" class="tab-content">
            <h2>Coś o nas</h2>
            <p>Ogarnaimy pvp suzkamy obecnie czlonkow do gildi mili pomagany dajemy itemy </p>
        </div>
        <div id="tab3" class="tab-content">
            <h2>Informacje o Awansach</h2>
            <p>Tu beda sie pojawiac informacje o awansach 
               dajemy awans za 2tygodniową aktywnosc :)
            </p>
        </div>
    </main>
    <footer>
    </footer>

    <script>
   function openTab(evt, tabName) {
            var i, tabContent, tabButton;

            tabContent = document.getElementsByClassName("tab-content");
            for (i = 0; i < tabContent.length; i++) {
                tabContent[i].style.display = "none";
            }

            tabButton = document.getElementsByClassName("tab-button");
            for (i = 0; i < tabButton.length; i++) {
                tabButton[i].style.backgroundColor = "#555";
            }

            document.getElementById(tabName).style.display = "block";
            evt.currentTarget.style.backgroundColor = "#333";
        }

        // Otwarcie domyślnej zakładki
        document.getElementById("tab1").style.display = "block";
    </script>
</body>
</html>
