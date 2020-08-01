<template>
  <div class="container">
    <div class="row">
      <div class="col-xs-12">
        <header>
          <h1>Sunucu Durumu</h1>
        </header>
      </div>
    </div>
    <hr>
    <div class="row">
      <div class="col-xs-12 col-sm-6">
        <ul class="list-group">
          <li
            class="list-group-item"
            :key="index"
            v-for="index in 5">
            Sunucu #{{ index }}
          </li>
        </ul>
      </div>
      <div class="col-xs-12 col-sm-6">
        <p>Sunucu Bilgisi güncel değil!!</p>
      </div>
    </div>
    <hr>
    <div class="row">
      <div class="col-xs-12">
        <footer>
          <p>Tüm Hakları Saklıdır | varolmaksutoglu.com</p>
        </footer>
      </div>
    </div>
  </div>
</template>

<script>
</script>

<style>

</style>
