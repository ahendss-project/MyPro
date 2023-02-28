<template>
    <header class="header">
      <h1>{{ pageTitle }}</h1>
      <nav>
        <ul>
          <li><router-link to="/">Home</router-link></li>
          <li><router-link to="/about">About</router-link></li>
          <li><router-link to="/contact">Contact</router-link></li>
        </ul>
      </nav>
    </header>
  </template>
  
  <script>
  export default {
    name: "app-header",
    props: {
      pageTitle: {
        type: String,
        required: true
      }
    }
  };
  </script>
  
  <style>
  .header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem;
    background-color: #f2f2f2;
    border-bottom: 1px solid #ccc;
  }
  
  nav ul {
    list-style: none;
    display: flex;
    gap: 1rem;
  }
  
  nav ul li {
    font-size: 1.2rem;
  }
  </style>