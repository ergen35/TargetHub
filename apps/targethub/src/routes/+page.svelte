<script>
	import { Button, Table, Loading } from 'attractions';

	let headers = [
		{ text: 'First Name', value: 'firstName' },
		{ text: 'Last Name', value: 'lastName' },
		{ text: 'Age', value: 'age', align: 'end' }
	];
	let items = [
		{ firstName: 'John', lastName: 'Doe', age: 694 },
		{ firstName: 'Leo', lastName: 'Tolstoy', age: new Date().getFullYear() - 1828 },
		{ firstName: 'فلان', lastName: 'الفلاني', age: 42 },
		{ firstName: 'Иван', lastName: 'Иванов', age: 69 }
	];
</script>

<Button filled>Click Me</Button>

<h1>Welcome to SvelteKit</h1>
<p>Visit <a href="https://kit.svelte.dev">kit.svelte.dev</a> to read the documentation</p>

<Loading />

<Table {headers} {items} />

<style>
	/* your styles go here */
</style>
