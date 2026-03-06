<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>PARRLX Premium</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

<style>

body{
font-family:Poppins;
margin:0;
background:#f5f5f5;
}

header{
background:black;
color:white;
display:flex;
align-items:center;
padding:15px 40px;
}

header img{
height:45px;
margin-right:15px;
}

.logo{
font-size:24px;
font-weight:600;
letter-spacing:2px;
}

.hero{
text-align:center;
padding:40px;
background:white;
}

.products{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(220px,1fr));
gap:25px;
padding:40px;
}

.card{
background:white;
border-radius:10px;
box-shadow:0 3px 10px rgba(0,0,0,0.1);
overflow:hidden;
transition:0.3s;
}

.card:hover{
transform:translateY(-6px);
}

.card img{
width:100%;
height:260px;
object-fit:cover;
}

.card h3{
padding:10px;
font-size:16px;
}

.price{
color:#e53935;
font-weight:600;
padding:0 10px;
}

.card button{
margin:10px;
padding:10px;
border:none;
background:black;
color:white;
width:90%;
border-radius:6px;
cursor:pointer;
}

.checkout{
background:white;
padding:40px;
margin:40px;
border-radius:10px;
}

input,select{
width:100%;
padding:10px;
margin:8px 0;
border:1px solid #ccc;
border-radius:6px;
}

.paybtn{
background:#1a73e8;
color:white;
padding:12px;
border:none;
width:100%;
font-size:16px;
border-radius:6px;
cursor:pointer;
}

footer{
text-align:center;
padding:20px;
color:#777;
}

</style>
</head>

<body>

<header>

<img src="YOUR_LOGO_IMAGE_LINK_HERE">
<div class="logo">PARRLX</div>

</header>

<section class="hero">

<h1>Premium Streetwear</h1>
<p>Luxury style. Affordable price.</p>

</section>

<section class="products">

<div class="card">
<img src="https://i.ibb.co/gLHGHRPw/Screenshot-20260306-195322.jpg">
<h3>PARRLX Premium Tee</h3>
<div class="price">₹1299</div>
<button onclick="buy('PARRLX Premium Tee')">Buy Now</button>
</div>

<div class="card">
<img src="https://i.ibb.co/FLQXSHvx/Screenshot-20260306-195355.jpg">
<h3>PARRLX Black Fit</h3>
<div class="price">₹1299</div>
<button onclick="buy('PARRLX Black Fit')">Buy Now</button>
</div>

<div class="card">
<img src="https://i.ibb.co/5g6hKwHB/Screenshot-20260306-195405.jpg">
<h3>PARRLX Urban Tee</h3>
<div class="price">₹1299</div>
<button onclick="buy('PARRLX Urban Tee')">Buy Now</button>
</div>

<div class="card">
<img src="https://i.ibb.co/yB7JCfrc/Screenshot-20260306-195343.jpg">
<h3>PARRLX Signature</h3>
<div class="price">₹1299</div>
<button onclick="buy('PARRLX Signature')">Buy Now</button>
</div>

<div class="card">
<img src="https://i.ibb.co/TqdPc8x6/Screenshot-20260306-195429.jpg">
<h3>PARRLX Limited Tee</h3>
<div class="price">₹1299</div>
<button onclick="buy('PARRLX Limited Tee')">Buy Now</button>
</div>

</section>

<section class="checkout">

<h2>Checkout</h2>

<form action="https://formsubmit.co/parrlx08@gmail.com" method="POST">

<input type="hidden" name="_subject" value="New Order - PARRLX">

<label>Product</label>
<input id="product" name="Product" required>

<label>Name</label>
<input name="Name" required>

<label>Email</label>
<input name="Email" required>

<label>Phone</label>
<input name="Phone" required>

<label>Address</label>
<input name="Address" required>

<label>Payment Method</label>

<select name="Payment Method">

<option>Cash On Delivery</option>
<option>Online Payment</option>

</select>

<input type="hidden" name="Price" value="1299">

<button class="paybtn">Place Order</button>

</form>

</section>

<footer>

© 2026 PARRLX • Premium Fashion Brand

</footer>

<script>

function buy(product){

document.getElementById("product").value = product;

window.scrollTo({
top:document.querySelector(".checkout").offsetTop,
behavior:"smooth"
});

}

</script>

</body>
</html>
