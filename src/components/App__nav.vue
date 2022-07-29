<template>
    <ul class="menu">
        <nav class="menu-indicator">
            <li class="menu-item" v-for="link in links" :key="link.id" ref="li" @click="sliderIndicator(link.id)">
                <a :href="link.href" class="menu-link">
                    <i class="menu-icon" :class="link.icon"></i>
                    <span>{{link.text}}</span>  
                </a>
            </li>


        </nav>
    </ul>


</template>
<script>

export default {
    name: 'App__nav',
    data() {
        return {
            sliderPosition: 0,
            selectedEelementWidth: 0,
            selectedIndex: 0,
            links: [
                {
                    id: 1,
                    icon: "fa-solid fa-house",
                    text: "Accueil",
                    href: "#"
                },
                {
                    id: 2,
                    icon: "fa-solid fa-circle-check",
                    text: "Présentation",
                    href: "#about"
                },
                {
                    id: 3,
                    icon: "fa-solid fa-child-reaching",
                    text: "Pilates",
                    href: "#pilates"
                },
                {
                    id: 4,
                    icon: "fa-solid fa-calendar-day",
                    text: "Horaires & Tarifs",
                    href: "#ht"
                },
                {
                    id: 5,
                    icon: "fa-solid fa-address-card",
                    text: "Contact",
                    href: "#contact"
                },
            ],
        };
    },
    methods: {
        sliderIndicator(id) {
            console.log(id);
            console.log(this.$refs.li);
            let el = this.$refs.li.id;
            console.log(el);
        }
    }
};


</script>

<style scoped>
* {
    margin: 0;
    padding: 0;
    border: 0;
    outline: 0;
    box-sizing: border-box;
    text-decoration: none;
    list-style: none;
}
nav {
    background: rgba(159, 54, 110, 0.7);
    width: max-content;
    display: block;
    padding: 0.7rem 1.7rem;
    z-index: 2;
    position: fixed;
    left: 50%;
    transform: translateX(-50%);
    bottom: 2rem;
    display: flex;
    gap: 0.8rem;
    border-radius: 3rem;
    backdrop-filter: blur(15px);
}

nav a {
    background: transparent;
    padding: 0.5rem;
    border-radius: 5%;
    display: flex;
    color: var(--color-text-menu);
    font-size: 1.1rem;
}

nav a:hover {
    background: var(--color-text-menu);
    color: var(--color-primary);
}

a.active {
    background: blue;
    color: green;
}
a {
    align-items: center;
}

a i {
    margin-right: 0.5rem;
    align-items: center;
}


/* ================ TABLETTE ============ */
@media screen and (max-width: 1024px) {

}

/* ================ PHONE ============ */
@media screen and (max-width: 600px) {
nav a {

    border-radius: 50px;
}

span {
    display: none;
}
a i {
    margin-right: 0;
}
}
</style>