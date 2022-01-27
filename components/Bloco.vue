<template>
  <div class="container">
    <div class="title">Integração com instituições governamentais</div>
    <div class="description">Temos soluções para ajudar prefeituras a distribuir renda para pessoas em vulnerabilidade</div>
  </div>
</template>
<style lang="scss" scoped>
div.container{
  width: calc((100% / 3) - 90px);
  height: 100%;
  background: rgb(255, 255, 255);
  margin: 10px;
  border: 1px solid rgb(214, 214, 214);
  padding: 30px 30px;
  .title{
    padding: 20px;
    font-size: 1.4rem;
    font-weight: bold;
    color: #3a3161;
  }
  .description{
        color: #575a73;
    font-size: 1.2rem;
    line-height: 30px;
    padding: 20px;
     max-width: 290px;
  }
  &:hover{
    transform: scale(1.01);
    -webkit-box-shadow: 1px 2px 19px -1px #7A7A7A;
box-shadow: 1px 2px 19px -1px #7A7A7A;
cursor: pointer;
  }
  @media screen and (max-width:1000px) {
   width: 90%;
  }
}
</style>
