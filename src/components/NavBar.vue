<template>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
        <div class="container-fluid">
            <router-link class="navbar-brand" to="#"><img src="https://ismaaeel-a.github.io/allimages/Images/P-ismaaeel.jpg" alt=""></router-link>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav">

                    <li class="nav-item">
                        <router-link class="nav-link active" aria-current="page" href="#">Home</router-link>
                    </li>

                    <li class="nav-item">
                        <router-link class="nav-link" to="#">About</router-link>
                    </li>

                    <li class="nav-item">
                        <router-link class="nav-link" to="#">Resume</router-link>
                    </li>

                    <li class="nav-item">
                        <router-link class="nav-link" to="#">Projects</router-link>
                    </li>

                    <li class="nav-item">
                        <router-link class="nav-link" to="#">Testimonials</router-link>
                    </li>

                    <li class="nav-item">
                        <router-link class="nav-link" to="#">Contact</router-link>
                    </li>



                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
export default {

}
</script>

<style></style>