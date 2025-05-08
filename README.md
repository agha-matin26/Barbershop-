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
