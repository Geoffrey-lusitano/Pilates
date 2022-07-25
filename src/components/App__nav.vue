<template>
    <ul class="menu">
        <nav class="menu-indicator">
            <li class="menu-item">
                <a href="#" class="menu-link">
                    <i class="menu-icon" ><font-awesome-icon icon="fa-regular fa-house" /></i>
                    <span>Accueil</span>  
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
                    icon: "fa-regular fa-house",
                    text: "Accueil",
                },
                {
                    id: 2,
                    icon: "fa-regular fa-badge-check",
                    text: "Présentation",
                },
                {
                    id: 3,
                    icon: "fa-regular fa-child-reaching",
                    text: "Pilates",
                },
                {
                    id: 4,
                    icon: "fa-regular fa-timer",
                    text: "Horaires & Tarifs"
                },
                {
                    id: 5,
                    icon: <font-awesome-icon icon="fa-regular fa-address-card" />,
                    text: "Contact",
                },
            ],
        };
    },
};


</script>

<style >
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
    background: rgba(0, 0, 0, 0.3);
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
    padding: 0.9rem;
    border-radius: 50%;
    display: flex;
    color: var(--color-light);
    font-size: 1.1rem;
}

nav a:hover {
    background: rgba(0, 0, 0, 0.2);
}

nav a.active {
    background: blue;
    color: green;
}
</style>