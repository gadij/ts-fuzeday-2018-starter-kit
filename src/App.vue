<template>
	<div id="app">
		<Navbar/>
		<router-view/>
	</div>
</template>
<script lang="ts">
    import {Component, Vue} from "vue-property-decorator";
    import Navbar from "./components/Navbar.vue";

    @Component({
        components: {
            Navbar,
        },
    })
    export default class App extends Vue {
    }
</script>
<style lang="scss" scoped>
	#app {
		font-family: Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		color: #2c3e50;
	}
</style>
