<template>
   <b-row align-h="center"  class="">

    <b-col cols="11"   md="10" lg="10" class="">
      <div class="bg-white rounded shadow p-2">

        <img :src="require(`~/assets/img/${img}`)" class="slider" alt="icon"/>

        <div class="d-flex flex-wrap-reverse justify-content-end  mt-3">

          <div class="d-flex mt-3">
            <img :src="require(`~/assets/icon/star.png`)" class="icon" alt="icon"/>
            <img :src="require(`~/assets/icon/star.png`)" class="icon" alt="icon"/>
            <img :src="require(`~/assets/icon/star.png`)" class="icon" alt="icon"/>
            <img :src="require(`~/assets/icon/star.png`)" class="icon" alt="icon"/>
            <img :src="require(`~/assets/icon/star2.png`)" class="icon" alt="icon"/>

          </div>
          <div class="text_Purple text-right mx-3 mt-2">
            <p class="font-weight-bolder f_18 my-0">اسم البائع</p>
            <p>+966598398</p>
          </div>

          <img :src="require(`~/assets/img/personthree.png`)" class="img my-0" alt="icon"/>

        </div>

        <p class="font-weight-bolder text-right f_22"> شراء مجموعة من السيارات من موديلات1990</p>
        <p class="text-right text_GrayTHr">code 1234</p>

        <div class="d-flex  flex-wrap-reverse we">

          <form class="d-flex justify-content-between align-items-center mt-2">
            <button class="btn rounded bg_Pink mr-2 text-white" type="submit">تأكيد</button>
            <input type="text" class="form-control text-right rounded" placeholder="اكتب المبلغ">
          </form>

          <div class="d-flex flex-wrap-reverse mt-2 ">
            <div class="bg_LightPink p-2 mt-1"><p class="text_Pink f_18 m-0">+10020</p></div>
            <div class="bg_LightPink p-2 mx-2 mt-1"><p class="text_Pink f_18 m-0">+10010</p></div>
            <div class="bg_LightPink p-2 mt-1"><p class="text_Pink f_18 m-0">+10000</p></div>
          </div>



        </div>

        </div>
    </b-col>
    <b-col cols="11"  md="2" lg="2" class="p-0 m-0 Group">
      <div class="bg-white shadow mx-auto w_fit p-1 pb-0 mb-2 d-flex justify-content-center align-items-center " v-on:click="Next()" >
        <img :src="require(`~/assets/icon/arrow.png`)" class="rounded  mx-auto rotate" alt="icon"/>
      </div>
      <img v-for="img in Slider" :key="img.id" v-on:click="Show(img.name)" :src="require(`~/assets/img/${img.name}`)" class="SideSlider rounded mb-2" alt="icon"/>
      <div class="bg-white shadow mx-auto w_fit p-1 pb-0 mb-2 d-flex justify-content-center align-items-center " v-on:click="Pre()" >
        <img :src="require(`~/assets/icon/arrow.png`)" class="rounded  mx-auto rotatetwo" alt="icon"/>
      </div>
    </b-col>
   </b-row>

</template>

<script>

export default ({
  data() {
    return {
      img:'slider.png',
      AllSlider :[
        {id:1, name:'slider.png'},
        {id:2, name:"download.jpeg"},
        {id:3, name:"download (1).jpeg"},
        {id:4, name:"download (2).jpeg"},
        {id:5, name:"download (3).jpeg"},
        {id:6, name:"download (4).jpeg"},
        {id:7, name:"download (5).jpeg"},

      ],
      Slider :[],
      min: 0,
      max: 5
    };
  },
  mounted(){
    this.AllSlider.forEach(ele => {
      if(ele.id > this.min && ele.id < this.max){
        this.Slider.push(ele)
      }

    });
  },
  methods:{
    Show(img){
      this.img = img
    },
    Next(){
      this.min = this.min + 1
      this.max = this.max+1
      if(this.min <4){
        this.Slider = []
        this.AllSlider.forEach(ele => {
         if(ele.id > this.min && ele.id < this.max){
           this.Slider.push(ele)
         }

        });
      }else{
        this.min = 0
      this.max = 5
        this.Slider = []
        this.AllSlider.forEach(ele => {
         if(ele.id > this.min && ele.id < this.max){
           this.Slider.push(ele)
         }

        });
      }


    },
    Pre(){
      this.min = this.min + 1
      this.max = this.max+1
      if(this.min <4){
        this.Slider = []
        this.AllSlider.forEach(ele => {
         if(ele.id > this.min && ele.id < this.max){
           this.Slider.push(ele)
         }

        });
      }else{
        this.min = 0
      this.max = 5
        this.Slider = []
        this.AllSlider.forEach(ele => {
         if(ele.id > this.min && ele.id < this.max){
           this.Slider.push(ele)
         }

        });
      }

    }
  }
})
</script>


<style scop>
.img{
  width: 60px;
  height: 60px;
}
.icon{
  width:15px;
  height:15;
  margin-left: 5px;
}
.slider{
  width: 100%;
  height: 350px;
}
.SideSlider{
  width: 100%;
  height: 100px;
  cursor: pointer;
}
.w_fit{
  width: fit-content;
  cursor: pointer;
}
.rotate{
  transform: rotate(180deg) ;
}
.Group{
  display: flex;
  flex-direction: column;
}
.we{
  justify-content: space-between !important;
}

@media screen and  (max-width:750px) and (min-width:567px) {
  .we{
   justify-content: end !important;
  }
}
@media (max-width:767px) {
  .Group{
    margin: 20px !important;
    display: flex;
    flex-direction: row;
  }
  .SideSlider{
    width: 20%;
    height: 80px;
    margin: 0 5px;
  }
  .rotate{
    transform: rotate(90deg) ;
  }
  .rotatetwo{
    transform: rotate(270deg) ;
  }
  .slider{
  width: 100%;
  height: 250px;
}
.we{
  justify-content: end !important;
}
}
</style>
