<template>
  <div class="app">
		<!-- Sidebar -->
    <Sidebar></Sidebar>

		<!-- Content
		<router-view /> -->
	</div>
  <p>test</p>
</template>

<script>
import Sidebar from "@/components/Sidebar.vue";

export default ({
  name: "MainView",
  components: {
    Sidebar
  },
  data() {
    return {


    }
  },
  methods: {
    showMessageModal() {
      
    }
  }
})
</script>

<style lang="scss">
:root {
	--primary: #4ade80;
	--primary-alt: #22c55e;
	--grey: #64748b;
	--dark: #1e293b;
	--dark-alt: #334155;
	--light: #f1f5f9;
	--sidebar-width: 300px;
}

* {
	margin: 0;
	padding: 0;
	box-sizing: border-box;
	font-family: 'Fira sans', sans-serif;
}

button {
	cursor: pointer;
	appearance: none;
	border: none;
	outline: none;
	background: none;
}

.app {
	display: flex;

	main {
		flex: 1 1 0;
		padding: 2rem;

		@media (max-width: 1024px) {
			padding-left: 6rem;
		}
	}
}
</style>