<script></script>
<template>
    <div>
        <button>LOAD MORE</button>
    </div>
</template>
<style lang="scss" scoped>
@use 'src/assets/scss/_var.scss' as *;

div {
    display: flex;
    justify-content: center;
    align-items: center;

    button {
        padding: 5px 25px;
        margin: 20px 0;
        color: white;
        background-color: $blue;
        border-color: $blue;
        cursor: pointer;
        font-weight: 700;
    }
}
</style>