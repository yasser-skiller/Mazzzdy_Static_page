<template>
    <b-col cols="11"   md="10" lg="10" class="bg-white rounded shadow p-4 mt-5 mx-auto">

    <p class="font-weight-bolder text-right f_22">تفاصيل المزاد</p>

    <div class="d-flex flex-wrap-reverse justify-content-between sp  w-100 my-3 pb-3 border-bottom">
      <div class="d-flex flex-column align-items-end">
        <div class="d-flex f_18 text_GrayTHr">
          <p class="mr-3">قطعة </p>
          <p>200 </p>
        </div>
        <div class="d-flex">
          <p class="text_Yellow font-weight-bolder">صوت</p>
          <img :src="require(`~/assets/icon/sound.png`)" class="icon" alt="icon"/>
        </div>
      </div>
      <div class="d-flex flex-column align-items-end">
        <div class="d-flex">
          <p>Egypt , Mansoura</p>
          <img :src="require(`~/assets/icon/location.png`)" class="icon" alt="icon"/>
        </div>
        <div class="d-flex">
          <p class="text_GrayTHr">البيع لاعلى سعر</p>
          <img :src="require(`~/assets/icon/dor.png`)" class="icontwo" alt="icon"/>
        </div>
        <div class="d-flex">
          <p>منتجات متعددة</p>
          <img :src="require(`~/assets/icon/Group.png`)" class="icontwo" alt="icon"/>
        </div>
      </div>
    </div>

    <div class="text-right pb-3 border-bottom">
      <p class="font-weight-bolder text-right f_22"> وصف</p>
      <p class="text_GrayTHr">
        هذا النص هو مثال لنص يمكن أن يستبدل في نفس المساحة، لقد تم توليد هذا النص من مولد النص العربى، حيث يمكنك أن تولد مثل هذا النص أو العديد من النصوص الأخرى إضافة إلى زيادة عدد الحروف التى يولدها التطبيق. إذا كنت تحتاج إلى عدد أكبر من الفقرات يتيح لك مولد النص العربى زيادة عدد الفقرات كما تريد، النص لن يبدو مقسما ولا يحوي أخطاء لغوية، مولد النص العربى مفيد لمصممي المواقع على وجه الخصوص، حيث يحتاج العميل فى كثير من الأحيان أن يطلع على صورة حقيقية لتصميم الموقع. ومن هنا وجب على المصمم أن يضع نصوصا مؤقتة على التصميم ليظهر للعميل الشكل كاملاً،دور مولد النص العربى أن يوفر على المصمم عناء البحث عن نص بديل لا علاقة له بالموضوع الذى يتحدث عنه التصميم فيظهر بشكل لا يليق.

      </p>
    </div>

    <div class="text-right ">
      <p class="font-weight-bolder text-right f_22 pt-3"> سياسة الاسترجاع والاستبدال</p>
      <p class="text_GrayTHr">
        هذا النص هو مثال لنص يمكن أن يستبدل في نفس المساحة، لقد تم توليد هذا النص من مولد النص العربى، حيث يمكنك أن تولد مثل هذا النص أو العديد من النصوص الأخرى إضافة إلى زيادة عدد الحروف التى يولدها التطبيق. إذا كنت تحتاج إلى عدد أكبر من الفقرات يتيح لك مولد النص العربى زيادة عدد الفقرات كما تريد، النص لن يبدو مقسما ولا يحوي أخطاء لغوية، مولد النص العربى مفيد لمصممي المواقع على وجه الخصوص، حيث يحتاج العميل فى كثير من الأحيان أن يطلع على صورة حقيقية لتصميم الموقع. ومن هنا وجب على المصمم أن يضع نصوصا مؤقتة على التصميم ليظهر للعميل الشكل كاملاً،دور مولد النص العربى أن يوفر على المصمم عناء البحث عن نص بديل لا علاقة له بالموضوع الذى يتحدث عنه التصميم فيظهر بشكل لا يليق.

      </p>
    </div>


  </b-col>
</template>

<style scop>
.icon{
  width:15px;
  height:20px;
  margin-left: 5px;
}
.icontwo{
  width:20px;
  height:20px;
  margin-left: 5px;
}
@media (max-width:360px) {
  .sp{
    justify-content: end !important;
  }

}
</style>
