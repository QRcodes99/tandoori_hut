<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Materials</title>
    <style>
        body {
            font-family: Arial, sans-serif;
        }
        section {
            position: relative; /* Needed for absolute positioning */
            padding: 20px;
            margin: 10px;
            border: 2px solid black;
            border-radius: 5px;
            cursor: pointer;
        }
        .section {
            background-color: lightblue;
        }
        .details {
            display: none; /* Initially hidden */
            margin-top: 10px;
            padding: 10px;
            background: white;
            border: 1px solid black;
            border-radius: 5px;
        }
        img {
            max-width: 100%;
            height: auto;
            border-radius: 5px;
        }
        .best {
            font-size: 18px;
            font-weight: bold;
            color: red;
        }
        .click-here {
            position: absolute;
            top: 10px;
            right: 10px;
            background: red;
            color: white;
            padding: 5px 10px;
            font-size: 12px;
            border-radius: 5px;
        }
        /* Popup Styling */
        .popup {
            position: fixed;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 60%;
            max-width: 500px;
            background: white;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.3);
            padding: 20px;
            text-align: center;
            border-radius: 10px;
            display: none;
            max-height: 90vh;
            overflow: auto;
            z-index: 1000;
        }
        .popup img {
            width: 100%;
            max-height: 70vh;
            border-radius: 10px;
            display: block;
            margin: 0 auto;
        }
        .popup button {
            margin-top: 15px;
            padding: 10px 20px;
            background-color: #ff6600;
            border: none;
            color: white;
            font-size: 16px;
            cursor: pointer;
            border-radius: 5px;
            display: block;
            width: 100%;
        }
        .popup button:hover {
            background-color: #cc5200;
        }


    </style>
</head>
<body>

 <!-- Popup -->
    <div class="popup" id="welcomePopup">
    <h2><b>WELCOME TO TANDOORI HUT!</b></h2> 
        <img src="https://i.postimg.cc/x1PD4LnG/Screenshot-16-3-2025-232126.jpg">
        <button onclick="closePopup()">Close</button>
    </div>

    <script>
        window.onload = function() {
            document.getElementById("welcomePopup").style.display = "block";
        };

        function closePopup() {
            document.getElementById("welcomePopup").style.display = "none";
        }
    </script>


    <h2 style="text-align: center;">TANDOORI HUT</h2>

    <section class="section" onclick="toggleDetails('section1')">
        <span class="click-here">Click Here</span>
        <h2>INDIAN CUISINE(VEG.)</h2>
        <div id="section1" class="details">
        <div <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Indian Cuisine (Veg.) - Tandoori Hut</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            text-align: center;
        }
        .menu-container {
            width: 80%;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px gray;
        }
        h1 {
            color: #d9534f;
        }
        .menu-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            border-bottom: 1px solid #ddd;
            padding: 10px;
        }
        .menu-item img {
            width: 60px;
            height: 60px;
            border-radius: 10px;
            object-fit: cover;
        }
        .item-name {
            flex: 1;
            text-align: left;
            padding-left: 10px;
        }
        .price {
            font-weight: bold;
            color: #d9534f;
        }
    </style>
</head>
<body>
    <div class="menu-container">
        <h1>INDIAN CUISINE (VEG.)</h1>

        <div class="menu-item">
            <img src="https://i.postimg.cc/V6y5F3K8/kadai-paner.jpg" alt="Kadai Paneer">
            <div class="item-name">Kadai Paneer</div>
            <div class="price">₹250</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/kGp0QdyN/shahi-paner.jpg" alt="Shahi Paneer">
            <div class="item-name">Shahi Paneer</div>
            <div class="price">₹280</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/TPf4Ww6M/paner-labadar.jpg" alt="Paneer Labadar">
            <div class="item-name">Paneer Labadar</div>
            <div class="price">₹280</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/GtGfysHR/malai-kofta.jpg" alt="Malai Kofta">
            <div class="item-name">Malai Kofta</div>
            <div class="price">₹280</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/3NjTHqj2/paner-buter-masala.jpg" alt="Paneer Butter Masala">
            <div class="item-name">Paneer Butter Masala</div>
            <div class="price">₹280</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/50wGHCHV/paner-do-payaza.jpg" alt="Paneer Do Pyaza">
            <div class="item-name">Paneer Do Pyaza</div>
            <div class="price">₹280</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/hvZ0hD0n/paner-burji.jpg" alt="Paneer Bhurji">
            <div class="item-name">Paneer Bhurji</div>
            <div class="price">₹320</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/HWrzP5Ws/matar-paner.jpg" alt="Mattar Paneer">
            <div class="item-name">Mattar Paneer</div>
            <div class="price">₹280</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/9F8WX65B/chana-masala-recipe.jpg" alt="Chana Masala">
            <div class="item-name">Chana Masala</div>
            <div class="price">₹200</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/x12W2gqP/dum-alo.jpg" alt="Dum Aalu Kashmiri">
            <div class="item-name">Dum Aalu Kashmiri</div>
            <div class="price">₹240</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/zvYkgtst/jeera-alu.jpg" alt="Jeera Aalu">
            <div class="item-name">Jeera Aalu</div>
            <div class="price">₹160</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/GmDhMXVJ/mix-veh.jpg" alt="Mixed Veg">
            <div class="item-name">Mixed Veg</div>
            <div class="price">₹250</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/d3zcrYsM/mashrom-masala.jpg" alt="Mushroom Masala">
            <div class="item-name">Mushroom Masala</div>
            <div class="price">₹270</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/JnHLn083/veg-kofta.jpg" alt="Veg Kofta">
            <div class="item-name">Veg Kofta</div>
            <div class="price">₹280</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/85M096DY/mashrom-do-paya.jpg" alt="Mushroom Do Pyaza">
            <div class="item-name">Mushroom Do Pyaza</div>
            <div class="price">₹280</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/nrMQMvzR/mashrom-matar.jpg" alt="Mushroom Matar">
            <div class="item-name">Mushroom Matar</div>
            <div class="price">₹270</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/c4wf3Bh2/dal-makhkoojgt.jpg" alt="Dal Makhni">
            <div class="item-name">Dal Makhni</div>
            <div class="price">₹240</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/fTzM7wfs/yellow.jpg" alt="Yellow Dal">
            <div class="item-name">Yellow Dal</div>
            <div class="price">₹220</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/1XW2rZyR/fry-dal.jpg" alt="Dal Fry">
            <div class="item-name">Dal Fry</div>
            <div class="price">₹220</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/BbyNvZqF/chap-tikka.jpg" alt="Champ Tikka Butter Masala">
            <div class="item-name">Champ Tikka Butter Masala</div>
            <div class="price">₹320</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/sDGC4vGt/paneer-tikka-buter-masaa.jpg" alt="paneer Tikka Butter Masala">
            <div class="item-name">Paneer Tikka Butter Masala</div>
            <div class="price">₹350</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/vThRcV4K/tawa-champ.jpg" alt="Tawa Champ">
            <div class="item-name">Tawa Champ</div>
            <div class="price">₹280</div>
        </div>
    </div>
