<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Food Delivery System</title>
    <link rel="stylesheet" href="styles1.css">
</head>
<body>
    <div class="navbar">
        <ul>
            <li><a href="#" data-section="home">Home</a></li>
            <li><a href="#" data-section="rice">Rice</a></li>
            <li><a href="#" data-section="beans">Beans</a></li>
            <li><a href="#" data-section="spaghetti">Spaghetti</a></li>
            <li><a href="#" data-section="swallow">Swallow</a></li>
            <li><a href="#" data-section="bread-egg">Bread & Egg</a></li>
            <li><a href="#" data-section="drinks">Drinks</a></li>
            <li><a href="#" data-section="cart">Cart</a></li>
        </ul>
    </div>

    
    <div id="home" class="section">
        <h1>Welcome to the Scharde's Food Delivery System</h1>
        <p>Select an option from the menu to start ordering.</p>
        <div class="animation">
            <div class="spinner"></div>
            <p>Loading...</p>
        </div>
    </div>

    
    <div id="rice" class="section hidden">
        <h1>Rice</h1>
        <form id="rice-form">
            <label for="rice-type">Type of Rice:</label>
            <select id="rice-type">
                <option value="white">White Rice</option>
                <option value="jollof">Jollof Rice</option>
                <option value="fried">Fried Rice</option>
                <option value="jollof-fried">Jollof + Fried Rice</option>
                <option value="rice-beans">Rice + Beans</option>
            </select>

            <label for="rice-spoons">Spoons (₦200 per spoon):</label>
            <input type="number" id="rice-spoons" min="1" value="1">

            <fieldset>
                <legend>Extras:</legend>
                <label><input type="checkbox" id="add-chicken"> Chicken (₦900)</label>
                <label><input type="checkbox" id="add-egg"> Egg (₦200)</label>
                <label><input type="checkbox" id="add-fish"> Fish (₦200)</label>
                <label><input type="checkbox" id="add-coleslaw"> Coleslaw (₦200)</label>
                <label><input type="checkbox" id="add-beans"> Beans (₦200)</label>
                <label><input type="checkbox" id="add-moi-moi"> Moi-Moi (₦200)</label>
            </fieldset>

            <label for="rice-packs">Packs:</label>
            <input type="number" id="rice-packs" min="1" value="1">

            <button type="button" id="add-to-cart-rice">Add to Cart</button>
        </form>

        
        <div id="rice-display" class="selection-display">
            <h4>Your Selection:</h4>
            <p id="rice-selection-text">Nothing selected yet.</p>
        </div>
    </div>

    
    <div id="beans" class="section hidden">
        <h1>Beans</h1>
        <form id="beans-form">
            <label for="beans-spoons">Spoons (₦200 per spoon):</label>
            <input type="number" id="beans-spoons" min="1" value="1">

            <label for="beans-packs">Packs:</label>
            <input type="number" id="beans-packs" min="1" value="1">

            <button type="button" id="add-to-cart-beans">Add to Cart</button>
        </form>

       
        <div id="beans-display" class="selection-display">
            <h4>Your Selection:</h4>
            <p id="beans-selection-text">Nothing selected yet.</p>
        </div>
    </div>

    
    <div id="spaghetti" class="section hidden">
        <h1>Spaghetti</h1>
        <form id="spaghetti-form">
            <label for="spaghetti-type">Type of Spaghetti:</label>
            <select id="spaghetti-type">
                <option value="white">White Spaghetti</option>
                <option value="jollof">Jollof Spaghetti</option>
            </select>
            <label for="spaghetti-spoons">Spoons (₦200 per spoon):</label>
            <input type="number" id="spaghetti-spoons" min="1" value="1">

            <fieldset>
                <legend>Extras:</legend>
                <label><input type="checkbox" id="add-chicken-spag"> Chicken (₦900)</label>
                <label><input type="checkbox" id="add-egg-spag"> Egg (₦200)</label>
                <label><input type="checkbox" id="add-fish-spag"> Fish (₦200)</label>
                <label><input type="checkbox" id="add-beef-spag"> Beef (₦200)</label>
            </fieldset>

            <label for="spaghetti-packs">Packs:</label>
            <input type="number" id="spaghetti-packs" min="1" value="1">

            <button type="button" id="add-to-cart-spaghetti">Add to Cart</button>
        </form>

       
        <div id="spaghetti-display" class="selection-display">
            <h4>Your Selection:</h4>
            <p id="spaghetti-selection-text">Nothing selected yet.</p>
        </div>
    </div>

    
    <div id="swallow" class="section hidden">
        <h1>Swallow</h1>
        <form id="swallow-form">
            <label for="swallow-type">Type of Swallow:</label>
            <select id="swallow-type">
                <option value="eba">EBA</option>
                <option value="fufu">Fufu</option>
                <option value="amala">Amala</option>
            </select>

            <label for="soup-type">Type of Soup:</label>
            <select id="soup-type">
                <option value="egusi">Egusi</option>
                <option value="gbegiri">Gbegiri</option>
                <option value="okro">Okro</option>
                <option value="ewedu">Ewedu</option>
                <option value="vegetable">Vegetable</option>
            </select>

            <label for="swallow-servings">Number of Swallows (₦200 per swallow):</label>
            <input type="number" id="swallow-servings" min="1" value="1">

            <label for="swallow-packs">Packs:</label>
            <input type="number" id="swallow-packs" min="1" value="1">

            <fieldset>
                <legend>Extras:</legend>
                <label><input type="checkbox" id="add-fish-swallow"> Fish (₦200)</label>
                <label><input type="checkbox" id="add-chicken-swallow"> Chicken (₦900)</label>
            </fieldset>

            <button type="button" id="add-to-cart-swallow">Add to Cart</button>
        </form>

        
        <div id="swallow-display" class="selection-display">
            <h4>Your Selection:</h4>
            <p id="swallow-selection-text">Nothing selected yet.</p>
        </div>
    </div>

    
    <div id="bread-egg" class="section hidden">
        <h1>Bread & Egg</h1>
        <form id="bread-egg-form">
            <label for="bread-size">Size of Bread:</label>
            <select id="bread-size">
                <option value="small">Small</option>
                <option value="medium">Medium</option>
                <option value="big">Big</option>
            </select>

            <label for="egg-quantity">Number of Eggs:</label>
            <input type="number" id="egg-quantity" min="1" value="1">

            <label for="bread-egg-packs">Packs:</label>
            <input type="number" id="bread-egg-packs" min="1" value="1">

            <button type="button" id="add-to-cart-bread-egg">Add to Cart</button>
        </form>

        
        <div id="bread-egg-display" class="selection-display">
            <h4>Your Selection:</h4>
            <p id="bread-egg-selection-text">Nothing selected yet.</p>
        </div>
    </div>

   
