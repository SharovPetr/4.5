<nav>
    <div class="nav-container">
        <a href="/" class="nav-logo" title="Back to Homepage">Главная</a>
        <div class="nav-links">
            {#each nav as link}
            <a href={link.href} class="link">{link.title}</a>
            {/each}
        </div>
    </div>
</nav>

<div class="container">
    <!-- Pages will be injected below -->
    <slot></slot>
</div>

<script>
    const nav = [
        {
         title: "Фильмы",
         href: "/films",
         isShow: true,
        },
        {
         title: "Контакты",
         href: "/contacts",
         isShow: true,
        }
    ];
</script>
<style>
    .container {
    max-width: 1400px;
    margin: 50px auto;
    }
</style>