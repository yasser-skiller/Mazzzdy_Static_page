<template>
  <div class="bg-white rounded shadow p-3 mt-5">

    <h3 class="text-right font-weight-bold">المزادات الممفضلة</h3>

    <div class="d-flex justify-content-end  w-100 mt-4 sp">
      <div class="">
        <p class="text-right font-weight-bold">سيارة سريعة بى ام دابليو تصنيع 2021 حالته جديدة سيارة سريعة بى ام دابليو تصنيع 2021 حالته جديدة</p>
        <div class="d-flex justify-content-between">
          <p class="text_PurpleSec font-weight-bold">$   500</p>
          <div class="d-flex">
          <p class="mr-2">أعلي سعر</p>
            <img :src="require(`~/assets/icon/price.png`)" class="icon" alt="icon"/>
          </div>
        </div>
      </div>

      <div class="ml-2">
        <img :src="require(`~/assets/img/CompositeLayer.png`)" class="img" alt="icon"/>
      </div>
    </div>


    <div class="d-flex justify-content-end  w-100 mt-4 sp">
      <div class="">
        <p class="text-right font-weight-bold">سيارة سريعة بى ام دابليو تصنيع 2021 حالته جديدة سيارة سريعة بى ام دابليو تصنيع 2021 حالته جديدة</p>
        <div class="d-flex justify-content-between">
          <p class="text_PurpleSec font-weight-bold">$   500</p>
          <div class="d-flex">
          <p class="mr-2">أعلي سعر</p>
            <img :src="require(`~/assets/icon/price.png`)" class="icon" alt="icon"/>
          </div>
        </div>
      </div>

      <div class="ml-2">
        <img :src="require(`~/assets/img/CompositeLayer.png`)" class="img" alt="icon"/>
      </div>
    </div>


    <div class="d-flex justify-content-end  w-100 mt-4 sp">
      <div class="">
        <p class="text-right font-weight-bold">سيارة سريعة بى ام دابليو تصنيع 2021 حالته جديدة سيارة سريعة بى ام دابليو تصنيع 2021 حالته جديدة</p>
        <div class="d-flex justify-content-between">
          <p class="text_PurpleSec font-weight-bold">$   500</p>
          <div class="d-flex">
          <p class="mr-2">أعلي سعر</p>
            <img :src="require(`~/assets/icon/price.png`)" class="icon" alt="icon"/>
          </div>
        </div>
      </div>

      <div class="ml-2">
        <img :src="require(`~/assets/img/CompositeLayer.png`)" class="img" alt="icon"/>
      </div>
    </div>


  </div>
</template>

<style scoped>
.img{
  width: 130px;
  height: 130px;
}
.icon{
  width: 20px;
  height: 20px;
}
@media screen and (max-width:1060px) and (min-width:990px){
  .sp{
    flex-wrap: wrap-reverse;
  }
}
@media screen and (max-width:875px) and (min-width:767px){
  .sp{
    flex-wrap: wrap-reverse;
  }
}
@media (max-width:400px) {
  .sp{
    flex-wrap: wrap-reverse;
  }
}
</style>
