<nav>
    <div class="nav-container">
        <a href="/" class = "nav-logo" title = "Back to homepage">Имя Фамилия</a>
        <div class="nav-links">
            <a href="/about" class = "link">Обо мне</a>
            <a href="/blog" class = "link">Блог</a>
            <a href="/projects" class = "link">Портфолио</a>
            <a href="/contact" class = "link">Контакты</a>
        </div>  
    </div>
</nav>
<div class="conyainer">
    <slot></slot>
</div>
<style>
    .container {
        min-width: 1400px;
        margin: 50 auto;
    }
</style>