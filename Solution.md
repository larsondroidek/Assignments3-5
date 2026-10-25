# Assignment 3.5 — Solution: Blog / Portfolio Mini-Project

## Project Structure
```
portfolio-website/
├── index.html
├── blog.html
└── images/
    ├── html-badge.png
    ├── laptop-coding.png
    └── mountain-sunset.png
```

## Steps
1. Create the folder, the `images` folder, and put the three images inside it.
2. Create `index.html` and `blog.html` in the project root and paste the code below.
3. Replace "Your Name", email, GitHub username and city with your real details.
4. Test every navigation link with Live Server.
5. Publish to GitHub:
```bash
git init
git add .
git commit -m "Add blog/portfolio website"
git branch -M main
git remote add origin https://github.com/<your-username>/portfolio-website.git
git push -u origin main
```

## index.html
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Your Name — Portfolio</title>
  </head>

  <body>
    <!-- ===== Header with logo/name and navigation ===== -->
    <header>
      <img src="images/html-badge.png" alt="Orange HTML badge used as the website logo" width="60" height="40" />
      <h1>Your Name</h1>
      <p><em>Web Developer in the Making</em></p>

      <nav aria-label="Main navigation">
        <ul>
          <li><a href="index.html">Home</a></li>
          <li><a href="index.html#about">About</a></li>
          <li><a href="index.html#skills">Skills</a></li>
          <li><a href="blog.html">Blog</a></li>
          <li><a href="index.html#gallery">Gallery</a></li>
          <li><a href="index.html#links">Links</a></li>
          <li><a href="index.html#contact">Contact</a></li>
        </ul>
      </nav>
    </header>

    <main>
      <!-- ===== About Me ===== -->
      <section id="about">
        <h2>About Me</h2>
        <p>
          Hello! I am <strong>Your Name</strong>, a computer science student who
          loves building websites. This portfolio shows what I have learned
          about <em>HTML</em> so far, and I update it with every new project.
        </p>
      </section>

      <!-- ===== Skills and interests ===== -->
      <section id="skills">
        <h2>Skills and Interests</h2>

        <h3>Skills</h3>
        <ul>
          <li>HTML5 (semantic structure, forms, links, images)</li>
          <li>Git and GitHub</li>
          <li>Visual Studio Code and Chrome DevTools</li>
        </ul>

        <h3>Interests</h3>
        <ol>
          <li>Web development</li>
          <li>Open source</li>
          <li>Chess</li>
        </ol>
      </section>

      <!-- ===== Projects ===== -->
      <section id="projects">
        <h2>Projects</h2>

        <article>
          <h3>Personal Introduction Page</h3>
          <p>A resume-style page built with headings, lists, and sections.</p>
        </article>

        <article>
          <h3>Two-Page Website</h3>
          <p>A small site with working navigation and an external link.</p>
        </article>

        <p><a href="blog.html">Read my blog posts &rarr;</a></p>
      </section>

      <!-- ===== Images ===== -->
      <section id="gallery">
        <h2>Gallery</h2>

        <figure>
          <img src="images/mountain-sunset.png" alt="Purple mountain silhouettes under an orange sunset sky with a glowing sun" width="300" height="200" />
          <figcaption>Mountain sunset</figcaption>
        </figure>

        <figure>
          <img src="images/laptop-coding.png" alt="Laptop on a desk showing lines of colorful code on a dark screen" width="300" height="200" />
          <figcaption>Coding on a laptop</figcaption>
        </figure>
      </section>

      <!-- ===== Useful links ===== -->
      <aside id="links">
        <h2>Useful Links</h2>
        <ul>
          <li><a href="https://developer.mozilla.org" target="_blank" rel="noopener noreferrer">MDN Web Docs</a></li>
          <li><a href="https://validator.w3.org" target="_blank" rel="noopener noreferrer">W3C Markup Validator</a></li>
          <li><a href="https://git-scm.com/doc" target="_blank" rel="noopener noreferrer">Git Documentation</a></li>
        </ul>
      </aside>
    </main>

    <footer id="contact">
      <h2>Contact</h2>
      <address>
        Email: <a href="mailto:your.email@example.com">your.email@example.com</a><br />
        GitHub: <a href="https://github.com/your-username" target="_blank" rel="noopener noreferrer">github.com/your-username</a><br />
        Location: Your City, Country
      </address>
      <p><small>&copy; 2026 Your Name. All rights reserved.</small></p>
    </footer>
  </body>
