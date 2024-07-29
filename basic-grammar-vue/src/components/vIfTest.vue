<script>
export default {
    data() {
        return {
            visible : true,
            unvisible: false,
        };
    },
};
</script>
<template>
    <p v-if="visible">이 요소 렌더링됨</p>
    <p v-if="unvisible">이 요소 렌더링 안됨</p>
    <p v-else>요소 렌더링 안됐음</p>
</template>
<style></style>