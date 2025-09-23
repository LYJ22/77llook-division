<script setup>
import { defineProps } from 'vue'
const props = defineProps([
  'imgURL',
  'KRname',
  'ENname',
  'JPname',
  'birth',
  'age',
  'height',
  'weight',
  'bloodtype',
  'bio',
])
</script>

<template>
  <div id="profile-card">
    <div class="profile-img">
      <img :src="imgURL" />
    </div>
    <div class="profile-text pretendard-jp font-black">
      <h3 style="font-size: 32px; font-weight: 900; line-height: 100%">{{ KRname }}</h3>
      <div>{{ ENname }}</div>
      <div>{{ JPname }}</div>
      <hr
        style="
          width: 216px;
          margin-top: 20px;
          margin-bottom: 8px;
          border: 0;
          border-top: 3px solid #000000;
        "
      />
      <div>{{ birth }}, {{ age }}</div>
      <div>{{ height }} / {{ weight }} / {{ bloodtype }}</div>
      <div style="margin-top: 16px">{{ bio }}</div>
    </div>
  </div>
</template>
