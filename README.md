base_dir = "thebaddiehabitat_site"
if os.path.exists(base_dir):
    shutil.rmtree(base_dir)
os.makedirs(base_dir, exist_ok=True)

path, content):
    full = os.path.join(base_dir, path)
    os.makedirs(os.path.dirname(full), exist_ok=True)
    with open(full, "w", encoding="utf-8") as f:
        f.write(content)

<!doctype html><html lang='en'><head><meta charset='utf-8'><meta name='viewport' content='width=device-width,initial-scale=1'><title>The Baddie Habitat</title><link href='https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700;900&display=swap' rel='stylesheet'><link rel='stylesheet' href='css/style.css'><script defer src='js/main.js'></script></head><body><header><h1 class='neon'>The Baddie Habitat</h1><nav><a href='index.html'>Home</a> | <a href='shop.html'>Shop</a> | <a href='about.html'>About</a></nav></header><main><h2>Welcome to The Habitat</h2><p>Luxury teas & supplements for bold women.</p><a href='shop.html' class='btn gold'>Shop Now</a></main><footer><p>© 2025 The Baddie Habitat</p></footer></body></html>")
<!doctype html><html lang='en'><head><meta charset='utf-8'><meta name='viewport' content='width=device-width,initial-scale=1'><title>Shop — The Baddie Habitat</title><link rel='stylesheet' href='css/style.css'><script defer src='js/shop.js'></script></head><body><header><h1 class='neon'>Shop</h1></header><main><div id='products'></div><div id='cart'><h3>Your Cart</h3><div id='cart-items'></div><div>Total: $<span id='cart-total'>0.00</span></div><button id='checkout-btn' class='btn gold'>Checkout</button></div></main><footer><p>© 2025 The Baddie Habitat</p></footer></body></html>")
<!doctype html><html lang='en'><head><meta charset='utf-8'><meta name='viewport' content='width=device-width,initial-scale=1'><title>About — The Baddie Habitat</title><link rel='stylesheet' href='css/style.css'></head><body><header><h1 class='neon'>About Us</h1></header><main><p>The Baddie Habitat is your go-to for clean, chic self-care. Built by women who embody confidence, balance, and beauty.</p></main><footer><p>© 2025 The Baddie Habitat</p></footer></body></html>") 
:root {
  --blush: #f7d7d9;
  --neon-pink: #ff2d95;
  --neon-gold: #ffd166;
  --medium-gray: #b9b9b9;
  --black: #0b0b0b;
}
body {
  font-family: 'Montserrat', sans-serif;
  background: var(--medium-gray);
  color: var(--black);
  margin: 0;
  text-align: center;
}
h1.neon { color: var(--neon-pink); text-shadow: 0 0 8px rgba(255,45,149,0.8); }
a { color: var(--neon-pink); text-decoration: none; }
.btn.gold { background: var(--neon-gold); color: var(--black); padding: 0.5em 1em; border-radius: 8px; }
footer { margin-top: 2em; font-size: 0.9em; }
""")
console.log('Main script loaded');
console.log('Shop script loaded');
os.makedirs(os.path.join(base_dir, "assets"), exist_ok=True)
os.makedirs(os.path.join(base_dir, "content/products"), exist_ok=True)
for i in range(1, 11):
    content/products/product-{i}.md\---
title: "Product {i}"
price: {10+i}
description: "Placeholder description for Product {i}."
image: "/assets/product-{i}.png"
---\"\"\")

textwrap.dedent(\\
# The Baddie Habitat Website Package

home, Shop, About pages
- 10 product placeholders
- Cart + checkout placeholders
- Customizable neon aesthetic (pink, gold, blush)
  



