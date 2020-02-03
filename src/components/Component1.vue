<template>
    <!--    string is null, it cannot meet the condition in v-if as string.length > 0-->
    <!--    Change "string.length > 0" to "string == null"-->
    <div v-if="string == null">
        <p>Congrats you have discovered the issue</p>
        <p>Don't forget to commit this solution</p>
    </div>
</template>

<script>
    export default {
        name: 'Component1',
        data() {
            return {
                string: null
            }
        }
    }
</script>