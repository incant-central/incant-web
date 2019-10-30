<script>
    let m = {
        x: 0,
        y: 0
    };
    function handleMouse({ x, y }) {
        m.x = x;
        m.y = y;
    }
</script>

<svelte:head>
    <title>About</title>
</svelte:head>

<h1>About this site</h1>

<h1 on:mousemove={handleMouse}>x: {m.x} y: {m.y}</h1>

<p>This is the 'about' page. There's not much here.</p>
