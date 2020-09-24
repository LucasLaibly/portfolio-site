<!--script-->
<script>
    export let navlists = [];
    export let header;
</script>

<!--markup-->
<section id="nav-bar">
    <nav class="navbar nar-bar">
        <a class="" href='/' style="padding-right:12%">
            <span style="font-weight:bold">{header}</span> | coder
        </a>

      <div class="nav-bar" id="navbarNav" style="padding-left:80%">
        <ul class="navbar-nav">
          {#each navlists as list}
            <li class="nav-item">
              <a href={list.url}>{list.label}</a>
            </li>
          {/each}
        </ul>
      </div>
    </nav>

</section>

<!--style-->
<style>
  #body {
    margin: 0px;
    border: 0px;
    padding: 0px;
    font-family: Arial, Helvetica, sans-serif;
  }

  #nav-bar {
    overflow: hidden;
    background-color: #333;
  }

  .navbar a {
    float: left;
    color: #f2f2f2;
    text-align: center;
    padding: 14px 16px;
    text-decoration: none;
    font-size: 17px;
  }

  .navbar-nav li a:hover {
    background-color: #ddd;
    color: black;
  }

  .navbar-nav li a.active {
    background-color: #24a4d6;
    color: white;
  }
</style>
