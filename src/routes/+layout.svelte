<nav>
    <div class="nav-container">
        <a href="/" class = "nav-logo" title = "Back to homepage">Имя Фамилия</a>
        <div class="nav-links">
            {#each nav as link}
                <a href = {link.href} class = "link">{link.title}</a>
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
            href: '/about'
        },
        {
            title: 'Блог',
            href: '/blog'
        },
        {
            title: 'Портфолио',
            href: '/projects'
        },
        {
            title: 'Котнтакты',
            href: '/contact'
        },
        {
            title: 'temp',
            href: '/temp'
        }
    ]
</script>
<style>
    .container {
        min-width: 1400px;
        margin: 50 auto;
    }
</style>