<template>
    <footer id="footer">
        <p>Pet App &copy; 2023</p>
    </footer>
</template>

<script>
export default {
    name: 'Footer',
}
</script>

<style scoped>
#footer {
    height: 200px;
    background-color: var(--roxo-1);
    border-top: 4px solid var(--roxo-2);
    color: var(--branco);
    display: flex;
    align-items: center;
    justify-content: center;
    bottom: 0;
    width: 100%;
}
</style>