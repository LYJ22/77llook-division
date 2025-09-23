<script setup>
import ProfileCard from './ProfileCard.vue'
import profileImg1 from '../assets/images/profile/profileImg1.png'
import profileImg2 from '../assets/images/profile/profileImg2.png'
</script>

<template>
  <div id="profile-component">
    <div id="profile-wrapper">
      <h1 class="profile-title alfa-slab-one-regular">profile</h1>
      <hr style="margin: 16px 36px 0 0; border: 0; border-top: 3px solid #000000" />

      <!-- 본문 내용 -->
      <ProfileCard
        :imgURL="profileImg1"
        KRname="이루마 쥬토"
        ENname="Iruma Jyuto"
        JPname="入間銃兎"
        birth="0530"
        age="29"
        height="181"
        weight="65"
        bloodtype="A"
        bio="He who is no courageous enough to take risks will accomplish nothing in life."
      />
      <ProfileCard
        :imgURL="profileImg2"
        KRname="후지사키 료코"
        ENname="Fujisaki Ryoko"
        JPname="藤咲凉狐"
        birth="0131"
        age="27"
        height="161"
        weight="45"
        bloodtype="AB"
        bio="Age is no guarantee of maturity."
      />
      <div class="introduction">
        <p class="font-black">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus lectus erat, fermentum
          vitae pharetra a, sollicitudin sed enim. Nullam viverra iaculis neque eu feugiat.
          Suspendisse faucibus lacinia augue at tempor. Pellentesque magna mauris, cursus vitae
          tortor sed, euismod consectetur purus. Suspendisse non scelerisque libero. Morbi
          ullamcorper turpis lacus, eu pretium magna pretium tempor. Ut sed aliquet ligula. Morbi id
          gravida eros. Sed condimentum tortor nec congue viverra. Phasellus non dolor non ex
          laoreet aliquet vel nec erat. Nunc sed porta nisi. Vivamus eu justo id tellus egestas
          rhoncus. Aliquam at dolor libero. Nunc consequat tortor vel consectetur elementum.
          Suspendisse nisi leo, placerat vel lacus in, consequat tempor libero. Vestibulum id
          dignissim justo, nec sodales nisl. Nullam mattis justo a diam finibus sollicitudin.
          Vestibulum non interdum metus, vitae ultricies sem. Mauris eget augue vel tellus laoreet
          viverra. Cras tempus turpis elit, nec tincidunt lacus pellentesque ut. Vestibulum iaculis,
          ipsum a tempus euismod, sapien tellus pharetra neque, eget convallis enim arcu at leo. In
          lobortis eros purus, et rutrum ipsum sagittis id.
        </p>
      </div>
    </div>
  </div>
</template>
