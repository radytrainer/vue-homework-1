<template>
  <div id="app" class="box-shadow-lg">
    <nav class="navbar navbar-expand-lg navbar-light bg-light shadow-custom">
      <div class="container-fluid">
        <a class="navbar-brand" href="#">Kimo App</a>
        <button
          class="navbar-toggler"
          type="button"
          data-bs-toggle="collapse"
          data-bs-target="#navbarNav"
          aria-controls="navbarNav"
          aria-expanded="false"
          aria-label="Toggle navigation"
        >
          <span class="navbar-toggler-icon"></span>
        </button>
        <div class="collapse navbar-collapse" id="navbarNav">
          <ul class="navbar-nav">
            <li class="nav-item">
              <router-link class="nav-link" to="/">Home</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/about">About</router-link>
            </li>
            <li class="nav-item">
              <router-link class="nav-link" to="/service">Services</router-link>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    
  </div>
  <div class="container mt-4">
    <router-view></router-view>
  </div>
</template>
  
  <script>
export default {
  name: "App",
};
</script>
  
  <style>
/* Add any global styles here */
.shadow-custom {
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}
</style>