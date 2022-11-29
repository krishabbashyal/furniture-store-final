<template>

    <div class="topnav">
        <h1>Store Name</h1>
        <div class="select-buttons">
            <a class="active" href="#home">Home</a>
            <a href="#news">Upcoming</a>
            <a href="#about">About</a>
            <a href="https://github.com/krishabbashyal/furniture-store-final" target="_blank">GitHub</a>
        </div>

    </div>
</template>

<script>
export default {
    name: 'Header',
}
</script>

<style scoped>

.topnav {
  overflow: hidden;
  display: flex;
  justify-content: center;
  border: 1px solid gray;
  font-weight: bold;
}

h1 {
    display: flex;
    width: 70%;
    padding-top: 5px;
    font-size: 35px;
}

.topnav a {
  float: left;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
  font-size: 17px;
}

.topnav a:hover {
  background-color: #00c97f;
}

.topnav a.active {
  background-color: #005838;
  color: white;
}

</style>