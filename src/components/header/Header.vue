<template>
    <header class="header">
      <h1>{{ title }}</h1>
      <nav>
        <ul>
          <li><a href="/">Home</a></li>
          <li><a href="/about">About</a></li>
          <li><a href="/contact">Contact</a></li>
        </ul>
      </nav>
    </header>
  </template>
  
  <script>
  export default {
    name: 'Header',
    props: {
      title: {
        type: String,
        default: 'My App'
      }
    }
  }
  </script>
  
  <style scoped>
  .header {
    background-color: #f8f9fa;
    padding: 10px;
    border-bottom: 1px solid #e1e1e1;
  }
  
  .header h1 {
    margin: 0;
    font-size: 24px;
  }
  
  .header nav ul {
    list-style-type: none;
    padding: 0;
    margin: 0;
    display: flex;
  }
  
  .header nav ul li {
    margin-right: 15px;
  }
  
  .header nav ul li a {
    text-decoration: none;
    color: #007bff;
  }
  
  .header nav ul li a:hover {
    text-decoration: underline;
  }
  </style>
  