</body>
</html> >   
            <p></p>

        </div>
    </section>

    <section class="section" onclick="toggleDetails('section2')">
        <span class="click-here">Click Here</span>
        <h2>COMBO+BEVERAGE HOT+SHAKES</h2>
        <div id="section2" class="details">
        <div <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            text-align: center;
        }
        .menu-container {
            width: 80%;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #d32f2f;
        }
        .menu-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px;
            border-bottom: 1px solid #ddd;
        }
        .menu-item img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 10px;
        }
        .menu-text {
            flex-grow: 1;
            padding: 0 20px;
            text-align: left;
        }
        .price {
            font-weight: bold;
            color: #d32f2f;
        }
    </style>
</head>
<body>
    <div class="menu-container">
        <h1>Menu</h1>

        <h2>COMBO</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/kXhpch1j/puri-chana.jpg" alt="Puri Chana"><div class="menu-text">Puri + Chana + Salad</div><div class="price">120/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/FsJjMWFC/chole-bhat.jpg" alt="Chole Bhatura"><div class="menu-text">Chole + Bhatura + Chatni + Salad</div><div class="price">120/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/G3TKRhqj/alu-nan.jpg" alt="Aalu Naan"><div class="menu-text">Aalu Naan + Chana + Chatni + Salad</div><div class="price">130/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/kX9bHnZG/mix-veg-nan.jpg" alt="Mix Veg Naan"><div class="menu-text">Mix Veg. Naan + Chana + Chatni + Salad</div><div class="price">150/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/mDfDFjWk/panner-nan.jpg" alt="Paneer Naan"><div class="menu-text">Paneer Naan + Chana + Chatni + Salad</div><div class="price">180/-</div></div>
        
        <h2>BEVERAGE HOT</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/BvNYjYKc/tea.jpg" alt="Tea"><div class="menu-text">Tea</div><div class="price">20/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/tgmcrv4R/ginger-tea.jpg" alt="Ginger Lemon Honey Tea"><div class="menu-text">Ginger Lemon Honey Tea</div><div class="price">60/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/9Mdt9Y1b/cofi.png"><div class="menu-text">Hot Coffee</div><div class="price">50/-</div></div>
        
        <h2>BEVERAGE COLD</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/D0zHBVqz/cold-cofie.jpg" alt="Cold Coffee"><div class="menu-text">Cold Coffee</div><div class="price">120/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/Z5kZKR8F/cofie-icecream.jpg" alt="Cold Coffee With Ice Cream"><div class="menu-text">Cold Coffee With Ice Cream</div><div class="price">140/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/SKPb3xxM/lasi.jpg" alt="Lassi"><div class="menu-text">Lassi (Sweet/Sour)</div><div class="price">70/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/htH0YFqG/soda.jpg" alt="Lemon Soda"><div class="menu-text">Lemon Soda</div><div class="price">50/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/8zDMVGzK/cold-drink.jpg" alt="Cold Drinks"><div class="menu-text">Cold Drinks (Glass)</div><div class="price">30/-</div></div>
        
        <h2>SHAKES</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/mZRdVvQw/bana.jpg" alt="Banana Shake"><div class="menu-text">Banana Shake</div><div class="price">100/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/50ZC0YwJ/mango.jpg" alt="Mango Shake"><div class="menu-text">Mango Shake</div><div class="price">120/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/nhzcyVDG/choclat.jpg" alt="Chocolate Shake"><div class="menu-text">Chocolate Shake</div><div class="price">120/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/MH9J5Rd2/oreo.jpg" alt="Oreo Shake"><div class="menu-text">Oreo Shake</div><div class="price">120/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/qv8jd0Hg/apple.jpg" alt="Apple Shake"><div class="menu-text">Apple Shake</div><div class="price">130/-</div></div>
    </div>
