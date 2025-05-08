# Barbershop-
<!DOCTYPE html><html lang="fa">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>آرایشگاه Matin</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>آرایشگاه Matin</h1>
    <p>رزرو نوبت آنلاین</p>
  </header>  <main>
    <section class="form-section">
      <h2>فرم رزرو نوبت</h2>
      <form id="appointmentForm">
        <input type="text" id="name" placeholder="نام شما" required>
        <input type="date" id="date" required>
        <input type="time" id="time" required>
        <button type="submit">رزرو</button>
      </form>
    </section><section class="list-section">
  <h2>نوبت‌های رزرو شده</h2>
  <ul id="appointmentsList"></ul>
</section>

  </main>  <footer>
    <p>طراحی شده توسط Matin - 2025</p>
  </footer>  <script src="script.js"></script></body>
</html>
body {
  font-family: Tahoma, sans-serif;
  direction: rtl;
  margin: 0;
  padding: 0;
  background-color: #f3f3f3;}

header {
  background-color: #0057b8;
  color: white;
  padding: 20px;
  text-align: center;}

main {
  padding: 20px;}

h2 {
  color: #d40000;}

form {
  margin-bottom: 20px;
  background-color: white;
  padding: 15px;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(0,0,0,0.1);}

input, button {
  width: 100%;
  padding: 10px;
  margin: 8px 0;
  border: 1px solid #ccc;
  border-radius: 4px;}

button {
  background-color: #d40000;
  color: white;
  font-weight: bold;
  cursor: pointer;}

button:hover {
  background-color: #a30000;}
footer {
  background-color: #0057b8;
  color: white;
  text-align: center;
  padding: 10px;
  margin-top: 30px;}
  const form = document.getElementById('appointmentForm');
const list = document.getElementById('appointmentsList');
form.addEventListener('submit', function(e) {
  e.preventDefault();
  const name = document.getElementById('name').value;
  const date = document.getElementById('date').value;
  const time = document.getElementById('time').value;
  const appointment = `${name} - ${date} - ${time}`;
  const li = document.createElement('li');
  li.textContent = appointment;
  list.appendChild(li);
  form.reset();});
