<template>
    <div>
        <slot></slot>
        <!-- Buradaki slot ile diğer tarafta header içerisine ne yazarsam yazayım gelip veri buraya girecektir. -->
    </div>
  
</template>

<script>
export default {
data(){
    return{
        props:['content']
    }
}
}
</script>

<style>

</style>