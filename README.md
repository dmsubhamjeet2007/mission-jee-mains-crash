# mission-jee-mains-crash
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Mission JEE Mains Crash</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background-color: #f4f4f4;
      color: #333;
      transition: background-color 0.3s, color 0.3s;
    }
    header {
      background-color: #007BFF;
      color: white;
      padding: 1rem;
      text-align: center;
    }
    nav {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      background-color: #0056b3;
      padding: 0.5rem;
    }
    nav button {
      background: none;
      border: none;
      color: white;
      margin: 0.5rem;
      padding: 0.5rem 1rem;
      cursor: pointer;
      font-size: 1rem;
    }
    nav button:hover {
      text-decoration: underline;
    }
    .search-box {
      display: flex;
      justify-content: center;
      margin: 1rem;
    }
    .search-box input {
      width: 80%;
      padding: 0.5rem;
      font-size: 1rem;
    }
    .content {
      padding: 1rem;
    }
    .note {
      background-color: white;
      padding: 1rem;
      margin: 1rem auto;
      border-radius: 10px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
      max-width: 600px;
    }
    .download {
      display: block;
      margin-top: 0.5rem;
      color: #007BFF;
    }
    .dark-mode {
      background-color: #121212;
      color: #f1f1f1;
    }
    .dark-mode .note {
      background-color: #1e1e1e;
    }
    .toggle-theme {
      position: fixed;
      top: 10px;
      right: 10px;
      background-color: #007BFF;
      color: white;
      border: none;
      padding: 0.5rem 1rem;
      border-radius: 20px;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <button class="toggle-theme" onclick="toggleTheme()">🌙</button>
  <header>
    <h1>Mission JEE Mains Crash</h1>
    <p>Your all-in-one hub for JEE preparation notes</p>
  </header>  <nav>
    <button onclick="filterNotes('all')">All</button>
    <button onclick="filterNotes('physics')">Physics</button>
    <button onclick="filterNotes('chemistry')">Chemistry</button>
    <button onclick="filterNotes('maths')">Maths</button>
  </nav>  <div class="search-box">
    <input type="text" id="searchInput" onkeyup="searchNotes()" placeholder="Search notes...">
  </div>  <div class="content" id="notes">
    <div class="note" data-subject="physics"> 
      <h3>Physics - Motion in One Dimension</h3>
      <p>Concepts, formulas, and solved examples.</p>
      <a href="#" class="download">📥 Download PDF</a>
    </div>
    <div class="note" data-subject="chemistry">
      <h3>Chemistry - Atomic Structure</h3>
      <p>All about electrons, protons and neutrons.</p>
      <a href="#" class="download">📥 Download PDF</a>
    </div>
    <div class="note" data-subject="maths">
      <h3>Maths - Quadratic Equations</h3>
      <p>Roots, nature and graphical analysis.</p>
      <a href="#" class="download">📥 Download PDF</a>
    </div>
  </div>  <script>
    function filterNotes(subject) {
      const notes = document.querySelectorAll('.note');
      notes.forEach(note => {
        note.style.display = (subject === 'all' || note.dataset.subject === subject) ? 'block' : 'none';
      });
    }

    function searchNotes() {
      const input = document.getElementById('searchInput').value.toLowerCase();
      const notes = document.querySelectorAll('.note');
      notes.forEach(note => {
        note.style.display = note.innerText.toLowerCase().includes(input) ? 'block' : 'none';
      });
    }

    function toggleTheme() {
      document.body.classList.toggle('dark-mode');
    }
  </script></body>
</html>
    
