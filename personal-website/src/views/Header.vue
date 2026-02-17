<template>
    <nav class="navbar" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
            <a class="navbar-item" href="/">
                <strong>
                    <router-link to="/" class="navbar-item">
                        <font-awesome-icon icon="fa-solid fa-house" />home
                    </router-link>
                </strong>
            </a>
        </div>
        <div class="navbar-menu">
            <div class="navbar-end">
                <router-link to="/" class="navbar-item">
                    about @me
                </router-link>
                <router-link to="/" class="navbar-item">
                    projects
                </router-link>
            </div>
        </div>
    </nav>
</template>

<style scoped>
    .navbar {
        background-color: transparent;
        background-image: none;
        padding: 1rem 15rem;
    }
</style>