<template>
    <div class="md:container md:m-auto mt-4 grid grid-row-2">
       <div>
         <span class="float-left text-white text-bold">Ramazana Özel Ürünler</span>
        </div> 
             <div class="md:container md:m-auto sm:my-auto mt-3 xs:mt-4">
                 <div class="justify-center grid lg:grid-cols-2 xs:grid-cols-1 gap-2 m-auto">
                     <div class="rounded-lg bg-white mt-1"  v-for="item in ramazanPaketleri" :key="item.id">
                         <div class="rounded-lg sm:p-1 md:p-3 md:m-4 object-center bg-white grid grid-cols-2">
                             <div class="flex items-center">
                                 <img class="rounded m-auto" :src="item.src" alt="/alt"/>
                             </div>
                            <div class="flex flex-col">
                                <span class="my-12" style="">{{item.name}}</span>
                                <h1 class="my-12" style="color: #45AC4C; font-weight: 700;">{{item.price}} TL</h1>
                                <button type="button" class="button px-4 py-2.5 my-12 shadow-md transition text-white rounded-lg font-semibold" style="background-color: rgb(245 158 11);">Sepete Ekle</button>
                            </div>
                         </div>
                     </div>
                 </div>
             </div>
             <div class="w-full flex justify-between md:mx-auto mb-4">
                <div class="mt-3">
                  <button type="button" class="text-black bg-white font-medium rounded-lg px-8 py-2 text-sm text-center">
                    8 Ürün Göster
                    </button>
                </div>
                <div class="flex flex-row space-between mt-3">
                    <button type="button" class="text-black bg-white font-medium rounded-lg px-2 text-sm text-center">
                        ❮ Önceki Sayfa 
                    </button>
                    <div class="flex flex-row mx-4">
                        <button type="button" class="text-black bg-white px-4 py-2 font-medium rounded-lg text-sm text-center mr-2">
                        1 
                        </button>
                        <button type="button" class="text-black-700 border px-4 py-2 hover:text-black hover:bg-white font-medium rounded-lg text-sm  text-center mr-2">
                        2
                        </button>
                        <button type="button" class="text-black-700 border px-4 py-2 hover:text-black hover:bg-white font-medium rounded-lg text-sm mr-2">
                        3
                        </button>
                    </div>
                    <button type="button" class="text-black bg-white font-medium rounded-lg text-sm text-center px-2">
                    Sonraki Sayfa ❯
                    </button> 
                </div> 
            </div>
   </div>
</template>
<script>
export default {
    name: 'appRamazanOzel',
        data() {
        return {
        ramazanPaketleri: [
            {id:1,name:"Fındıklı Hindistan Cevizli Afyon Lokumu",price:"29,00" , src: require('../assets/image 302.svg')},
            {id:2,name:"Tarcın & Anberçicekli Bitkisel Su Karışımı Şerbet 250ml",price:"40" , src: require('../assets/image 303.svg')},
            {id:3,name:"Gazioğlu Üçler Güllaç 500gr",price:"29,00" , src: require('../assets/image 308.svg')},
            {id:4,name:"Medine Hurması Paketi 600gr",price:"70" , src: require('../assets/image 309.svg')},
            {id:5,name:"Nuh'un Ankara Makarnası Paket",price:"2,90" , src: require('../assets/image 311.svg')},
            {id:6,name:"Knorr Klasik Hazır Mercimek Çorbası",price:"3,90" , src: require('../assets/image 314.svg')},
            {id:7,name:"Gaziantep Fıstıklı Baklava 1kg",price:"90" , src: require('../assets/image 316.svg')},
            {id:8,name:"Söke Un,Dr.Oetker Ekşi Maya,Bağdat Susam",price:"29,00" , src: require('../assets/Group 7719.svg')},
            
        ],
        }
   
    }
}
</script>