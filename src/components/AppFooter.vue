<script>
export default {
    name: 'AppFooter',
}
</script>

<template>
    <footer>
        <div class="container">
            <div class="logo">
                <!-- <img src="/img/la-molisana-logo.png"> -->
                <img src="../assets/img/la-molisana-logo.png">
            </div>

            <div class="menu-col">
                <h3>Titolo menu</h3>

                <nav>
                    <ul>
                        <li>
                            Link 1
                        </li>
                        <li>
                            Link 2
                        </li>
                        <li>
                            Link 3
                        </li>
                        <li>
                            Link 4
                        </li>

                    </ul>
                </nav>
            </div>

            <div class="menu-col">
                <h3>Titolo menu</h3>

                <nav>
                    <ul>
                        <li>
                            Link 1
                        </li>
                        <li>
                            Link 2
                        </li>
                        <li>
                            Link 3
                        </li>
                        <li>
                            Link 4
                        </li>

                    </ul>
                </nav>
            </div>
        </div>

        <div class="bottom-img">
            <img src="../assets/img/footer-montagne-bottom.jpg">
        </div>
    </footer>
</template>

<style lang="scss" scoped>
@use '../style/partials/variables' as *;

.container {
    display: flex;

    .logo {
        width: 40%;
    }

    .menu-col {
       width: 30%;

       h3 {
            color: $brand-primary;
            margin-bottom: 10px;
       }

       li {
        padding: 3px 0;
        font-size: 20px;
       }
    }

}

.bottom-img {
    margin-top: 50px;
}
</style>