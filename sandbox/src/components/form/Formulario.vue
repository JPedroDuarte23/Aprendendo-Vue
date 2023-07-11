<template>
    <form action="" @submit="enviarFormulario">
        <div><input type="text" v-model="name"></div>
        <div><input type="text" v-model="email"></div>
        <Submit/>
    </form>
</template>

<script>
import Submit from './Submit.vue';
export default {
    name: 'Formulario',
    data() {
        return {
            name: '',
            email: ''
        }
    },
    methods: {
        enviarFormulario(event) {
            event.preventDefault();
            console.log("Formulario enviado");
            const name = this.name;
            const email = this.email;

            console.log("O email é " + email);
            console.log("O nome é " + name);
            
            // Envio de formulário AJAX para inserir o usuário

            // Inserir no banco os dados
        }
    },
    components: {
        Submit
    }
}
</script>