<template>
  <div id="app">
    
    <!-- Nav bar -->
    <b-navbar toggleable="md" type="dark"  class="bg-dark" >

        <b-container >

          <b-navbar-brand href="#" ><b-icon-bootstrap/>BootstrapVue</b-navbar-brand>
          <b-navbar-toggle target="nav-collapse" ></b-navbar-toggle> 

          <b-collapse is-nav id="nav-collapse">

            <b-navbar-nav >
              <b-nav-item to="/"> Home</b-nav-item>
              <b-nav-item to="form" >Form</b-nav-item>
              <b-nav-item to="iconos"> Iconos</b-nav-item>
            </b-navbar-nav>


          </b-collapse>
        
        </b-container>

    </b-navbar>
    <!-- Nav bar -->



        <b-container>
              <router-view/>
        </b-container>


  </div>
</template>
