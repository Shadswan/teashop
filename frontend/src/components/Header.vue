<template>
  <header class="main-header">
  <div>
    <p>Icon</p>
  </div>
  <div class="search-menu">
    <a @click="showSearchField">Teashop</a>
    <transition>
      <a v-if="show">Поисковая строка</a>
    </transition>
  </div>
  <div class="profile">
    <img src="../picture/user.png">
    <a>Профиль</a>
  </div>
  </header>
</template>

<script setup>
  function showSearchField() {
    var show;
    show = !show;
  }
</script>

<style lang="scss">
.main-header
{
  background-color: #696969;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  border-radius: 5px;
  align-items: center;
}

.search-menu{
  color: white;
  font-family: "Playfair Display", serif;
  font-size: 3vh;
}

.search-menu:hover{
  color: red;
}

.profile
{
  font-family: "Rubik", sans-serif;
  margin: 5px;
  padding: 5px;
  align-items: center;
  background-color: white;
  display: flex;
  flex-direction: column;
  border-radius: 5px;
  img{
    width: 100%;
    max-width: 50px;
    height: auto;
  }
}
</style>
