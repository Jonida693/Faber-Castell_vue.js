<template>
  <section class="payments-section">
    <div class="icon-section row ">
      <div class=" col-md-3" v-for="pay in pay" :key="pay" href="*">
        <div class="total-content" >
          <div class="icon-footer">
            <img alt="" :src="pay.img" />
          </div>

          <div class="content">
            <h4>{{ pay.content }}</h4>
          </div>
        </div>

        

      </div>
    </div>
  </section>
</template>

<script>
export default {
  data: () => {
    return {
      pay: [
        {
          //First
          id: "0",

          img: "https://www.faber-castell.de/-/media/Faber-Castell-new/icons/Zahlarten_Icon.ashx?h=40&w=50&la=de-DE&hash=CDB85BC8D9F9D98C9AE92F037AB7C972CA96A8CE",
          content:
            "PayPal | Rechnung | Vorauskasse | Sofortüberweisung | Mastercard | Visa",
        },

        //second pay

        {
          id: "1",

          img: "https://www.faber-castell.de/-/media/Faber-Castell-new/icons/versand.ashx?h=32&w=50&la=de-DE&hash=BF5365582B02420ED44B44E41562B5E037DD42F9",
          content:
            "Kostenloser Versand ab 39€",
        },
        //third pay

        {
          id: "2",

          img: "https://www.faber-castell.de/-/media/Faber-Castell-new/icons/reshipment.ashx?h=37&w=50&la=de-DE&hash=3B28EF62D1FF87B193F2A742DC8394A9C32BF636",
          content:
            "Kostenloser Rückversand",
        },
        //fourth pay
        {
          id: "3",

          img: "https://www.faber-castell.de/-/media/Faber-Castell-new/icons/Secure_Icon.ashx?h=37&w=50&la=de-DE&hash=99D04CE0BC9831590E305B28DCD7268923999365",
          content:
            "SSL Verschlüsselung zum Schutz Ihrer Daten",
        },
      ],
    };
  },
};
</script>

<style lang="scss">
.payments-section{
background-color: white;
    padding-top: 30px;
    padding-bottom: 30px;
   



    .icon-section{
           
             padding-top: 30px;
            max-width: 1280px;
    margin: 0 auto;
     border-top: 1px solid #e2e3e3;
    }
    .total-content {
    display: flex;
        align-items: center;

 
    img{
        height: auto;
    padding: 4px 4px 0 0;
        width: 40px;
    }
    h4{
    /* width: 46%; */
    font-weight: normal;
        color: #05301a;
    font-family: Arial,Helvetica,sans-serif;
    font-size: 16px;
    line-height: 21px;
    margin: 0;
    padding: 0
 
    
    
    }
    
   
}

}

</style>