</body>
</html>
>
            <p></p>
            
        </div>
    </section>

    <section class="section" onclick="toggleDetails('section3')">
        <span class="click-here">Click Here</span>
        <h2>FAST FOOD I</h2>
        <div id="section3" class="details">
        <div <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fast Food Menu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            text-align: center;
        }
        .menu-container {
            width: 80%;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #d32f2f;
        }
        .menu-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px;
            border-bottom: 1px solid #ddd;
        }
        .menu-item img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 10px;
        }
        .menu-text {
            flex-grow: 1;
            padding: 0 20px;
            text-align: left;
        }
        .price {
            font-weight: bold;
            color: #d32f2f;
        }
    </style>
</head>
<body>

    <div class="menu-container">
        <h1>Fast Food Menu</h1>

        <div class="menu-item">
            <img src="https://i.postimg.cc/DwHbvpLD/white-pasta.jpg" alt="White Sauce Pasta">
            <div class="menu-text">White Sauce Pasta</div>
            <div class="price">180/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/bJzYp1CW/reds-pasta.jpg" alt="Red Sauce Pasta">
            <div class="menu-text">Red Sauce Pasta</div>
            <div class="price">150/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/GtfbFVLn/white-so-chiken-pasta.jpg" alt="White Sauce Chicken Pasta">
            <div class="menu-text">White Sauce Chicken Pasta</div>
            <div class="price">250/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/pT4283Xb/red-souse-chiken.jpg" alt="Red Sauce Chicken Pasta">
            <div class="menu-text">Red Sauce Chicken Pasta</div>
            <div class="price">220/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/8kfkDkt1/veg-manchur.jpg" alt="Veg Manchurian">
            <div class="menu-text">Veg Manchurian (10 pc)</div>
            <div class="price">180/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/mr3MmN15/manchurian-gravy.jpg" alt="Veg Manchurian With Gravy">
            <div class="menu-text">Veg Manchurian With Gravy (10 pc)</div>
            <div class="price">220/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/Kj782JF6/chiuiken-manchurian.jpg" alt="Chicken Manchurian">
            <div class="menu-text">Chicken Manchurian (10 pc)</div>
            <div class="price">250/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/W1Fxqtq3/chiken-manchurian-gravy.jpg" alt="Chicken Manchurian With Gravy">
            <div class="menu-text">Chicken Manchurian With Gravy (10 pc)</div>
            <div class="price">290/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/25PWj9Ry/cryspy-veg.jpg" alt="Crispy Veg">
            <div class="menu-text">Crispy Veg</div>
            <div class="price">150/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/SNyMKz56/chiken-fry-rice.jpg" alt="Chicken Fried Rice">
            <div class="menu-text">Chicken Fried Rice</div>
            <div class="price">200/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/W4Pj20Yj/egg-fry-rice.jpg" alt="Egg Fried Rice">
            <div class="menu-text">Egg Fried Rice</div>
            <div class="price">180/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/bvTXpW2H/veg-fried-rice.jpg" alt="Veg Fried Rice">
            <div class="menu-text">Veg Fried Rice</div>
            <div class="price">180/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/yYbcr8Q0/tiki-burger.jpg" alt="Tikki Burger">
            <div class="menu-text">Tikki Burger</div>
            <div class="price">70/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/mrGc0zQ1/chese-burger.jpg" alt="Cheese Burger">
            <div class="menu-text">Cheese Burger</div>
            <div class="price">100/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/sXg2rp1x/chese-chily.jpg" alt="Cheese Chilly">
            <div class="menu-text">Cheese Chilly</div>
            <div class="price">250/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/Fz2F38pk/chese-finger.jpg" alt="Cheese Finger">
            <div class="menu-text">Cheese Finger</div>
            <div class="price">250/-</div>
        </div>

        <div class="menu-item">
            <img src="https://i.postimg.cc/4NfRFJ74/madhjikhesd.jpg" alt="Mushroom Chilly">
            <div class="menu-text">Mushroom Chilly</div>
            <div class="price">250/-</div>
        </div>

    </div>

</body>
</html> >
   <p></p>
            
        </div>
    </section>

    <section class="section" onclick="toggleDetails('section4')">
        <span class="click-here">Click Here</span>
        <h2>FAST FOOD II</h2>
        
<div id="section4" class="details">
<div <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fast Food Menu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            text-align: center;
        }
        .menu-container {
            width: 80%;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #d32f2f;
        }
        .menu-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px;
            border-bottom: 1px solid #ddd;
        }
        .menu-item img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 10px;
        }
        .menu-text {
            flex-grow: 1;
            padding: 0 20px;
            text-align: left;
        }
        .price {
            font-weight: bold;
            color: #d32f2f;
        }
    </style>
