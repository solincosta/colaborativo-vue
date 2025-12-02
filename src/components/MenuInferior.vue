<template>
    <menu id="menu_id" class="menu">
        <li class="item-menu"><span class="material-symbols-outlined">
                settings
            </span> Home </li>
        <li class="item-menu"><span class="material-symbols-outlined">
                settings
            </span> Tienda</li>
        <li class="item-menu"><span class="material-symbols-outlined">
                settings
            </span> Noticias</li>
        <li class="item-menu"><span class="material-symbols-outlined">
                settings
            </span> Nuestro Shop</li>
        <li class="item-menu"><span class="material-symbols-outlined">
                settings
            </span> Productos</li>
    </menu>
</template>

<script>
export default {
    name: 'MenuInferior'
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=GROBOLD&display=swap');

.material-symbols-outlined {
  font-variation-settings:
  'FILL' 0,
  'wght' 400,
  'GRAD' 0,
  'opsz' 24
}


.menu {
    background-color: #F9C30D;
    height: 50px;
    display: flex;
    justify-content: center;
    align-items: center;
    position: relative;
    top: 0;
    right: 0;

}

.item-menu {
    list-style: none;
    height: 100%;
    display: flex;
    gap: 10px;
    justify-content: center;
    align-items: center;
    padding: 0 1rem;
    font-family: 'GROBOLD', sans-serif;
}

.item-menu:hover {
    background-color: black;
    color: white;
    cursor: pointer;
}
</style>