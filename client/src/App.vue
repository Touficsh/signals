<script setup>
const items = [
  {
    pair: "XAUUSD",
    entry: '2000',
    sl: '1980',
    tp: '2020'
  }
]

</script>

<template>
  <div class="">
     <div class="font-bold text-2xl text-center bg-[#010101] text-[#C8902B] pt-2 pb-3 shadow-md">
         Signals
     </div>
     <div>
        <div v-for="(item, index) in items" :key="index">
            <div class="m-4 p-2 w-[200px] h-[120px] border-2 bg-[#C8902B] text-center flex rounded-md shadow-md">
              <div class="flex flex-col text-left">
                <span class="font-bold mr-2">Pair Symbol:</span>
                <span class="font-bold mr-2">Entry Price :</span>
                <span class="font-bold mr-2">Stop Loss:</span>
                <span class="font-bold mr-2">Take Profit:</span>
              </div>
              <div class="flex flex-col text-left">
                <span>{{item.pair}}</span>
                <span>{{item.entry}}</span>
                <span>{{item.sl}}</span>
                <span>{{item.tp}}</span>
              </div>
            </div>
        </div>
     </div>
  </div>
</template>

<style scoped>

</style>