</head>
<body>

    <div class="menu-container">
        <h1>Fast Food Menu</h1>

        <div class="menu-item"><img src="https://i.postimg.cc/HkFfCN9j/veg-dpring.jpg" alt="Veg. Spring Roll"><div class="menu-text">Veg. Spring Roll</div><div class="price">120/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/SK8HQGgd/paner-rol.jpg" alt="Paneer Spring Roll"><div class="menu-text">Paneer Spring Roll</div><div class="price">170/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/d372v5Bt/chiken-rol.jpg" alt="Chicken Spring Roll"><div class="menu-text">Chicken Spring Roll</div><div class="price">200/-</div></div>
        
        <div class="menu-item"><img src="https://i.postimg.cc/Qx16TMQN/veg-kathi-rol.jpg" alt="Veg. Kathi Roll"><div class="menu-text">Veg. Kathi Roll</div><div class="price">100/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/8c5SC6JC/panner-kathi-rol.jpg" alt="Paneer Kathi Roll"><div class="menu-text">Paneer Kathi Roll</div><div class="price">130/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/9FD25yH8/chuiken-kathi-rol.jpg" alt="Chicken Kathi Roll"><div class="menu-text">Chicken Kathi Roll</div><div class="price">150/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/kXbHvsmm/chiken-tika-rol.jpg" alt="Chicken Tikka Roll"><div class="menu-text">Chicken Tikka Roll</div><div class="price">200/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/yNvp8rFF/paner-tika-rol.jpg" alt="Paneer Tikka Roll"><div class="menu-text">Paneer Tikka Roll</div><div class="price">150/-</div></div>
        
        <div class="menu-item"><img src="https://i.postimg.cc/wjFn1vzy/veg-momo-steam.jpg" alt="Veg. Steamed Momos"><div class="menu-text">Veg. Steamed Momos</div><div class="price">70/- , 100/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/Cxv6FQCb/fry-momo.jpg" alt="Veg. Fried Momos"><div class="menu-text">Veg. Fried Momos</div><div class="price">80/- , 120/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/xCgX7LVj/kurkura-momo.jpg" alt="Kurkure Momos"><div class="menu-text">Kurkure Momos</div><div class="price">160/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/5NXX7H71/veg-tandori-momo.jpg" alt="Veg. Tandoori Momos"><div class="menu-text">Veg. Tandoori Momos</div><div class="price">170/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/c4fvGqS5/chiken-steam-momo.jpg" alt="Chicken Steamed Momos"><div class="menu-text">Chicken Steamed Momos</div><div class="price">100/- , 150/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/Qt53K3S2/chiken-tandori-momo.jpg" alt="Chicken Tandoori Momos"><div class="menu-text">Chicken Tandoori Momos</div><div class="price">200/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/k4W0Xyg9/chiken-fry-nmomo.jpg" alt="Chicken Fry Momos"><div class="menu-text">Chicken Fry Momos</div><div class="price">120/- , 170/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/y6gjMT8r/veg-pan-momo.jpg" alt="Veg. Pan Momos"><div class="menu-text">Veg. Pan Momos</div><div class="price">190/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/vmZL3rKh/chiken-poan-momo.jpg" alt="Chicken Pan Momos"><div class="menu-text">Chicken Pan Momos</div><div class="price">240/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/g0hk9512/veg-noodle.jpg" alt="Veg. Noodles"><div class="menu-text">Veg. Noodles</div><div class="price">70/- , 100/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/zvzJgfvy/egg-noodle.jpg" alt="Egg Noodles"><div class="menu-text">Egg Noodles</div><div class="price">90/- , 130/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/CMnyckTw/chikenm-noodle.jpg" alt="Chicken Noodles"><div class="menu-text">Chicken Noodles</div><div class="price">120/- , 170/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/gkyT7KMb/thupka.jpg" alt="Thupka"><div class="menu-text">Thupka</div><div class="price">100/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/gkyT7KMb/thupka.jpg" alt="Chicken Thupka"><div class="menu-text">Chicken Thupka</div><div class="price">140/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/zBgrHgqD/french-fries.jpg" alt="French Fries"><div class="menu-text">French Fries</div><div class="price">130/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/x1pDsRCT/chillinpotato.jpg" alt="Chilli Potato"><div class="menu-text">Chilli Potato</div><div class="price">150/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/Gh35Zy6B/crispy-potato.jpg" alt="Crispy Honey Chilli Potato"><div class="menu-text">Crispy Honey Chilli Potato</div><div class="price">190/-</div></div>
    </div>

</body>
</html>
 >       
     <p></p>
           
        </div>
    </section>

    <section class="section" onclick="toggleDetails('section5')">
        <span class="click-here">Click Here</span>
        <h2>PIZZA MENU</h2>
        <div id="section5" class="details">
        <div <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pizza Menu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            text-align: center;
        }
        .menu-container {
            width: 80%;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #d32f2f;
        }
        .menu-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px;
            border-bottom: 1px solid #ddd;
        }
        .menu-item img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 10px;
        }
        .menu-text {
            flex-grow: 1;
            padding: 0 20px;
            text-align: left;
        }
        .price {
            font-weight: bold;
            color: #d32f2f;
        }
    </style>
