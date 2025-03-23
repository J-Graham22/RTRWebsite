<script>
  const navItems = [
    { name: "Games", href: "/Games" },
    { name: "Software", href: "/Software" },
    { name: "Music", href: "/Music" },
    { name: "eSports", href: "/eSports" },
    { name: "Literature", href: "/Literature" },
  ];
</script>

<nav class="navbar">
  <div class="navbar-container">
    <div class="navbar-logo">
      <a href="/">Remember the Ravens</a>
    </div>
    
    <div class="navbar-menu">
      {#each navItems as item}
        <a href={item.href} class="navbar-item">{item.name}</a>
      {/each}
    </div>
  </div>
</nav>

<style>
  .navbar {
    background-color: #333;
    color: white;
    width: 100%;
    height: 60px;
  }
  
  .navbar-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 100%;
    padding: 0 20px;
    max-width: 1200px;
    margin: 0 auto;
  }
  
  .navbar-logo a {
    color: white;
    text-decoration: none;
    font-weight: bold;
    font-size: 1.2rem;
  }
  
  .navbar-menu {
    display: flex;
    gap: 20px;
  }
  
  .navbar-item {
    color: white;
    text-decoration: none;
    padding: 5px 10px;
    border-radius: 4px;
    transition: background-color 0.2s;
  }
  
  .navbar-item:hover {
    background-color: rgba(255, 255, 255, 0.1);
  }
  
  /* For responsive design */
  @media (max-width: 768px) {
    .navbar-container {
      flex-direction: column;
      padding: 10px;
    }
    
    .navbar {
      height: auto;
    }
    
    .navbar-menu {
      margin-top: 10px;
    }
  }
</style>
