# mission-jee-mains-crash
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Mission JEE Mains Crash</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background: #f9f9f9;
      color: #222;
    }
    header {
      background: #003366;
      color: #fff;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    nav a {
      margin: 0 1rem;
      color: #fff;
      text-decoration: none;
      font-weight: 600;
    }
    .hero {
      padding: 4rem 2rem;
      text-align: center;
      background: linear-gradient(to right, #007acc, #005fa3);
      color: white;
    }
    .hero h1 {
      font-size: 2.5rem;
      margin-bottom: 1rem;
    }
    .section {
      padding: 2rem;
      max-width: 1000px;
      margin: auto;
    }
    .cards {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 1rem;
    }
    .card {
      background: white;
      padding: 1.5rem;
      border-radius: 12px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      transition: transform 0.2s;
    }
    .card:hover {
      transform: translateY(-5px);
    }
    .search-box {
      margin: 2rem auto;
      max-width: 600px;
      text-align: center;
    }
    .search-box input {
      width: 100%;
      padding: 0.75rem;
      font-size: 1rem;
      border: 1px solid #ccc;
      border-radius: 8px;
    }
    ul.notes-list {
      list-style: none;
      padding-left: 0;
    }
    ul.notes-list li {
      background: white;
      padding: 1rem;
      margin-bottom: 1rem;
      border-radius: 8px;
      box-shadow: 0 1px 4px rgba(0,0,0,0.05);
    }
    footer {
      background: #003366;
      color: white;
      text-align: center;
      padding: 1rem;
      margin-top: 2rem;
    }
  </style>
</head>
<body>
  <header>
    <h2>Mission JEE Mains Crash</h2>
    <nav>
      <a href="#subjects">Subjects</a>
      <a href="#notes">Notes</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section class="hero">
    <h1>Crack JEE Mains with Expert Notes</h1>
    <p>Get topic-wise crash course notes for Physics, Chemistry & Math</p>
  </section>

  <section class="section" id="subjects">
    <h2>Subjects</h2>
    <div class="cards">
      <div class="card">
        <h3>Physics</h3>
        <p>Mechanics, Electrodynamics, Modern Physics and more.</p>
      </div>
      <div class="card">
        <h3>Chemistry</h3>
        <p>Organic, Inorganic, Physical Chemistry notes organized by chapters.</p>
      </div>
      <div class="card">
        <h3>Mathematics</h3>
        <p>Functions, Calculus, Algebra, Coordinate Geometry, and more.</p>
      </div>
    </div>
  </section>

  <section class="section" id="notes">
    <h2>Download Notes</h2>
    <div class="search-box">
      <input type="text" id="searchInput" placeholder="Search notes by topic...">
    </div>
    <ul class="notes-list" id="notesList">
      <li><a href="#">📘 Physics: Kinematics - Download PDF</a></li>
      <li><a href="#">📗 Chemistry: Atomic Structure - Download PDF</a></li>
      <li><a href="#">📙 Math: Quadratic Equations - Download PDF</a></li>
      <li><a href="#">📘 Physics: Thermodynamics - Download PDF</a></li>
      <li><a href="#">📗 Chemistry: Chemical Bonding - Download PDF</a></li>
      <li><a href="#">📙 Math: Integration - Download PDF</a></li>
    </ul>
  </section>

  <section class="section" id="about">
    <h2>About Mission JEE Mains Crash</h2>
    <p>We are passionate about helping JEE aspirants simplify their revision journey with crisp, high-yield notes designed for last-minute revision.</p>
  </section>

  <section class="section" id="contact">
    <h2>Contact Us</h2>
    <p>Email: missionjeemainscrash@example.com</p>
  </section>

  <footer>
    &copy; 2025 Mission JEE Mains Crash. All rights reserved.
  </footer>

  <script>
    const searchInput = document.getElementById("searchInput");
    const notesList = document.getElementById("notesList");
    const notes = notesList.getElementsByTagName("li");

    searchInput.addEventListener("input", function() {
      const filter = searchInput.value.toLowerCase();
      Array.from(notes).forEach(note => {
        const text = note.textContent.toLowerCase();
        note.style.display = text.includes(filter) ? "block" : "none";
      });
    });
  </script>
</body>
</html>


✅ The search function is now live on your site!

🔍 What’s added:

A search box in the “Download Notes” section.

Users can type a topic name (e.g. “thermo”, “kinematics”) and the list of notes will dynamically filter as they type.


💡 You can:

Add more <li> elements under #notesList to grow your library.

Customize placeholder text or search behavior easily if needed.


Would you like to:

Host the site next?

Add categories or filters by subject?

Enable PDF preview or download counter?


Let me know how else you'd like to enhance it!