</head>
<body>
    <div class="menu-container">
        <h1>Pizza Menu</h1>
        
        <h2>Veg Pizza</h2>
        <div class="menu-item">
            <img src="https://i.postimg.cc/v82GfZLn/margretta-cheze-piza.jpg" alt="Margretta Cheese Pizza">
            <div class="menu-text">Margretta Cheese Pizza</div>
            <div class="price">250/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/MHn2d1bQ/veg-piza.jpg" alt="Veg Pizza">
            <div class="menu-text">Veg Pizza</div>
            <div class="price">300/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/V6N3kXhV/from-fresh-piza.jpg" alt="Form Fresh Pizza">
            <div class="menu-text">Form Fresh Pizza</div>
            <div class="price">350/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/hvvtW1WV/paner-piza.jpg" alt="Paneer Lover Pizza">
            <div class="menu-text">Paneer Lover Pizza</div>
            <div class="price">400/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/ZqjmbvLH/veg-delight-piza.jpg" alt="Veg Delight Pizza">
            <div class="menu-text">Veg Delight Pizza</div>
            <div class="price">450/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/c4YrsTtc/chese-corn-piza.jpg" alt="Cheese Corn Pizza">
            <div class="menu-text">Cheese Corn Pizza</div>
            <div class="price">400/-</div>
        </div>
        <h3>Extra Cheese: 50/-</h3>
        
        <h2>Non-Veg Pizza</h2>
        <div class="menu-item">
            <img src="https://i.postimg.cc/QxLckFp0/chiken-chese-piza.jpg" alt="Chicken Cheese Pizza">
            <div class="menu-text">Chicken Cheese Pizza</div>
            <div class="price">400/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/02xbyDGR/nonveg-delight-piza.jpg" alt="Non-Veg Delight Pizza">
            <div class="menu-text">Non-Veg Delight Pizza</div>
            <div class="price">450/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/JnZz1zGz/indiapiza.jpg" alt="Indian Pizza">
            <div class="menu-text">Indian Pizza (Paneer & Chicken)</div>
            <div class="price">500/-</div>
        </div>
        
        <h2>Desserts</h2>
        <div class="menu-item">
            <img src="https://i.postimg.cc/XJCk4dfB/ice-cream.jpg" alt="Ice Cream">
            <div class="menu-text">Ice Cream</div>
            <div class="price">60/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/PJbb8HFt/glulab-jamun.jpg" alt="Gulab Jamun">
            <div class="menu-text">Gulab Jamun (2pc)</div>
            <div class="price">60/-</div>
        </div>
    </div>
</body>
</html>
 >   
 <p></p>
            
        </div>
    </section>

    <section class="section" onclick="toggleDetails('section6')">
        <span class="click-here">Click Here</span>
        <h2>BREAKFAST</h2>
        <div id="section6" class="details">
        <div <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            text-align: center;
        }
        .menu-container {
            width: 80%;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #d32f2f;
        }
        .menu-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px;
            border-bottom: 1px solid #ddd;
        }
        .menu-item img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 10px;
        }
        .menu-text {
            flex-grow: 1;
            padding: 0 20px;
            text-align: left;
        }
        .price {
            font-weight: bold;
            color: #d32f2f;
        }
    </style>
</head>
<body>
    <div class="menu-container">
        <h1>Menu</h1>
        <h2>BREAKFAST</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/8zkQyBWH/alu-parantha.jpg" alt="Aalu Parantha"><div class="menu-text">Aalu Parantha</div><div class="price">60/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/k5Z0X0H1/panner-parantha.jpg" alt="Paneer Parantha"><div class="menu-text">Paneer Parantha</div><div class="price">80/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/MppN0Z23/gobi-parantha.jpg" alt="Gobi Parantha"><div class="menu-text">Gobi Parantha</div><div class="price">60/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/qMjZ7fhs/mixed-parantha.jpg" alt="Mixed Parantha"><div class="menu-text">Mixed Parantha</div><div class="price">70/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/hPvPvBZg/plain-omlete.jpg" alt="Plain Omelette"><div class="menu-text">Plain Omelette</div><div class="price">50/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/QNyZ6WSG/veg-sandwitch.jpg" alt="Veg Sandwich"><div class="menu-text">Veg Sandwich</div><div class="price">90/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/KvtFR876/maggi.jpg" alt="Maggi"><div class="menu-text">Maggi</div><div class="price">60/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/cCHgd88G/panneer-maggi.jpg" alt="Paneer Maggi"><div class="menu-text">Paneer Maggi</div><div class="price">120/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/VNV2KxB9/chiken-maggi.jpg" alt="Chicken Maggi"><div class="menu-text">Chicken Maggi</div><div class="price">150/-</div></div>
        <h2>RICE</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/jj7Bk88G/plain-rice.jpg" alt="Plain Rice"><div class="menu-text">Plain Rice</div><div class="price">130/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/m2gJGZX3/jeera-rice.jpg" alt="Jeera Rice"><div class="menu-text">Jeera Rice</div><div class="price">150/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/c1XkTyxv/lemmon-rice.jpg" alt="Lemon Rice"><div class="menu-text">Lemon Rice</div><div class="price">170/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/CKZVpG7V/peas.jpg" alt="Peas Pulao"><div class="menu-text">Peas Pulao</div><div class="price">180/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/ZnSBXKr6/veg-pulao.jpg" alt="Veg Pulao"><div class="menu-text">Veg Pulao</div><div class="price">200/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/k4rBtXYL/biryani.jpg" alt="Veg Biryani"><div class="menu-text">Veg Biryani</div><div class="price">280/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/Nj5MJrWW/chiken-biryani.jpg" alt="Chicken Biryani"><div class="menu-text">Chicken Biryani</div><div class="price">380/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/j2Hgr5BT/egg-biryani.jpg" alt="Egg Biryani"><div class="menu-text">Egg Biryani</div><div class="price">300/-</div></div>
    </div>