<div id="drinks" class="section hidden">
    <h1>Drinks</h1>
    <form id="drinks-form">
        <fieldset>
            <legend>Drinks:</legend>
            <div class="drink-selection">
                <label for="coke-quantity">Coke (₦150):</label>
                <input type="number" id="coke-quantity" min="0" value="0">
            </div>
            <div class="drink-selection">
                <label for="fanta-quantity">Fanta (₦150):</label>
                <input type="number" id="fanta-quantity" min="0" value="0">
            </div>
            <div class="drink-selection">
                <label for="sprite-quantity">Sprite (₦150):</label>
                <input type="number" id="sprite-quantity" min="0" value="0">
            </div>
            <div class="drink-selection">
                <label for="pepsi-quantity">Pepsi (₦150):</label>
                <input type="number" id="pepsi-quantity" min="0" value="0">
            </div>
            <div class="drink-selection">
                <label for="bottle-water-quantity">Bottle Water (₦100):</label>
                <input type="number" id="bottle-water-quantity" min="0" value="0">
            </div>
            <div class="drink-selection">
                <label for="maltina-quantity">Maltina (₦150):</label>
                <input type="number" id="maltina-quantity" min="0" value="0">
            </div>
        </fieldset>

        <button type="button" id="add-to-cart-drinks">Add to Cart</button>
    </form>

    
    <div id="drinks-display" class="selection-display">
        <h4>Your Selection:</h4>
        <p id="drinks-selection-text">Nothing selected yet.</p>
    </div>
</div>


    
    <div id="cart" class="section hidden">
        <h1>Cart</h1>
        <div id="cart-items">
            
        </div>
        <button type="button" id="clear-cart">Clear Cart</button>                                                                                             








css

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    color: #333;
    background-color: #f4f4f4; 
}

.navbar {
    background-color: #ff6f61; 
    padding: 1rem;
    text-align: center;
}

.navbar ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
}

.navbar ul li {
    display: inline;
    margin: 0 1rem;
}

.navbar ul li a {
    color: #fff;
    text-decoration: none;
    font-weight: bold;
    font-size: 1.5rem;
}

