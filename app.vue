<template>
    <div>
        <Header />
        <index />
    </div>
</template>

<script>
import index from './pages';
import Header from './components/header/Header';

export default {
    name: 'app',

    components: { Header, index }
};
</script>
