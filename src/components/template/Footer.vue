<template>
    <footer class="footer">
        <span>Copyright <strong>MyTapp</strong> © 2016-2018</span>
    </footer>
</template>

<script>
export default {
    name: "Footer"
}
</script>

<style>
    .footer {
        grid-area: footer;
        background: -webkit-linear-gradient(90deg, rgb(156, 39, 176), rgb(103, 58, 183));
        background: linear-gradient(90deg, rgb(156, 39, 176), rgb(103, 58, 183));
        color: #fff;

        display: flex;
        align-items: center;
        justify-content: flex-end;
        padding-right: 10px;
    }
</style>