</html>
```

## blog.html
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Blog — Your Name</title>
  </head>

  <body>
    <header>
      <img src="images/html-badge.png" alt="Orange HTML badge used as the website logo" width="60" height="40" />
      <h1>Your Name</h1>
      <p><em>Web Developer in the Making</em></p>

      <nav aria-label="Main navigation">
        <ul>
          <li><a href="index.html">Home</a></li>
          <li><a href="index.html#about">About</a></li>
          <li><a href="index.html#skills">Skills</a></li>
          <li><a href="blog.html">Blog</a></li>
          <li><a href="index.html#gallery">Gallery</a></li>
          <li><a href="index.html#links">Links</a></li>
          <li><a href="index.html#contact">Contact</a></li>
        </ul>
      </nav>
    </header>

    <main>
      <h2>Blog</h2>

      <article id="post-1">
        <h3>Why I Started Learning HTML</h3>
        <p><small>Published on <time datetime="2026-10-01">1 October 2026</time></small></p>
        <img src="images/laptop-coding.png" alt="Laptop showing colorful lines of code" width="300" height="200" />
        <p>
          HTML is the foundation of every website. In this post I explain why I
          decided to start my web development journey here.
        </p>
        <ul>
          <li>It is easy to start</li>
          <li>You see results immediately</li>
          <li>Every other web skill builds on it</li>
        </ul>
      </article>

      <article id="post-2">
        <h3>What I Learned About Semantic Tags</h3>
        <p><small>Published on <time datetime="2026-10-15">15 October 2026</time></small></p>
        <p>
          Tags like <code>header</code>, <code>nav</code>, <code>main</code> and
          <code>footer</code> give meaning to a page and help screen readers.
        </p>
      </article>

      <p><a href="index.html">&larr; Back to Home</a></p>
    </main>

    <footer id="contact">
      <h2>Contact</h2>
      <address>
        Email: <a href="mailto:your.email@example.com">your.email@example.com</a><br />
        GitHub: <a href="https://github.com/your-username" target="_blank" rel="noopener noreferrer">github.com/your-username</a><br />
        Location: Your City, Country
      </address>
      <p><small>&copy; 2026 Your Name. All rights reserved.</small></p>
    </footer>
  </body>
</html>
```

## Requirements Checklist
| Requirement | Where it is met |
|-------------|-----------------|
| Header with name/logo | `<header>` with logo image and `<h1>` |
| Navigation bar | `<nav>` with a `<ul>` of links (same on both pages) |
| About Me | `<section id="about">` |
| Skills or Interests | `<section id="skills">` (`ul` and `ol`) |
| Blog posts or projects | `#projects` on home and `<article>` posts in `blog.html` |
| Images | Logo, gallery figures, blog image — all with `alt`, `width`, `height` |
| Useful links | `<aside id="links">` (external links with `target="_blank"` and `rel`) |
| Footer with contact details | `<footer>` with `<address>`, email and GitHub links |
| Links, images, lists | All used |
| Semantic tags | `header`, `nav`, `main`, `section`, `article`, `aside`, `figure`, `footer`, `address`, `time` |
| Working navigation | Page links (`blog.html`, `index.html`) and anchors (`index.html#about`) |
| Clean, indented code | 2 spaces per level, comments per section |
| Multiple HTML files | `index.html` + `blog.html` |

## Submission
- ✅ Source code (attached) and the `images` folder
- 📸 Screenshots of both pages (optional)
- 🔗 GitHub link: `https://github.com/<your-username>/portfolio-website`