</body>
</html>
 >  
  <p></p>
   </div>
    </section>

    <section class="section" onclick="toggleDetails('section7')">
        <span class="click-here">Click Here</span>
        <h2>SALAD + EXTRA</h2>
        <div id="section7" class="details">
        <div <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            text-align: center;
        }
        .menu-container {
            width: 80%;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #d32f2f;
        }
        .menu-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px;
            border-bottom: 1px solid #ddd;
        }
        .menu-item img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 10px;
        }
        .menu-text {
            flex-grow: 1;
            padding: 0 20px;
            text-align: left;
        }
        .price {
            font-weight: bold;
            color: #d32f2f;
        }
    </style>
</head>
<body>

    <div class="menu-container">
        <h1>Menu</h1>

        <h2>SALAD</h2>
        <div class="menu-item">
            <img src="https://i.postimg.cc/dV7mK3by/green-sald.jpg" alt="Green Salad">
            <div class="menu-text">Green Salad</div>
            <div class="price">80/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/Gpd2xSxm/kachumber.jpg" alt="Kachumber Salad">
            <div class="menu-text">Kachumber Salad</div>
            <div class="price">80/-</div>
        </div>

        <h2>EXTRA</h2>
        <div class="menu-item">
            <img src="https://i.postimg.cc/KjDFjmC7/curd-simple.jpg" alt="Curd">
            <div class="menu-text">Curd</div>
            <div class="price">90/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/tgb0csJX/curd.jpg" alt="Mix Raita">
            <div class="menu-text">Mix Raita</div>
            <div class="price">100/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/FHj80hZw/boondi-raita.jpg" alt="Boondi Raita">
            <div class="menu-text">Boondi Raita</div>
            <div class="price">90/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/g2N5gNCK/papad.jpg" alt="Papad">
            <div class="menu-text">Papad</div>
            <div class="price">15/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/NfrjqrsT/fried-papad.jpg" alt="Fried Papad">
            <div class="menu-text">Fried Papad</div>
            <div class="price">20/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/8k76cckk/masala-papad.jpg" alt="Masala Papad">
            <div class="menu-text">Masala Papad</div>
            <div class="price">50/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/9090p4zG/peanut-masala.jpg" alt="Peanut Masala">
            <div class="menu-text">Peanut Masala</div>
            <div class="price">150/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/JzpXtkXn/chana-chat.jpg" alt="Chana Chaat">
            <div class="menu-text">Chana Chaat</div>
            <div class="price">120/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/GhGwcFZF/alu-chana-chat.jpg" alt="Aalu Chana Chaat">
            <div class="menu-text">Aalu Chana Chaat</div>
            <div class="price">150/-</div>
        </div>
        <div class="menu-item">
            <img src="https://i.postimg.cc/dtmHH4bx/water.jpg" alt="Mineral Water">
            <div class="menu-text">Mineral Water</div>
            <div class="price">20/-</div>
        </div>
    </div>

</body>
</html>
  > 
   <p></p>
            
        </div>
    </section>

    <section class="section" onclick="toggleDetails('section8')">
        <span class="click-here">Click Here</span>
        <h2>TANDOORI SNACKS & SOUPS MENU</h2>
       
 <div id="section8" class="details">
<div <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            text-align: center;
        }
        .menu-container {
            width: 80%;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #d32f2f;
        }
        .menu-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px;
            border-bottom: 1px solid #ddd;
        }
        .menu-item img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 10px;
        }
        .menu-text {
            flex-grow: 1;
            padding: 0 20px;
            text-align: left;
        }
        .price {
            font-weight: bold;
            color: #d32f2f;
        }
    </style>
