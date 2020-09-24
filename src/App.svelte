<!--script-->
<script>
	import Navbar from "./Components/Navbar/Navbar.svelte";
	import { NAV_BAR_DATA, HEADER } from "./Data/data";
</script>

<!-- Navbar -->
<Navbar navlists={NAV_BAR_DATA} header={HEADER} />