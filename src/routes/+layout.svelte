<svelte:head>
	<link rel="preconnect" href="https://fonts.googleapis.com">
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin >
	<link href="https://fonts.googleapis.com/css2?family=Bricolage+Grotesque:opsz,wght@10..48,400;10..48,700&family=Dosis:wght@400;500;700&family=Inter:wght@400;700&family=Space+Grotesk:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <title>Roti by Matt</title>
    <meta name="viewport" content="width=device-width, initial-scale=1">
</svelte:head>

<slot />

<style>
    :global(*, *::before, *::after) {
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        font-size: 14px;
        font-family: "Dosis", sans-serif;
    }
    :global(html, body) {
        width: 100%;
        height: 100%;
        background-color: #2F241D;
        color: #FEFEFE;
    }
    :global(a) {
        text-decoration: none;
    }
</style>