</head>
<body>
    <div class="menu-container">
        <h1>Tandoori Snacks & Soups Menu</h1>
        <h2>TANDOORI SNACKS (NON-VEG.)</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/xdfKRNBr/tandoori-hiken.jpg" alt="Tandoori Chicken"><div class="menu-text">Tandoori Chicken (Half)</div><div class="price">240/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/xdfKRNBr/tandoori-hiken.jpg" alt="Tandoori Chicken"><div class="menu-text">Tandoori Chicken (Full)</div><div class="price">450/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/2jsnfCK5/chiken-tikka.jpg" alt="Chicken Tikka"><div class="menu-text">Chicken Tikka (10 pcs)</div><div class="price">300/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/J4HKbT9s/afgani-chhiken.jpg" alt="Afghani Chicken"><div class="menu-text">Afghani Chicken (Half)</div><div class="price">250/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/J4HKbT9s/afgani-chhiken.jpg" alt="Afghani Chicken"><div class="menu-text">Afghani Chicken (Full)</div><div class="price">480/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/mkz3yDpv/crispy-chiken-fry.jpg" alt="Crispy Chicken Fry"><div class="menu-text">Crispy Chicken Fry (10 pcs)</div><div class="price">320/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/65H2pwHR/chiken-fry.jpg" alt="Chicken Fry"><div class="menu-text">Chicken Fry (Half)</div><div class="price">300/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/65H2pwHR/chiken-fry.jpg" alt="Chicken Fry"><div class="menu-text">Chicken Fry (Full)</div><div class="price">550/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/pXdr742d/chiken-malai-tukka.jpg" alt="Chicken Malai Tikka"><div class="menu-text">Chicken Malai Tikka (10 pcs)</div><div class="price">360/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/8CCVPQ0F/irani-chiken.jpg" alt="Irani Chicken"><div class="menu-text">Irani Chicken (10 pcs)</div><div class="price">370/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/2S2Pt9SC/chiken-tangiri.jpg" alt="Chicken Tangri"><div class="menu-text">Chicken Tangri (6 pcs)</div><div class="price">500/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/d0CjCDXg/chiken-sheekh-kabab.jpg" alt="Chicken Sheekh Kabab"><div class="menu-text">Chicken Sheekh Kabab</div><div class="price">300/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/gJqyMQGD/fry-fish.jpg" alt="Fish Fry"><div class="menu-text">Fish Fry (Half)</div><div class="price">300/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/gJqyMQGD/fry-fish.jpg" alt="Fish Fry"><div class="menu-text">Fish Fry (Full)</div><div class="price">550/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/rmnsFNjT/fish-tikka.jpg" alt="Fish Tikka"><div class="menu-text">Fish Tikka (8 pcs)</div><div class="price">350/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/cLSnzT5k/nion-veg-platter.jpg" alt="Non-Veg Platter"><div class="menu-text">Non-Veg Platter</div><div class="price">500/-</div></div>
        <h2>SOUPS</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/HxDD0cLM/tomato-sou.jpg" alt="Tomato Soup"><div class="menu-text">Tomato Soup</div><div class="price">80/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/QCd6chc5/veg-machorian-soup.jpg" alt="Veg Manchow Soup"><div class="menu-text">Veg. Manchow Soup</div><div class="price">90/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/7694xPxT/chiken-manchow-soop.jpg" alt="Chicken Manchow Soup"><div class="menu-text">Chicken Manchow Soup</div><div class="price">150/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/mkP50Th4/veg-hot.jpg" alt="Veg Hot & Sour Soup"><div class="menu-text">Veg. Hot & Sour Soup</div><div class="price">80/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/9X9StQ3P/chiken-hot.jpg" alt="Chicken Hot & Sour Soup"><div class="menu-text">Chicken Hot & Sour Soup</div><div class="price">150/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/RFLt4t6Q/veg-sw-eat-corn-soup.jpg" alt="Veg Sweet Corn Soup"><div class="menu-text">Veg. Sweet Corn Soup</div><div class="price">120/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/jjXqj4c5/chiken-corn-soup.jpgS" alt="Chicken Sweet Corn Soup"><div class="menu-text">Chicken Sweet Corn Soup</div><div class="price">180/-</div></div>
    </div>
</body>
</html>
 > 
           <p>\</p>
            
        </div>
    </section>

    <section class="section" onclick="toggleDetails('section9')">
        <span class="click-here">Click Here</span>
        <h2>RESTAURANT MENU I</h2>
        <div id="section9" class="details">
         <div <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Menu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            text-align: center;
        }
        .menu-container {
            width: 80%;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #d32f2f;
        }
        h2 {
            color: #333;
        }
        .menu-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px;
            border-bottom: 1px solid #ddd;
        }
        .menu-item img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 10px;
        }
        .menu-text {
            flex-grow: 1;
            padding: 0 20px;
            text-align: left;
        }
        .price {
            font-weight: bold;
            color: #d32f2f;
        }
    </style>
</head>
<body>
    <div class="menu-container">
        <h1>Restaurant Menu</h1>
        
        <h2>CHINESE (NON-VEG.)</h2>
        <div class="menu-item"><img scr="https://i.postimg.cc/t4PRPjqY/chili-chiken.jpg" alt="Chilli Chicken"><div class="menu-text">Chilli Chicken (Half/Full)</div><div class="price">300/- | 500/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/YSzpnzm7/schezwan-chiken.jpg" alt="Schezwan Chicken"><div class="menu-text">Schezwan Chicken</div><div class="price">300/- | 500/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/gJjfVVVN/grlic-chiken.jpg" alt="Garlic Chicken"><div class="menu-text">Garlic Chicken (Half/Full)</div><div class="price">300/- | 500/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/xjz9BQmg/chicken-black-pepper.jpg" alt="Chicken Black Pepper"><div class="menu-text">Chicken Black Pepper (Half/Full)</div><div class="price">300/- | 500/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/2S2Pt9SC/chiken-tangiri.jpg" alt="Lemon Chicken"><div class="menu-text">Lemon Chicken (Half/Full)</div><div class="price">300/- | 500/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/DfBckVKJ/chiken-lolipop.jpg" alt="Chicken Lollipop"><div class="menu-text">Chicken Lollipop (8 pcs)</div><div class="price">360/-</div></div>
        
        <h2>TANDOORI SNACKS (VEG.)</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/ydJZSNN2/paneer-tikka.jpg" alt="Paneer Tikka"><div class="menu-text">Paneer Tikka</div><div class="price">290/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/jd6Jfmsq/paner-malai-tikka.jpg" alt="Paneer Malai Tikka"><div class="menu-text">Paneer Malai Tikka</div><div class="price">320/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/SxWVJDPc/veg-sheekhkabab.jpg" alt="Veg Sheekh Kabab"><div class="menu-text">Veg. Sheekh Kabab</div><div class="price">180/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/ryKBK2NW/veg-pakoda.jpg" alt="Veg Pakora"><div class="menu-text">Veg. Pakora</div><div class="price">100/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/Z5Tjvrzg/mix-pakora.jpg" alt="Mix Pakora"><div class="menu-text">Mix Pakora</div><div class="price">150/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/Px8Mny1L/panner-pakoda.jpg" alt="Paneer Pakora"><div class="menu-text">Paneer Pakora</div><div class="price">190/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/D0vmPyf2/masala-champ-tandori.jpg" alt="Tandoori Masala Champ"><div class="menu-text">Tandoori Masala Champ</div><div class="price">200/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/43pdChmf/tandor-malai-champ.jpg" alt="Tandoori Malai Champ"><div class="menu-text">Tandoori Malai Champ</div><div class="price">220/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/PfCqhcLV/veg-patter.jpg" alt="Veg Platter"><div class="menu-text">Veg Platter</div><div class="price">400/-</div></div>
    </div>
