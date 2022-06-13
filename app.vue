<template>
    <Header />
    <index />
</template>

<script>
import index from './pages';
import Header from './components/home/header/Header';

export default {
    name: 'app',

    components: {Header, index }
};
</script>