.navbar ul li a:hover {
    text-decoration: underline;
}


.section {
    padding: 2rem;
    background-color: #fff; 
    border-radius: 8px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
    margin: 1rem;
}

.hidden {
    display: none;
}

h1 {
    font-size: 2.5rem;
    color: #2e8b57;
    margin-bottom: 1rem;
}

form {
    margin: 2rem 0;
    font-size: 1.2rem;
}

label {
    display: block;
    margin: 0.5rem 0;
}

input[type="number"], select {
    padding: 0.5rem;
    margin-left: 0.5rem;
    border: 1px solid #ddd;
    border-radius: 5px;
}

button {
    background-color: #2e8b57; 
    color: #fff;
    padding: 0.7rem 1.5rem;
    border: none;
    cursor: pointer;
    font-size: 1.2rem;
    margin-top: 1rem;
    border-radius: 5px;
}

button:hover {
    background-color: #1e6f4c; }


.selection-display {
    margin-top: 1rem;
    padding: 1rem;
    background-color: #e6f9e6; 
    border-radius: 8px;
    border: 1px solid #2e8b57; 
}

.selection-display h4 {
    margin: 0;
    color: #2e8b57; 
}

.selection-display p {
    margin: 10px 0;
}


#cart {
    background-color: #fff; 
    border: 1px solid #ddd;
    padding: 1rem;
    border-radius: 8px;
    margin: 1rem;
}

#cart-items {
    margin: 1rem 0;
    padding: 1rem;
    background-color: #f0f0f0; 
    border-radius: 5px;
    font-size: 1.2rem;
}

.cart-item {
    padding: 10px;
    margin-bottom: 10px;
    border: 1px solid #ddd;
    border-radius: 5px;
    background-color: #fff; 
}

#total-price {
    font-size: 1.5rem;
    font-weight: bold;
    color: #ff6f61; 
}


.animation {
    text-align: center;
    margin-top: 2rem;
}

.spinner {
    border: 8px solid #f3f3f3; 
    border-top: 8px solid #2e8b57; 
    border-radius: 50%;
    width: 60px;
    height: 60px;
    animation: spin 1s linear infinite;
    margin: 0 auto;
}

@keyframes spin {
    0% { transform: rotate(0deg); }
    100% { transform: rotate(360deg); }
}

/* Responsive Design */
@media (max-width: 768px) {
    .navbar ul li {
        display: block;
        margin: 0.5rem 0;
    }
    
    .section {
        margin: 0.5rem;
        padding: 1rem;
    }
}
html {
    scroll-behavior: smooth;
}

@media (max-width: 768px) {
    .navbar ul li {
        display: block;
        margin: 0.5rem 0;
    }
    button {
        width: 100%;
        margin-top: 1rem;
    }
}















