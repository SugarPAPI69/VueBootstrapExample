<template>
  <div class="hello">
  

    <div class="name">
      <div class="letter">
        <img src="../assets/img/crash.png" class="letter-image">
        <p>First Game ive ever played  still holds up[ til this day- Ricky Brain </p>
      </div>
      <div class="letter">
        <img src="../assets/img/drake.png" class="letter-image">
        <p>Tomb Raider Clone lol, First entry on my favourite video game series (Made by Naughtydog same devs on that crash game)- Ricky Brain </p>
      </div>
      <div class="letter">
        <img src="../assets/img/gta.jpg" class="letter-image">
      </div>
      <div class="letter">
        <img src="../assets/img/pacman.jpg" class="letter-image">
      </div>
      <div class="letter">
        <img src="../assets/img/lol.jpg" class="letter-image">
      </div>
      
    </div>
    
  </div>
</template>

<script>
export default {
  name: 'Home',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.name {
  display: flex;
  align-items: center;
  justify-content: center;
  vertical-align: middle;
  width: 100vw;
  height: calc(100vh - 60px);
}
.letter {
  margin: .8%;
  filter: drop-shadow(0px 0px 7px rgba(150, 150, 150, .7));
}
.letter-image {
  width: 100%;
}

.menu {
  display: flex;
  align-items: center;
  justify-content: space-around;
  margin-top: 10px;
  height: 60px;
}

.menu-item {
  flex: 1;
  text-align: center;
  display: flex;
  justify-content: center;
  align-items: center;
}

.menu-text{
  font-size: 20px;
  color: #818181;
  cursor: pointer;
  padding: 10px;
  border-bottom: 2px solid #080808;
  width: fit-content;
}

.menu-text:hover {
  border-bottom: 2px solid #c278ff;
}

.menu-center {
  font-size: 36px;
  color: #EAEAEA;
}
</style>

