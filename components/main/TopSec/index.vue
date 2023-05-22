<template>
  <div class="bg-white rounded shadow p-3">

    <div class="bg_Gray rounded d-flex justify-content-between align-items-center text-white p-3 w-100">
      <p class="font-weight-bold my-0">2/3/2023</p>
      <p class="my-0">تاريخ البث</p>
    </div>

    <b-row  class="flex-wrap justify-content-between parent mt-2 w-100 mx-0">

      <div class="child bg-white rounded-pill shadow">
        <p class="text_Purple font-weight-bold m-0 pl-3">أحمد الرائد</p>
        <img :src="require(`~/assets/img/persontwo.png`)" class="" alt="icon"/>
      </div>

      <b-col cols="6" class="px-1">
        <div class="bg_LightPurple rounded text-center text_Purple py-2">
          <p class="">  القيمة الحالية بعد الضريبة</p>
          <p class="font-weight-bold my-0 f_22">$ 5050</p>
        </div>
      </b-col>
      <b-col cols="6" class="px-1 h-100">
        <div class="py-2 bg_Purple rounded text-center text-white h-100">
          <p>  القيمة الحالية للمزاد المعلن</p>
          <p class="font-weight-bold my-0 f_22">$ 5000</p>
        </div>
      </b-col>
    </b-row>

  </div>
</template>

<style scoped>
.parent{
  position: relative;
}
.child{
  position: absolute;
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 25px;
  width: 120px;
  padding: 5px;
  z-index: 2;
  bottom: -20px;
  right: 20px;
}
.child img{
  width: 20px;
  height: 20px;
}
.col {
    padding-bottom: 100%;
    margin-bottom: -100%;
}
</style>
