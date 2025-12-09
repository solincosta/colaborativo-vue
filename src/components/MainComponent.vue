<template>
    <main class="contenedor">
        <div class="banner-grande">
            <img class="imagen-grande" src="../assets/ps5.jpg" alt="">
        </div>
        <div class="columna-imagenes">
            <div class="cuadros fondo-play-5">

            </div>
            <div class="cuadros fondo-play-4">

            </div>
            <div class="cuadros fondo-switch">

            </div>
            <div class="cuadros fondo-360">

            </div>
        </div>
    </main>
</template>

<script>
export default {
    name: "MainComponent"
}
</script>

<style scoped>
.contenedor {
    height: 400px;
    width: 80%;
    margin: 5rem 10%;

    /* TAMAÑO, COLOR, TIPO */
    display: flex;
    gap: 1.5rem;
}

.banner-grande {
    width: 75%;
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;

}

.imagen-grande {
    height: 100%;
    width: 100%;
}

.columna-imagenes {
    width: 25%;
    display: flex;
    gap: 0.8rem;
    flex-direction: column;
}


.cuadros {
    flex-grow: 1;
    box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;

    /* background-image: url("assets/ps4.jpg");
    background-position: center center;
    background-size: cover; */
}

.fondo-play-5 {
    background-image: url("../assets/ps5.jpg");
    background-position: center center;
    background-size: cover;
}

.fondo-play-4 {
    background-image: url("../assets/ps4.jpg");
    background-position: center center;
    background-size: cover;
}

.fondo-switch {
    background-image: url("../assets/switch-2.jpg");
    background-position: center center;
    background-size: cover;
}

.fondo-360 {
    background-image: url("../assets/Consola-Xbox-One.png");
    background-position: center center;
    background-size: cover;
}



</style>