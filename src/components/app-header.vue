<template>
    <header class="main-header main-layout full">
        <section class="header-wrapper flex align-center justify-between">
            <div class="logo">
                <img src="../../src/assets/img/logo-web-1.png">
            </div>

            <nav>
                <ul class="link-list flex">
                    <li v-for="link in links" @click="toggleSelected">
                        {{ link }}
                        <span class="line"></span>
                    </li>
                </ul>
            </nav>
        </section>
    </header>
</template>

<script>
export default {
    data() {
        return {
            links: ['COPERATO','Home', 'VoIP', 'IT', 'Solutions', 'About', 'Contact']
        }
    },

    methods: {
        toggleSelected(ev) {
            [...document.querySelectorAll('.selected')].forEach(el => el.classList.remove('selected'))
            ev.target.classList.toggle('selected')
        }
    }
}
</script>

<style lang="scss" scoped>

</style>