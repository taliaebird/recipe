<template>
<div id="app">
  <div class="header">
    <router-link to="/">
    </router-link>
    <div class="title">
      <h1><strong><em>Recipe Collection</em></strong></h1>
    </div>
    <div class="subtitle">
      <a class="page-links" href='http://localhost:8080/'>
        <h3>Collection</h3>
      </a>
      <a class="page-links" href='http://localhost:8080/admin'>
        <h3>Add/Edit Recipes</h3>
      </a>
    </div>
  </div>
  <div class="content">
    <router-view />
  </div>
  <a href='https://github.com/taliaebird/recipe.git'>
  <div class="footer">
    GitHub
  </div>
  </a>
</div>
</template>

<style>
html {
  box-sizing: border-box;
}

body {
  font-family: 'Space Mono', sans-serif;
  font-size: 16px;
  background: #fff;
  padding: 0px;
  margin: 0px;
}

/* Header */
.header {
  display: flex;
  flex-wrap: wrap;
  width: 100%;
  color: #1C454F;
  text-align: center;
}

.title {
  width: 100%;
  height: 110px;
  font-family: 'Space Mono';
}

.title h1 {
  font-size: 40px;
  color: #002A53;
}
.subtitle {
  display: flex;
  flex-wrap: wrap;
 width: 100%;
 background-color: lightblue;
}
.page-links {
  height: 70px;
  width: 50%;
  background-color: lightblue;
}
a, a:visited {
  font-family: 'Space Mono';
  color: #696969;
  text-decoration: none;
}
.page-links a:hover, a:visited:hover {
  background-color: red;
  color: white;
}

a:hover, a:visited:hover {
  color: white;
}

.content {
  padding: 20px 100px;
  min-height: 500px;
}

/* Footer */
.footer {
  height: 50px;
  padding: 20px 100px 0px 100px;
  background-color: #e3e3e3;
  font-size: 12px;
  text-align: center;
}

h1 {
  font-size: 20px;
}

h2 {
  font-size: 14px;
}
</style>
