<template>
    <div>
        <div class="title"><span>Dev</span>challenges.io</div>
        <div class="navBar">
            <ul class="navbar-nav pe-3">
                <li class="nav-item mb-3">
                    <a class="nav-link" href="#">Typography</a>
                </li>
                <li class="nav-item mb-3">
                    <a class="nav-link" href="#">Grid</a>
                </li>
                <li class="nav-item mb-3">
                    <a class="nav-link" href="#">Buttons</a>
                </li>
                <li class="nav-item mb-3">
                    <a class="nav-link" href="#"><b>Inputs</b></a>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Navigation-container"
    }
</script>

<style scoped>
.title {
    margin-bottom: 79px;
    font-family: 'Poppins', sans-serif;
    font-weight: 600;
    font-size: 13px;
    line-height: 19.5px;
    color: #090F31;
}

.title span {
    color: #F7542E;
}

.navBar .nav-link {
    font-family: 'Noto Sans', sans-serif;
    font-weight: 500;
    font-size: 14px;
    line-height: 20.27px;
    color: #9E9E9E;
}

.navBar .nav-link b {
    color: #090F31;
}
</style>