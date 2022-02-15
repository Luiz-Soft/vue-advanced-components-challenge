<template>
    <div class='color'>
    <slot />
    </div>
</template>

<script>


export default{
    name: 'SelectedColor'
   
}
</script>

<style scoped>
.color{
    background-color: blue;
}
</style>