jss
document.addEventListener('DOMContentLoaded', function () {
    const sections = document.querySelectorAll('.section');
    const navLinks = document.querySelectorAll('.navbar a');

    function showSection(id) {
        sections.forEach(section => {
            section.classList.add('hidden');
            if (section.id === id) {
                section.classList.remove('hidden');
            }
        });
    }

    navLinks.forEach(link => {
        link.addEventListener('click', function (e) {
            e.preventDefault();
            showSection(this.dataset.section);
        });
    });

    // Rice calculations
    document.getElementById('add-to-cart-rice').addEventListener('click', function () {
        const riceType = document.getElementById('rice-type').value;
        const riceSpoons = parseInt(document.getElementById('rice-spoons').value);
        const ricePacks = parseInt(document.getElementById('rice-packs').value);

        let extrasPrice = 0;
        if (document.getElementById('add-chicken').checked) extrasPrice += 900;
        if (document.getElementById('add-egg').checked) extrasPrice += 200;
        if (document.getElementById('add-fish').checked) extrasPrice += 200;
        if (document.getElementById('add-coleslaw').checked) extrasPrice += 200;
        if (document.getElementById('add-beans').checked) extrasPrice += 200;
        if (document.getElementById('add-moi-moi').checked) extrasPrice += 200;

        const totalPerSpoon = 200 * riceSpoons;
        const total = (totalPerSpoon + extrasPrice) * ricePacks;

        document.getElementById('rice-selection-text').innerHTML = `
            <strong>Rice Type:</strong> ${riceType}<br>
            <strong>Spoons:</strong> ${riceSpoons}<br>
            <strong>Extras Price:</strong> ₦${extrasPrice}<br>
            <strong>Number of Packs:</strong> ${ricePacks}<br>
            <strong>Total Cost:</strong> ₦${total}
        `;
        addToCart(`
            <strong>Rice Type:</strong> ${riceType}<br>
            <strong>Spoons:</strong> ${riceSpoons}<br>
            <strong>Extras Price:</strong> ₦${extrasPrice}<br>
            <strong>Number of Packs:</strong> ${ricePacks}<br>
            <strong>Total Cost:</strong> ₦${total}
        `);
    });

    // Beans calculations
    document.getElementById('add-to-cart-beans').addEventListener('click', function () {
        const beansSpoons = parseInt(document.getElementById('beans-spoons').value);
        const beansPacks = parseInt(document.getElementById('beans-packs').value);

        const total = 200 * beansSpoons * beansPacks;

        document.getElementById('beans-selection-text').innerHTML = `
            <strong>Spoons:</strong> ${beansSpoons}<br>
            <strong>Number of Packs:</strong> ${beansPacks}<br>
            <strong>Total Cost:</strong> ₦${total}
        `;
        addToCart(`
            <strong>Spoons:</strong> ${beansSpoons}<br>
            <strong>Number of Packs:</strong> ${beansPacks}<br>
            <strong>Total Cost:</strong> ₦${total}
        `);
    });

    // Spaghetti calculations
    document.getElementById('add-to-cart-spaghetti').addEventListener('click', function () {
        const spaghettiType = document.getElementById('spaghetti-type').value;
        const spaghettiPacks = parseInt(document.getElementById('spaghetti-packs').value);

        let extrasPrice = 0;
        if (document.getElementById('add-chicken-spag').checked) extrasPrice += 900;
        if (document.getElementById('add-egg-spag').checked) extrasPrice += 200;
        if (document.getElementById('add-fish-spag').checked) extrasPrice += 200;
        if (document.getElementById('add-beef-spag').checked) extrasPrice += 200;

        const totalPerPack = 200 + extrasPrice;
        const total = totalPerPack * spaghettiPacks;

        document.getElementById('spaghetti-selection-text').innerHTML = `
            <strong>Spaghetti Type:</strong> ${spaghettiType}<br>
            <strong>Extras Price:</strong> ₦${extrasPrice}<br>
            <strong>Number of Packs:</strong> ${spaghettiPacks}<br>
            <strong>Total Cost:</strong> ₦${total}
        `;
        addToCart(`
            <strong>Spaghetti Type:</strong> ${spaghettiType}<br>
            <strong>Extras Price:</strong> ₦${extrasPrice}<br>
            <strong>Number of Packs:</strong> ${spaghettiPacks}<br>
            <strong>Total Cost:</strong> ₦${total}
        `);
    });

    // Swallow calculations
    document.getElementById('add-to-cart-swallow').addEventListener('click', function () {
        const swallowType = document.getElementById('swallow-type').value;
        const soupType = document.getElementById('soup-type').value;
        const swallowServings = parseInt(document.getElementById('swallow-servings').value);
        const swallowPacks = parseInt(document.getElementById('swallow-packs').value);

        let extrasPrice = 0;
        if (document.getElementById('add-fish-swallow').checked) extrasPrice += 200;
        if (document.getElementById('add-chicken-swallow').checked) extrasPrice += 900;

        const totalPerSwallow = 200 * swallowServings;
        const total = (totalPerSwallow + extrasPrice) * swallowPacks;

        document.getElementById('swallow-selection-text').innerHTML = `
            <strong>Swallow Type:</strong> ${swallowType}<br>
            <strong>Soup Type:</strong> ${soupType}<br>
            <strong>Number of Servings:</strong> ${swallowServings}<br>
            <strong>Extras Price:</strong> ₦${extrasPrice}<br>
            <strong>Number of Packs:</strong> ${swallowPacks}<br>
            <strong>Total Cost:</strong> ₦${total}
        `;
        addToCart(`
            <strong>Swallow Type:</strong> ${swallowType}<br>
            <strong>Soup Type:</strong> ${soupType}<br>
            <strong>Number of Servings:</strong> ${swallowServings}<br>
            <strong>Extras Price:</strong> ₦${extrasPrice}<br>
            <strong>Number of Packs:</strong> ${swallowPacks}<br>
            <strong>Total Cost:</strong> ₦${total}
        `);
    });

    // Bread & Egg calculations
    document.getElementById('add-to-cart-bread-egg').addEventListener('click', function () {
        const breadSize = document.getElementById('bread-size').value;
        const eggQuantity = parseInt(document.getElementById('egg-quantity').value);
        const breadEggPacks = parseInt(document.getElementById('bread-egg-packs').value);

        const breadPrices = { small: 100, medium: 150, big: 200 };
        const total = (breadPrices[breadSize] + (eggQuantity * 200)) * breadEggPacks;

        document.getElementById('bread-egg-selection-text').innerHTML = `
            <strong>Bread Size:</strong> ${breadSize}<br>
            <strong>Number of Eggs:</strong> ${eggQuantity}<br>
            <strong>Number of Packs:</strong> ${breadEggPacks}<br>
            <strong>Total Cost:</strong> ₦${total}
        `;
        addToCart(`
            <strong>Bread Size:</strong> ${breadSize}<br>
            <strong>Number of Eggs:</strong> ${eggQuantity}<br>
            <strong>Number of Packs:</strong> ${breadEggPacks}<br>
            <strong>Total Cost:</strong> ₦${total}
        `);
    });

    // Drinks calculations
    document.getElementById('add-to-cart-drinks').addEventListener('click', function () {
        const drinks = {
            coke: parseInt(document.getElementById('coke-quantity').value) || 0,
            fanta: parseInt(document.getElementById('fanta-quantity').value) || 0,
            sprite: parseInt(document.getElementById('sprite-quantity').value) || 0,
            pepsi: parseInt(document.getElementById('pepsi-quantity').value) || 0,
            bottleWater: parseInt(document.getElementById('bottle-water-quantity').value) || 0,
            maltina: parseInt(document.getElementById('maltina-quantity').value) || 0
        };

        let total = 0;
        total += drinks.coke * 150;
        total += drinks.fanta * 150;
        total += drinks.sprite * 150;
        total += drinks.pepsi * 150;
        total += drinks.bottleWater * 100;
        total += drinks.maltina * 200;

        document.getElementById('drinks-selection-text').innerHTML = `
            <strong>Selected Drinks:</strong><br>
            Coke: ${drinks.coke} x ₦150<br>
            Fanta: ${drinks.fanta} x ₦150<br>
            Sprite: ${drinks.sprite} x ₦150<br>
            Pepsi: ${drinks.pepsi} x ₦150<br>
            Bottle Water: ${drinks.bottleWater} x ₦100<br>
            Maltina: ${drinks.maltina} x ₦200<br>
            <strong>Total Cost:</strong> ₦${total}
        `;
        addToCart(`
            <strong>Selected Drinks:</strong><br>
            Coke: ${drinks.coke} x ₦150<br>
            Fanta: ${drinks.fanta} x ₦150<br>
            Sprite: ${drinks.sprite} x ₦150<br>
            Pepsi: ${drinks.pepsi} x ₦150<br>
            Bottle Water: ${drinks.bottleWater} x ₦100<br>
            Maltina: ${drinks.maltina} x ₦200<br>
            <strong>Total Cost:</strong> ₦${total}
        `);
    });

    // Cart functionality
    function addToCart(selectionText) {
        const cartItems = document.getElementById('cart-items');
        const itemDiv = document.createElement('div');
        itemDiv.innerHTML = selectionText + '<hr>';
        cartItems.appendChild(itemDiv);
    }

    document.getElementById('clear-cart').addEventListener('click', function () {
        document.getElementById('cart-items').innerHTML = '';
    });
});



        <a href="checkout.html"><button id="checkout">Checkout</button></a>
    </div>




payment
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Payment</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="logo">
            <h1>Drone Delivery</h1>
        </div>
        <nav>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="order.html">Order</a></li>
                <li><a href="cart.html">Cart</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="payment-form">
            <h2>Payment</h2>
            <form action="confirmation.html" method="post">
                <label for="cardholder">Cardholder Name:</label>
                <input type="text" id="cardholder" name="cardholder" required>
                
                <label for="cardnumber">Card Number:</label>
                <input type="text" id="cardnumber" name="cardnumber" required>
                
                <label for="expiry">Expiry Date:</label>
                <input type="month" id="expiry" name="expiry" required>
                
                <label for="cvv">CVV:</label>
                <input type="text" id="cvv" name="cvv" required>
                
                <button type="submit" class="cta-button">Confirm Payment</button>
            </form>
        </section>
    </main>

    <footer>
        <p>SAINT.</p>
    </footer>
</body>
</html>



    <script src="style.js"></script>
</body>
</html>
