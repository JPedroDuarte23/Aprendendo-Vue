<template>
    <img :src="avatar" :alt="descricao">
    <!-- Podemos usar o v-bind: mas o Vue ja tem algumas sintaxes para auxiliar em 
    certas coisas-->
    <MudarImagem @mudar-imagem="trocarImagem"/>
</template>
<script>
import MudarImagem from './MudarImagem.vue';

    export default  {
        name: 'Picture',
        components: {
            MudarImagem
        },
        data() {
            return{
                avatar: '/img/download.png',
                // o / ja acessa a pasta public como padrão
                descricao: 'Pikachu'
            }
        },
        methods: {
            trocarImagem() {
                this.avatar = '/img/222.jpg'
            }
        }
    }
</script>