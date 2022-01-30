<template>
  <div id="app">
   
    <b-navbar toggleable="md" type="dark" variant="danger">
      <b-container>

        <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
        <b-navbar-brand href="#">NavBar</b-navbar-brand>
        
        <b-collapse is-nav id="nav-collapse">
          <b-navbar-nav>
            <b-nav-item to="/" exact>Home</b-nav-item>
            <b-nav-item to="/about">About</b-nav-item>
            <b-nav-item to="/grid">Grid</b-nav-item>
            <b-nav-item to="/card">Card</b-nav-item>
            <b-nav-item to="/form">Form</b-nav-item>
          </b-navbar-nav>
        </b-collapse>

      </b-container>

    </b-navbar>
      <!-- <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link> -->
    <b-container>
      <router-view/>
    </b-container>
   
  </div>
</template>
