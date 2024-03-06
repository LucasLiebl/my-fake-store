<script setup>
import { useScreen } from '@/composables/screen';

import { Account } from 'vue-material-design-icons/Account.vue';

const { isMobile } = useScreen();
</script>

<template>
    <div class="navbarmobile" v-if="isMobile">
<button class="botoes">aaaa</button>
<button class="botoes">aaaaa</button>
<button class="botoes">aaaa</button>
<button class="botoes"><Account/></button>
    </div>
<div class="navbar" v-else>
    <h1>My FakeStore</h1>
</div>
</template>
<style scoped>
.navbar{
    background-color: #e74d3c;
    color: white;
}
.navbarmobile{
    background-color: #e74d3c;
    position: sticky;
    bottom: 0px;
}
button{
    width: 25% ;
    border: 0;
    height: 50px;
    background-color: #e74d3c;
    color: white;
    text-decoration: none;
    font-size: larger;
}
</style>