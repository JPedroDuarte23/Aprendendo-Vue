<template>
    <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">Projetos</a></li>
        <li><a href="#">Contatos</a></li>
        <li><a href="#" v-if="esta_logado">Meu Perfil</a></li>
    </ul>
</template>

<script>
export default {
    name: 'Header',
    props: {
        esta_logado: Boolean
    },
    data() {
        return {

        }
    }
}
</script>

<style scoped>
ul {
    list-style-type: none;
    display: flex;
    background-color: black;
}
li {
    margin-right: 10px;
}
a {
    text-decoration: none;
    color: #ddd;
}
a:hover {
    color: magenta;
}

</style>