<div class="menu">
  <ul>
    <li><a href="link">Shop</a></li>
    <li><a href="link">About</a></li>
    <li><a href="link">Stockists</a></li>
    <li><a href="link">Contact</a></li>
  </ul>
</div>

<style>
  /* Media query for tablet and mobile screens */
  @media (max-width: 768px) {
    .menu {
      display: none;
    }
  }
  ul {
    list-style: none;
    display: flex;
    gap: 1.6rem;
    font-size: 1.125rem;
    justify-content: center;
    padding-left: 0;
  }

  li {
    font-weight: 300;
    text-decoration: none;
    color: #000000;
  }

  a {
    text-decoration: none;
    color: inherit;
  }
</style>
