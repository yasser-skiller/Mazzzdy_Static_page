<template>
  <div class="m-4 mx-sm-3">
    <b-row align-h="center"  class="flex-wrap-reverse">
      <b-col cols="12"   md="5" lg="4" class="mx-auto mt-3">
        <TopSec/>
        <Contenders/>
        <MidSec/>
        <FavoriteAuctions/>
      </b-col>
      <b-col cols="12"  md="7" lg="8" class="mx-auto mt-3">
        <Header/>
        <Message/>
        <Details/>
      </b-col>
    </b-row>
  </div>
 </template>

 <script>
 import TopSec from '@/components/main/TopSec';
 import Contenders from '@/components/main/Contenders';
 import MidSec from '@/components/main/MidSec';
 import FavoriteAuctions from '@/components/main/FavoriteAuctions';
 import Header from '@/components/main/Header';
 import Message from '@/components/main/Message';
 import Details from '@/components/main/Details';

 export default {
   components:{
    TopSec,
    Contenders,
    MidSec,
    FavoriteAuctions,
    Header,
    Message,
    Details,

   },

 }
 </script>
