<script>
    let {name, ...other} = $props();
</script>

<p>
	The <code>{other.name}</code> package is {other.description}. Download version {other.version} from
	<a href="https://www.npmjs.com/package/{other.name}">npm</a> and <a href={other.website}>learn more here</a>
</p>