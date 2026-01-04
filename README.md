<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>1067 Taxi</title>
<style>
  body {
    margin: 0;
    padding: 0;
    font-family: 'Arial', sans-serif;
    background: linear-gradient(to bottom, #1abc9c, #16a085);
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    color: #fff;
  }

  .container {
    background: rgba(0,0,0,0.5);
    padding: 30px 40px;
    border-radius: 20px;
    text-align: center;
    box-shadow: 0 8px 20px rgba(0,0,0,0.3);
  }

  h1 {
    font-size: 96px;
    margin: 0 0 10px;
    letter-spacing: 5px;
  }

  p {
    font-size: 18px;
    margin: 0 0 30px;
    color: #ecf0f1;
  }

  input {
    width: 100%;
    padding: 14px;
    border-radius: 10px;
    border: none;
    font-size: 18px;
    margin-bottom: 20px;
  }

  button {
    width: 100%;
    padding: 14px;
    font-size: 20px;
    border: none;
    border-radius: 10px;
    background-color: #f1c40f;
    color: #000;
    cursor: pointer;
    transition: 0.3s;
  }

  button:hover {
    background-color: #f39c12;
  }

  small {
    display: block;
    margin-top: 15px;
    font-size: 14px;
    color: #ecf0f1;
  }
</style>
</head>
<body>

<div class="container">
  <h1>1067</h1>
  <p>Taxi chaqirish xizmati</p>

  <input type="tel" id="phone" placeholder="Telefon raqamingiz (+998...)">
  <button onclick="callTaxi()">🚕 Taxi chaqirish</button>

  <small>Minimal narx: 5 000 so‘m | 1 km = 1 500 so‘m</small>
</div>

<script>
function callTaxi() {
  const phone = document.getElementById('phone').value.trim();
  if(phone === '') {
    alert("Iltimos, telefon raqamingizni kiriting");
    return;
  }
  alert(`Buyurtmangiz qabul qilindi!\nOperator tez orada sizga qo'ng'iroq qiladi.\nTelefon: ${phone}`);
}
</script>

</body>
</html>
