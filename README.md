# BDC-Consulting-Website
<header class="site-header">
  <div class="container">
    <a href="/" class="logo">
      <img src="logo.png" alt="My Website Logo" />
      <span>My Website</span>
    </a>

    <nav class="nav">
      <a href="#about">About</a>
      <a href="#inventory">Inventory</a>
      <a href="#team">Team</a>
      <a href="#contact">Contact</a>
    </nav>

    <button class="menu-toggle" aria-label="Open Menu">☰</button>
  </div>
</header>

<style>
  .site-header {
    background: #0b0d10;
    border-bottom: 1px solid rgba(255,255,255,0.1);
    color: #fff;
    position: sticky;
    top: 0;
    z-index: 50;
  }
  .site-header .container {
    max-width: 1100px;
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 12px 20px;
  }
  .logo {
    display: flex;
    align-items: center;
    font-size: 1.2rem;
    text-decoration: none;
    color: #fff;
    font-weight: 600;
  }
  .logo img {
    height: 32px;
    margin-right: 8px;
  }
  .nav {
    display: flex;
    gap: 24px;
  }
  .nav a {
    color: #e7edf3;
    text-decoration: none;
    font-weight: 500;
    transition: color 0.2s;
  }
  .nav a:hover {
    color: #4aa3ff;
  }
  .menu-toggle {
    display: none;
    background: none;
    border: none;
    color: #fff;
    font-size: 1.5rem;
    cursor: pointer;
  }

  @media (max-width: 768px) {
    .nav {
      display: none;
      position: absolute;
      top: 60px;
      left: 0;
      width: 100%;
      background: #12161b;
      flex-direction: column;
      align-items: center;
      padding: 10px 0;
      border-top: 1px solid rgba(255,255,255,0.1);
    }
    .nav.active {
      display: flex;
    }
    .menu-toggle {
      display: block;
    }
  }
</style>

<script>
  document.querySelector(".menu-toggle").addEventListener("click", () => {
    document.querySelector(".nav").classList.toggle("active");
  });
</script>
