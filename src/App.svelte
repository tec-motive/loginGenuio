<script>
	import Header from './Header.svelte'
	import Form from './Form.svelte'
</script>

<main class="flex flex-col items-center mt-24 h-screen">
	<Header />
	<!-- (로고 이용시 주석을 풀어주세요)<p class="text-xs text-center">HANDMADE IN ITALY</p> -->
	<Form />
</main>



<style global>
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>