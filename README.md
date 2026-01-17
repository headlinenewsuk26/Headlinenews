headlinenewsuk26/
│
├─ index.html
├─ about.html
├─ contact.html
├─ news/
│   ├─ uk-featured.html
│   ├─ usa-news.html
│   ├─ uk-news.html
│   └─ europe-news.html
└─ css/
    └─ style.css
    <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Latest global and UK news, updates, and reports. Stay updated with breaking news from USA, UK, Europe, Asia, and worldwide.">
  <title>HeadlineNews UK.26</title>
  <link rel="stylesheet" href="css/style.css">
  <link rel="icon" href="favicon.ico" type="image/x-icon">
</head>
<body>

<header>
  <h1>HeadlineNews UK.26</h1>
  <nav>
    <a href="index.html">Home</a>
    <a href="about.html">About</a>
    <a href="contact.html">Contact</a>
  </nav>
</header>

<div class="ticker">
  Breaking: UK Parliament discusses new economic policy | US-China trade tensions rise | Europe climate summit updates
</div>

<main class="container">

  <section class="featured">
    <article>
      <h2><a href="news/uk-featured.html">UK Economic Policy Update 2026</a></h2>
      <p>The UK government has introduced new fiscal measures aimed at boosting growth and stability...</p>
    </article>
  </section>

  <section class="latest-news">
    <h2>Latest News</h2>

    <article class="article-card">
      <h3><a href="news/usa-news.html">US Elections 2026: Latest Updates</a></h3>
      <p>Breaking updates from the United States elections, latest polls and campaign news...</p>
    </article>

    <article class="article-card">
      <h3><a href="news/uk-news.html">UK Parliament Votes on Climate Bill</a></h3>
      <p>UK lawmakers have voted in favor of a new climate policy aimed at reducing emissions...</p>
    </article>

    <article class="article-card">
      <h3><a href="news/europe-news.html">Europe Summit Highlights</a></h3>
      <p>Major European nations discussed trade, climate, and security policies at the annual summit...</p>
    </article>

  </section>

  <aside class="sidebar">
    <h3>Trending</h3>
    <ul>
      <li><a href="#">Global Stock Markets Today</a></li>
      <li><a href="#">UK Housing Market Trends</a></li>
      <li><a href="#">Tech Innovations in Europe</a></li>
    </ul>
  </aside>

</main>

<footer>
  <p>&copy; 2026 HeadlineNews UK.26. All rights reserved.</p>
</footer>

</body>
</html>
body {
  font-family: Arial, sans-serif;
  line-height: 1.6;
  margin: 0;
  padding: 0;
  background: #f4f4f4;
}

header {
  background: #003366;
  color: white;
  padding: 15px 20px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
header h1 {
  margin: 0;
  font-size: 1.8em;
}
nav a {
  color: white;
  margin: 0 15px;
  text-decoration: none;
  font-weight: bold;
}
nav a:hover {
  text-decoration: underline;
}

/* Breaking News Ticker */
.ticker {
  background: #d32f2f;
  color: white;
  padding: 8px 15px;
  font-weight: bold;
  overflow: hidden;
  white-space: nowrap;
  animation: ticker 20s linear infinite;
}
@keyframes ticker {
  0% { transform: translateX(100%); }
  100% { transform: translateX(-100%); }
}

main.container {
  display: flex;
  flex-wrap: wrap;
  padding: 20px;
  gap: 20px;
}

/* Featured Section */
.featured article {
  background: white;
  padding: 20px;
  border-radius: 8px;
  width: 100%;
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

/* Latest News Section */
.latest-news {
  flex: 3;
}
.article-card {
  background: white;
  padding: 15px;
  margin-bottom: 15px;
  border-radius: 5px;
  box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}
.article-card h3 a {
  color: #003366;
  text-decoration: none;
}
.article-card h3 a:hover {
  text-decoration: underline;
}

/* Sidebar */
.sidebar {
  flex: 1;
  background: #f5f5f5;
  padding: 15px;
  border-radius: 5px;
  height: fit-content;
}
.sidebar h3 { margin-top: 0; }
.sidebar ul { list-style: none; padding: 0; }
.sidebar ul li { margin-bottom: 10px; }
.sidebar ul li a { text-decoration: none; color: #003366; }
.sidebar ul li a:hover { text-decoration: underline; }

/* Footer */
footer {
  background: #003366;
  color: white;
  text-align: center;
  padding: 10px 0;
  margin-top: 20px;
}

/* Responsive */
@media (max-width: 900px) {
  main.container { flex-direction: column; }
  .sidebar { width: 100%; }
}
