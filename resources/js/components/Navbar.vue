<template>
 <nav class="navbar navbar-expand-md nav-bg fixed-top">
    <button class="navbar-toggler navbar-toggler-right" type="button" data-toggle="collapse" data-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
    </button>
    <a class="navbar-brand" href="#">
        <img src="../../assets/logo.png" width="30" height="30" class="d-inline-block align-top" alt="">
        <span class="menu-collapsed">FAS</span>
    </a>
    <div class="collapse navbar-collapse" id="navbarNavDropdown">
        <ul class="navbar-nav">
            <li class="nav-item active">
          <router-link class="nav-link" to="/">Home</router-link>
            </li>
            <li class="nav-item">
          <router-link class="nav-link" to="/about">About</router-link>
            </li>
            <li class="nav-item">
                <a class="nav-link" to="">Log-out</a>
            </li>

            <!-- This menu is hidden in bigger devices with d-sm-none. 
           The sidebar isn't proper for smaller screens imo, so this dropdown menu can keep all the useful sidebar itens exclusively for smaller screens  -->
            <li class="nav-item dropdown d-sm-block d-md-none">
                <a class="nav-link dropdown-toggle" href="#" id="smallerscreenmenu" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                  Menu
                </a>
                <div class="dropdown-menu" aria-labelledby="smallerscreenmenu">
                    <a class="dropdown-item" href="#">Dashboard</a>
                    <a class="dropdown-item" href="#">Profile</a>
                    <a class="dropdown-item" href="#">Tasks</a>
                    <a class="dropdown-item" href="#">Etc ...</a>
                </div>
            </li>
            <!-- Smaller devices menu END -->

        </ul>
    </div>
</nav>
</template>
<style>
.nav-link {
  color: #fff !important;
}

.navbar-brand {
  color: #fff !important;
}

.nav-bg {
  background-color: #462478;

}

.navbar-toggler-icon {
  color: #fff !important;
}
</style>
<script>
export default {
  name: "Navbar"
}
</script>

