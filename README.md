# CSS Layouts and Responsive Design

## Objectives

Implement Flexbox and Grid for layout design.
Make the webpage responsive using media queries.
Ensure proper alignment and spacing.

## Instructions

- use Flexbox or CSS Grid.
- Add a navigation bar and structure the content.
- Use media queries to adjust layout for mobile, tablet, and desktop.

>[!NOTE]
>  - Include at least:
>  - navigation bar
>  - media queries

# Tasks

- Apply Flexbox or Grid for layout.
- Make the page responsive.
- Test across different screen sizes.

- <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>PLP CSS Layout</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>

  <header class="navbar">
    <h1 class="logo">MySite</h1>
    <nav>
      <ul class="nav-links">
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Projects</a></li>
        <li><a href="#">Contact</a></li>
      </ul>
    </nav>
  </header>

  <main class="grid-container">
    <section class="main-content">
      <h2>Welcome to My Site</h2>
      <p>This is a responsive layout using Flexbox and Grid. Resize the screen to see it adapt!</p>
    </section>
    
    <aside class="sidebar">
      <h3>Sidebar</h3>
      <p>Extra content goes here.</p>
    </aside>
  </main>

  <footer class="footer">
    <p>© 2025 MySite. All rights reserved.</p>
  </footer>

</body>
</html>

/* Base styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
}

/* Navigation Bar */
.navbar {
  background-color: #333;
  color: #fff;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1rem;
}

.logo {
  font-size: 1.5rem;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1rem;
}

.nav-links li a {
  color: white;
  text-decoration: none;
}

/* Grid layout */
.grid-container {
  display: grid;
  grid-template-columns: 2fr 1fr;
  gap: 1rem;
  padding: 1rem;
}

.main-content, .sidebar {
  background: #f4f4f4;
  padding: 1rem;
  border-radius: 5px;
}

/* Footer */
.footer {
  background-color: #333;
  color: #fff;
  text-align: center;
  padding: 1rem;
  margin-top: 1rem;
}

/* Media Queries */

/* Tablet */
@media (max-width: 768px) {
  .grid-container {
    grid-template-columns: 1fr;
  }

  .nav-links {
    flex-direction: column;
    gap: 0.5rem;
  }

  .navbar {
    flex-direction: column;
    align-items: flex-start;
  }
}

/* Mobile */
@media (max-width: 480px) {
  .navbar {
    padding: 0.5rem;
  }

  .logo {
    font-size: 1.2rem;
  }

  .nav-links {
    font-size: 0.9rem;
  }

  .grid-container {
    padding: 0.5rem;
  }

  .main-content, .sidebar {
    padding: 0.8rem;
  }
}



Happy Coding! 💻✨
