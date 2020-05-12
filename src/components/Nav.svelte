<script>
	import Navbar from 'sveltestrap/src/Navbar.svelte';
	import Container from 'sveltestrap/src/Container.svelte';
	import NavbarToggler from 'sveltestrap/src/NavbarToggler.svelte';
	import NavbarBrand from 'sveltestrap/src/NavbarBrand.svelte';
	import Nav from 'sveltestrap/src/Nav.svelte';
	import NavItem from 'sveltestrap/src/NavItem.svelte';
	import NavLink from 'sveltestrap/src/NavLink.svelte';
	import Collapse from 'sveltestrap/src/Collapse.svelte';
	import UncontrolledDropdown from 'sveltestrap/src/UncontrolledDropdown.svelte';
	import DropdownItem from 'sveltestrap/src/DropdownItem.svelte';
	import DropdownMenu from 'sveltestrap/src/DropdownMenu.svelte';
	import DropdownToggle from 'sveltestrap/src/DropdownToggle.svelte';

	export let segment;
	let scrollY;

	let isOpen = false;

	function handleUpdate(event) {
		isOpen = event.detail.isOpen;
		scrollY = 0;
	}
</script>

<svelte:window bind:scrollY />

<Navbar expand="md" color="white" dark class="shadow fixed-top portfolio-navbar gradient">
	<Container>
		<NavbarBrand href="/">
			Filip Holčík
		</NavbarBrand>
		<NavbarToggler on:click={() => (isOpen = !isOpen)} />
		<Collapse {isOpen} navbar expand="md" on:update={handleUpdate}>
			<Nav class="ml-auto" navbar>
				<NavItem>
					<NavLink href="." active={segment === undefined} rel=prefetch>
						Home
					</NavLink>
				</NavItem>
				<NavItem>
					<NavLink href="story" active={segment === 'story'} rel=prefetch>
						Story
					</NavLink>
				</NavItem>
				<NavItem>
					<NavLink href="projects" active={segment === 'projects'} rel=prefetch>
						Projects
					</NavLink>
				</NavItem>
				<NavItem>
					<NavLink href="contact" active={segment === 'contact'} rel=prefetch>
						Contact
					</NavLink>
				</NavItem>
			</Nav>
		</Collapse>
	</Container>
</Navbar>

<style>
</style>
