<template>
    <div class="md:container md:mx-auto">
        <div class="justify-center grid grid-cols-3 gap-2">
           <div class="rounded-lg bg-white"  v-for="item in ramazanPaketleri" :key="item.id">
                  <div class="rounded-lg sm:p-1 md:p-3 md:m-4 object-center bg-white">
                     <a>
                     <img class="m-auto" :src="item.src" alt=""/>
                    </a>
                <button type="button" class="button px-4 py-2.5 sm:m-auto sm:text-xs">Paketi İncele</button>
                  </div>
             </div>
          </div>
    </div>
</template>
<script>
export default {
    name: 'appCard',
    data() {
        return {
        ramazanPaketleri: [
            {id:1,name:"kucukpaket", src: require('../assets/KüçükPaket.svg')},
            {id:2,name:"normalpaket", src: require('../assets/NormalPaket.svg')},
            {id:3,name:"buyukpaket", src: require('../assets/BüyükPaket.svg')},
        ],
        }
    }
}
</script>
<style scoped>
.button {
    color: rgb(255 255 255);
    font-weight: 700;
    font-size: 0.75rem;
    line-height: 1rem; 
    line-height: 1;
    border-radius: 0.25rem;
    background-color:#074387;
    margin-top: 0.5em;
}
</style>           