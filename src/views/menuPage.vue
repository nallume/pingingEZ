<template>
  <header>
    <div class="nav">
      <ul>
        <li><router-link to="/">게시판1</router-link></li>
        <li>게시판2</li>
        <li>게시판3</li>
        <li>게시판4</li>
        <li>게시판5</li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name:'menuPage'
}
</script>

<style>
  header{
    height: 50px;
  }
  .nav{
    position:fixed;
    top:0;
    width:100%;
    height:30px;
    background-color: #c1c1c1;
  }
  ul{
    margin:0;
    padding: 0;
  }
  li{
    list-style: none;
    float:left;
    width:100px;
    height:100%;
    line-height: 30px;
    text-align: center;
  }
  li:hover{
    font-weight: bold;
  }
</style>