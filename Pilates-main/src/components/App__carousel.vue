<template>
    <div class="carousel">
        <slot :currentSlide="currentSlide" />

        <!--- Navigation --->
        <div class="navigation">
            <div class="toggle_page left">
                <i @click="prevSlide" class="fa-solid fa-chevron-left"></i>
            </div>
            <div class="toggle_page right">
                <i @click="nextSlide" class="fa-solid fa-chevron-right"></i>
            </div>
        </div>
        <!--- Pagination -->
        <div class="pagination">
            <span @click="selectSlide(index)" v-for="(slide, index) in getSlideCount" :key="index" :class="{active : index + 1 === currentSlide}">
                
            </span>
        </div>
    </div>
</template>

<script>
import { ref, onMounted } from 'vue';
export default {
    setup () {
        const currentSlide = ref(1);
        const getSlideCount = ref(null);
        const autoPlayActived = ref(true);
        const timeoutDuration = ref(3000);

        // next slide
        const nextSlide = () => {
            if (currentSlide.value === getSlideCount.value) {
                currentSlide.value = 1;
                return;
            }
            currentSlide.value += 1;
        };

        // prev slide 
        const prevSlide = ( ) => {
            if (currentSlide.value === 1) {
                currentSlide.value = 1;
                return;
            }
            currentSlide.value -= 1;
        };
        // selec slide
        const selectSlide = (index) => {
            currentSlide.value = index + 1
        };
        // autoplay 
        const autoplay = () => {
            setInterval(() => {
                nextSlide()
            }, timeoutDuration.value);
        };

        if (autoPlayActived.value) {
            autoplay();
        }

        onMounted( () => {
            getSlideCount.value = document.querySelectorAll(".slide").length;
        });

        return { currentSlide, nextSlide, prevSlide, getSlideCount, selectSlide };
    }
}

</script>

<style scoped>
.navigation {
    padding: 0 16px;
    height: 100%;
    width: 100%;
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
}
.toggle_page {
    display:flex;
    flex: 1;
}
.right {
    justify-content: flex-end;
}
i { 
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content:center;
    border-radius:3rem;
    width: 40px;
    height: 40px;
    background-color: var(--color-primary);
}

/*  */
.pagination {
    position: absolute;
    bottom: 24px;
    width: 100%;
    display: flex;
    gap: 16px;
    justify-content: center;
    align-items: center;
}
span {
    cursor: pointer;
    width: 20px;
    height: 20px;
    border-radius: 3rem;
    background-color: var(--color-text-menu);
    box-shadow: rgba(0, 0, 0, 0.15) 0px 2px 8px;
}
.active {
    background-color: var(--color-primary);
}
</style>