<template>
    <div>
        <slot></slot>
        <!-- Buradaki slot ile diğer tarafta header içerisine ne yazarsam yazayım gelip veri buraya girecektir. -->
<p>{{ nameSurname }}</p>
    </div>
  
</template>

<script>
export default {
data(){
    return{
        name:'',
        surname:''
    }
},

//computed: daha çok matematiksel işlemlerde kullanılır. Bir grafiğin girilen verilere göre şekil almasını sağlarız. Methods ilede aşağıdaki işlemi yapabilirdik fakat aralarındaki fark computed bilgiyi cacheleyecek ve cacheden değeri alıp bize dönecektir.
computed:{
    nameSurname(){
        return this.name + ' ' + this.surname
    }
}

//Computed : verinin sonucunu cacheleyip , cache üzerinden işlemleri yapmasıdır.
}
</script>

<style>

</style>