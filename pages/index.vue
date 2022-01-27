<template>
  <div>
    <!-- aqui vai nosso html -->
    <section class="home">
      <div class="block">
        <div class="title">
          Solução <br>completa para <br>benefícios sociais
        </div>
        <p class="text">
          Temos soluções modularizadas para prefeituras no auxílio de pagamento de benefícios para pessoas em situação de vulnerabilidade.
        </p>
      </div>
    </section>
    <section class="about">
        <div class="container">
          <div class="title">
          Benefity <br> Soluções para benefícios sob demanda
        </div>
        <div class="container-block">
            <Bloco/>
            <Bloco/>
            <Bloco/>
        </div>
        </div>
    </section>
  </div>
</template>
<script>
// aqui vai nosso script
</script>
<style lang="scss" scoped>
section.home{
  max-width: 1280px;
  margin: 0 auto;
width: 100%;
.block{
  width: 50%;
  .title{
    max-width: 100%;
    font-size: 3rem;
    font-weight: 700;
    color: rgb(255, 255, 255);
    margin:60px 0 40px 0 ;
  }
  .text{
    max-width: 450px;
     color: rgb(233, 233, 233);
      padding:5px 0 80px 0 ;
         font-size: 1.2rem;
         line-height: 30px;
  }
}
 @media screen and (max-width:1000px) {

    padding: 0 90px;

  }
}
section.about{
  background: rgb(235, 235, 235);
padding: 10px 0 90px 0;
  width: 100%;
  .title{
    text-align: center;
   color: #3a3161;
    font-size: 2rem;
    padding: 30px 0;
    font-weight: bold;
  }
  .container{
      display: block;
        max-width: 1280px;
  margin: 0 auto;
    }
  .container-block{
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap:wrap ;
  }
  @media screen and (max-width:1000px) {

     .container-block{
    flex-direction: column;
    gap: 20px;
     }
  }
}
</style>
