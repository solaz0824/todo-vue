<template>
    <button
            class="list-group-item text-left bg-info text-white"
            @click="clickButton"
          >{{ label }}</button>
</template>

<script>
export default {
    props: ['label'],
    methods: {
        clickButton() {
            this.$emit('componentClick')
        }
    }
}
</script>