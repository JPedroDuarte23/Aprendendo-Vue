<template>
    <div>
        <button  @click="primeiro('Primeiro Evento',$event), segundo(txt2,$event), terceiro($event)">Ativar multiplos eventos</button>
        <!-- É possível utilizar texto puro e valores declarados no data() como um parametro -->
        <p> {{ multiplos_eventos }}</p>
    </div>
</template>

<script>
export default {
    name: 'MultiplosEventos',
    data() { 
        return {
            multiplos_eventos: '',
            txt2: 'Segundo Evento'
        }
    }, 
    methods: {
        primeiro(txt,event) {
            this.multiplos_eventos = txt
        },
        segundo(txt,event) {
            setTimeout(() => {
                this.multiplos_eventos = txt
            }, 1000)
        }, 
        terceiro(event) {
            setTimeout(() => {
                this.multiplos_eventos = ""
            }, 2000)
        }
    }
    
}
</script>
<style scoped>
div {
    margin: 100px
}
</style>