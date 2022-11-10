<script setup>
defineProps({

})
</script>

<template>
    <header>
        <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />


        <div class="wrapper greetings">
            <a href="/">
                <h1 class="green">Аналитика</h1>
            </a>
            <h3>
                Загрузите ваш портфель и просматривайте подробный анализ активов
            </h3>

            <nav>
                <RouterLink to="/SignIn">Войти</RouterLink>
                <RouterLink to="/SignUp">Зарегистрироваться</RouterLink>
            </nav>
        </div>
    </header>

</template>


<style scoped>
h1 {
    font-weight: 500;
    font-size: 2.6rem;
    top: -10px;
}

h3 {
    font-size: 1.2rem;
}

.greetings h1,
.greetings h3 {
    text-align: center;
}

@media (min-width: 1024px) {

    .greetings h1,
    .greetings h3 {
        text-align: left;
    }
}

header {
    line-height: 1.5;
    max-height: 100vh;
}

a:hover {
    text-decoration: none;
}

.logo {
    display: block;
    margin: 0 auto 2rem;
}

nav {
    width: 100%;
    font-size: 12px;
    text-align: center;
    margin-top: 2rem;
}

nav a.router-link-exact-active {
    color: var(--color-text);

}

nav a.router-link-exact-active:hover {
    background-color: transparent;

}

nav a {
    display: inline-block;
    padding: 0 1rem;
    border-left: 1px solid var(--color-border);
}

nav a:first-of-type {
    border: 0;
}

@media (min-width: 1024px) {
    header {
        display: flex;
        place-items: center;
        padding-right: calc(var(--section-gap) / 2);
    }

    .logo {
        margin: 0 2rem 0 0;
    }

    header .wrapper {
        display: flex;
        place-items: flex-start;
        flex-wrap: wrap;
    }

    nav {
        text-align: left;
        margin-left: -1rem;
        font-size: 1rem;

        padding: 1rem 0;
        margin-top: 1rem;
    }
}
</style>