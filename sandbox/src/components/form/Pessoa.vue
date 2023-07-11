<template>
    <div>
        <h2>Esta é a discrição da pessoa: {{ nome }}</h2>
        <Info :email="email" :esta_trabalhando=false />
    </div>
</template>
<script>
import Info from './Info.vue';

export default {
    name: 'Pessoa',
    data() {
        return {
            nome: 'João',
            email: 'João@gmail.com'
        }
    },
    components: {
        Info
    }
}
</script>