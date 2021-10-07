<template>
    <div>
        <div id="topbar">
            <div class="container-standard">
                <div class='flex wrap align-items-center justify-content-space-between'>
                    <div class='logo'>
                        <nuxt-link to="/" class='grid col-2 auto justify-content-start align-items-center'>
                            <img src="@/assets/img/logo.svg" alt="" class='logo mt20' />
                        </nuxt-link>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
#topbar {
    position: relative;
    top: 0px;
    left: 0px;
    width: 100%;
    background-color: #fff;
    z-index: 100;
    height: 68px;
}
.logo {
    height: 45px;
    border-radius: 50px;
}

#topbar > .container-standard {
    margin-top: 0px;
    margin-bottom: 0px;
    padding: 0px 20px;
    height: 100%;

    border-left: 0;
}
#topbar > .container-standard > div.flex {
    height: 100%;
}

.logo a {
    text-decoration: none;
    color: #000;
}
</style>