</body>
</html>
  >
   <p></p>
         
        </div>
    </section>

    <section class="section" onclick="toggleDetails('section10')">
        <span class="click-here">Click Here</span>
        <h2>RESTAURANT MENU II</h2>
        <div id="section10" class="details">
         <div <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Restaurant Menu</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f8f8f8;
            text-align: center;
        }
        .menu-container {
            width: 80%;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            color: #d32f2f;
        }
        h2 {
            background: #ff9800;
            color: white;
            padding: 10px;
            border-radius: 5px;
        }
        .menu-item {
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 15px;
            border-bottom: 1px solid #ddd;
        }
        .menu-item img {
            width: 60px;
            height: 60px;
            object-fit: cover;
            border-radius: 10px;
        }
        .menu-text {
            flex-grow: 1;
            padding: 0 20px;
            text-align: left;
        }
        .price {
            font-weight: bold;
            color: #d32f2f;
        }
    </style>
</head>
<body>
    <div class="menu-container">
        <h1>Restaurant Menu</h1>
        <h2>INDIAN CUISINE (NON-VEG)</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/kgBj7f2R/Kadai-Chicken.jpg" alt="Kadai Chicken"><div class="menu-text">Kadai Chicken (Half/Full)</div><div class="price">300/- | 500/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/fLTShgb6/rada-chiken.jpg" alt="Rada Chicken"><div class="menu-text">Rada Chicken (Half/Full)</div><div class="price">300/- | 500/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/YS91fVzd/masala-chiken.jpg" alt="chicken Masala"><div class="menu-text">Chicken Masala (Half/Full)</div><div class="price">300/- | 500/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/P5Bt2vm0/chiken-curry.jpg" alt="Chicken Curry"><div class="menu-text">Chicken Curry (Half/Full)</div><div class="price">300/- | 500/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/ydppycRZ/butter-chicken.jpg" alt="Butter Chicken"><div class="menu-text">Butter Chicken (Half/Full)</div><div class="price">350/- | 550/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/fb21BGny/chiken-tika-butter-masala.jpg" alt="Chicken Tikka Butter Masala"><div class="menu-text">Chicken Tikka Butter Masala (H/F)</div><div class="price">450/- | 600/-</div></div>
        
        <h2>EGG DISHES</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/XvmQZ46f/egg-burgy.jpg" alt="Egg Bhurji"><div class="menu-text">Egg Bhurji (4 Egg)</div><div class="price">150/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/xCLycmRQ/egg-curry.jpg" alt="Egg Curry"><div class="menu-text">Egg Curry (2 Egg)</div><div class="price">180/-</div></div>
        
        <h2>INDIAN BREADS</h2>
        <div class="menu-item"><img src="https://i.postimg.cc/5N54n2Pt/towa-roti.jpg" alt="Plain Tawa Roti"><div class="menu-text">Plain Tawa Roti</div><div class="price">20/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/6p5XcL2H/butter-roti.jpg" alt="Butter Roti"><div class="menu-text">Butter Roti</div><div class="price">25/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/sxy8Xs5n/tandori-roti.jpg" alt="Tandoori Roti"><div class="menu-text">Tandoori Roti</div><div class="price">20/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/zD60Dn1y/tandori-roti-buter.jpg" alt="Tandoori Roti With Butter"><div class="menu-text">Tandoori Roti With Butter</div><div class="price">25/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/0j0Q4YYV/Plain-Naan.jpg" alt="Plain Naan"><div class="menu-text">Plain Naan</div><div class="price">30/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/prWxpgjB/panner-stuf-nan.jpg" alt="Butter Naan"><div class="menu-text">Butter Naan</div><div class="price">50/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/MG6h0yHW/stuf-nan.webp" alt="Stuffed Naan"><div class="menu-text">Stuffed Naan</div><div class="price">70/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/prWxpgjB/panner-stuf-nan.jpg" alt="Paneer Stuffed Naan"><div class="menu-text">Paneer Stuffed Naan</div><div class="price">100/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/vB6X5BrY/lacha-prantha.jpg" alt="Lachha Parantha Tandoori"><div class="menu-text">Lachha Parantha Tandoori</div><div class="price">60/-</div></div>
        <div class="menu-item"><img src="https://i.postimg.cc/LsPZTZbb/masi-roti.jpg" alt="Missi Roti"><div class="menu-text">Missi Roti</div><div class="price">60/-</div></div>
    </div>
</body>
</html>
 >  
 <p></p>

 </div>
    </section>

    <script>
        function toggleDetails(id) {
            var details = document.getElementById(id);
            if (details.style.display === "none" || details.style.display === "") {
                details.style.display = "block"; // Show details
            } else {
                details.style.display = "none"; // Hide details
            }
        }
    </script>

</body>
</html>
