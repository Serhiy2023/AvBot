<script>
  import { goto } from '$app/navigation';
 </script>

  <header class="main-header">
      <a href="/" class="header-logo">
          <img src="/images/logo.jpg" alt="" class="logo-img">
          <span class="logo-text">AvBot.<span class="logo-org">org</span></span>
          
      </a>
      
      <nav class="main-menu">
        <a on:click={() => goto('/')}>How To Start a Business</a>
        <a on:click={() => goto('/LLC')}>How To Start an LLC</a>
        <a on:click={() => goto('/Registered_Agent')}>US Registered Agent</a>
    </nav>
  </header>

<slot /> 


<style>
 
 .main-menu {
    display: flex;
    gap: 20px;
    padding: 10px;
    
  }
  
  .main-header {
  display: flex;
  justify-content: space-between;  
  align-items: center;
  padding: 8px 120px;
  background: #FFFFFF;
  border-bottom: 1px;
  font-family: 'Roboto', sans-serif;
}

/* Логотип */
.header-logo {
  display: flex;
  align-items: center;
  text-decoration: none;
}

.logo-img {
  width: 80px; 
  height: auto;
  border-color: #FFFFFF;
 
}

.logo-text {
  color: #22222B;
  font-size: 48px;
  font-weight: bold;
  
}
.logo-org {
  color: #5856D6;
}

nav a {
      cursor: pointer;
      text-decoration: none;
      color: #636364;
      font-size: 16px;
  }

nav a:hover {
      color: #5856D6;
  }
</style>



