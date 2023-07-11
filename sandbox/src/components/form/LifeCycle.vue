<template>
    <h1>
        O meu nome é: {{ nome }}
    </h1>
</template>

<script>
    export default {
        name: 'LifeCycle',
        data() {
            return {
                nome: 'José'
            }
        },
        methods: {
            batata() {
                console.log("Executou")
            }
        },
        created() {
                setTimeout(() => {
                    this.nome = 'Mauro'
                }, 2000);
                this.batata()
        },
        mounted() {
            setTimeout(() => {
                this.nome = 'Nando'
            }, 3000)
        }
    }
</script>