<template>
    <nav class="navbar navbar-expand-lg bg-body-tertiary">
        <div class="container-fluid">
            <router-link class="navbar-brand" to="#"><img src="https://ismaaeel-a.github.io/allimages/Images/plc.png" alt="logo"></router-link>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav"
                aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto px-3">

                    <li class="nav-item">
                        <router-link class="nav-link mx-2 active" aria-current="page" to="/">Home</router-link>
                    </li>

                    <li class="nav-item">
                        <a class="nav-link mx-2" href="#about">About</a>
                    </li>

                    <li class="nav-item">
                        <a class="nav-link mx-2" href="#resume">Resume</a>
                    </li>

                    <li class="nav-item">
                        <a class="nav-link mx-2" href="#project">Projects</a>
                    </li>

                    <li class="nav-item">
                        <a class="nav-link mx-2" href="#testimonials">Testimonials</a>
                    </li>

                    <li class="nav-item">
                        <a class="nav-link mx-2" href="#reachMe">Contact</a>
                    </li>



                </ul>
            </div>
        </div>
    </nav>
</template>