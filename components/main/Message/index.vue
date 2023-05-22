<template>
  <b-col cols="11"   md="10" lg="10" class="bg-white rounded shadow p-4 mt-5 mx-auto">

    <p class="font-weight-bolder text-right f_22"> ارسال رسالة الى البائع</p>
    <p class="text-right">يمكنك في وقت البث المباشر ارسال رسالة الى البائع للاستفسار</p>


    <form class="d-flex justify-content-between align-items-center w-100 my-3">
      <button class="btn rounded-circle bg_Pink mr-2" type="submit">
        <img :src="require(`~/assets/icon/send.png`)" class="icon" alt="icon"/>
      </button>
      <input type="text" class="form-control text-right bg_GraySce rounded-pill" id="floatingInput" placeholder="اكتب سؤالك">
    </form>

  </b-col>
</template>

<style scoped>
.icon{
  width: 20px;
  height: 25px;
  margin: auto;
}
</style>
