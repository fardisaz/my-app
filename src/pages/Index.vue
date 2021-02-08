<template>
  <q-page class="flex flex-center ">
        <div v-for="arr in newArr" :key="arr.bgColor" class="q-pa-sm flex">
      <q-checkbox
        v-model="arr.checked"
        keep-color
        :label="arr.bgColor"
        :style="{ color: '#' + arr.bgColor }"
      ></q-checkbox>
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
 
  
  data(){
return{
 
   newArr: [
        {
          bgColor: "501253",
          checked: false
        },
        {
          bgColor: "acedef",
          checked: false
        },
        {
          bgColor: "deadbeef",
          checked: false
        }
      ]
  
}
  }
}
</script>
<style scoped >


.q-checkbox__inner {
  color: unset;
}
.q-checkbox__label {
  color: black;
}
.q-checkbox__inner .q-checkbox__bg {
    background: currentColor;
}
</style>
