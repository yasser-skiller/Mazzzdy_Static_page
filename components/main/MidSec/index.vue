<template>
  <div class="bg-white rounded shadow p-3 mt-5">

    <div class="bg_GraySce border rounded d-flex justify-content-between align-items-center text-white p-3 w-100 my-3">
      <p class="font-weight-bolder my-0 f_22 text_GrayTHr">5000</p>
      <p class="my-0 text_GrayFour text-right"> القيمة الأبتدائية</p>
    </div>

    <div class="bg_GraySce border rounded d-flex justify-content-between align-items-center text-white p-3 w-100 my-3">
      <p class="font-weight-bolder my-0 f_22 text_GrayTHr">5000</p>
      <p class="my-0 text_GrayFour text-right"> القيمة التقريبية</p>
    </div>

    <div class="bg_GraySce border rounded d-flex justify-content-between align-items-center text-white p-3 w-100 my-3">
      <p class="font-weight-bolder my-0 f_22 text_GrayTHr">5000</p>
      <p class="my-0 text_GrayFour text-right">  العربون</p>
    </div>

    <div class="bg_GraySce border rounded d-flex justify-content-between align-items-center text-white p-3 w-100 my-3">
      <p class="font-weight-bolder my-0 f_22 text_GrayTHr">5000</p>
      <p class="my-0 text_GrayFour text-right">  سعر الشراء الفورى</p>
    </div>

    <div class="bg_GraySce border rounded d-flex justify-content-between align-items-center text-white p-3 w-100 my-3">
      <p class="font-weight-bolder my-0 f_22 text_GrayTHr">5000</p>
      <p class="my-0 text_GrayFour text-right">  قيمة ذيادة المزاد</p>
    </div>

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
  height: 30px;
  width: 100px;
  padding: 5px;
  z-index: 2;
  bottom: -20px;
  right: 20px;
}
.child img{
  widows: 25px;
  height: 25px;
}
</style>
