<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            links: [
                {
                    text: 'Home',
                    active: false
                },
                {
                    text: 'Prodotti',
                    active: true
                },
                {
                    text: 'Chi siamo',
                    active: false
                },
                {
                    text: 'Contatti',
                    active: false
                },
            ],
        }
    }
}
</script>

<template>
    <header>
        <div class="logo">
            <img src="../assets/img/la-molisana-logo.png">
        </div>
        
        <nav>
            <ul>
                <li :class="{'active': link.active}" v-for="link in links">
                    <a href="#">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<style scoped lang="scss">
@use '../style/partials/variables' as *;

.logo {
    text-align: center;
    padding: 15px 0;
}

nav {
    display: flex;
    justify-content: center;

    ul {
        display: flex;

        li {
            padding: 10px;

            &.active {
                background-color: $brand-secondary;
            }

            a {
                font-size: 25px;
                color: black;
            }
        }
    }

}
</style>