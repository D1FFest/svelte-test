<nav>
    <div class="nav-container">
        <a href="/" class = "nav-logo" title = "Back to homepage">Имя Фамилия</a>
        <div class="nav-links">
            {#each nav as link}
            {#if link.isShow}
                <a href = {link.href} class = "link">{link.title}</a>
            {/if}
            {/each}
        </div>  
    </div>
</nav>
<div class="conyainer">
    <slot></slot>
</div>
<script>
    const nav = [
        {
            title: 'Обо мне',
            href: '/about',
            isShow: true
        },
        {
            title: 'Блог',
            href: '/blog',
            isShow: true
        },
        {
            title: 'Портфолио',
            href: '/projects',
            isShow: true
        },
        {
            title: 'Котнтакты',
            href: '/contact',
            isShow: true
        },
        {
            title: 'temp',
            href: '/temp',
            isShow: false
        }
    ]
</script>
<style>
    .container {
        min-width: 1400px;
        margin: 50 auto;
    }
</style>