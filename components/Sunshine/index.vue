<template>
  <view class="sunshine">
      <image
          :style="{width: 50, height: 50}"
          :source="{ uri: 'https://vignette.wikia.nocookie.net/robloxcreepypasta/images/2/26/Smile.png/revision/latest?cb=20180519182354'}"
      />
  </view>
</template>

<style>
 .sunshine {
   width: 120;
   height: 120;
   background-color: #fff00f;
   borderRadius: 60;
   shadowColor: rgb(112, 84, 46);
   shadowOpacity: 0.8;
   shadowRadius: 10;
   elevation: 1;
   position: absolute;
   top: 150;
   display: flex;
   justify-content: center;
   align-items: center;
 }

</style>

