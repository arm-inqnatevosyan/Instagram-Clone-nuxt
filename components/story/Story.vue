<template>
  <div class="story">
    <div id="one-block">
      <img src="/insta8.jpg" alt="">
      <div>
        <i id="add" class="fa-solid fa-circle-plus" />
      </div>
      <p>Your Story</p>
    </div>
    <div>
      <img src="/insta1.webp" alt="">
      <p>axelbeyon</p>
    </div>
    <div>
      <img src="/insta2.jpg" alt="">
      <p>simson</p>
    </div>
    <div>
      <img src="/insta3.jpg" alt="">
      <p>ico.wooy</p>
    </div>
    <div>
      <img src="/insta4.webp" alt="">
      <p>louwsers</p>
    </div>
    <div>
      <img src="/insta5.jpg" alt="">
      <p>tinanakey</p>
    </div>
    <div>
      <img src="/insta6.jpg" alt="">
      <p>robincield</p>
    </div>
    <div>
      <img src="/insta7.jpg" alt="">
      <p>arnauld</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'StoryVue'
}
</script>
<style scoped>
.story {
  width: 78%;
  height: auto;
  display: flex;
  justify-content: space-evenly;
  margin: 30px auto 0;
  overflow: hidden;
}

.story img {
  width: 60px;
  height: 60px;
  border-radius: 50% 50%;
  object-fit: cover;
}

.story p {
  font-size: 13px;
  font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}

#one-block {
  position: relative;
}

#add {
  position: absolute;
  bottom: 20%;
  color: rgb(52, 157, 228);
  right: -10%;
  font-size: 20px;
}

@media (max-width: 992px) {
  .story {
    width: 100%;
    display: flex;
    justify-content: center;
  }

  .story img {
    width: 50px;
    height: 50px;
    margin: 0 auto !important;
  }

  .story p {
    font-size: 10px;
  }
  .story div{
    margin-left: 20px !important;
  }
}

@media (max-width: 576px) {
  .story {
    display: grid;
    grid-template-columns: repeat(4, 0.11fr);
    grid-gap: 10px;
    width: 100%;
    margin: 0 auto;
  }
  .story div{
    width: 70px;
  }
  .story img {
    width: 30px;
    height: 30px;
    margin: 0 auto !important;
  }
  .story div{
    margin-left: 10px !important;
    margin: 0px auto;
  }
}
</style>
