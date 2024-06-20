<template>
    <button>
        <div class="container">
            <div>
                <h3> {{ name }}</h3>
                <span> {{ date }}</span>

            </div>
            <div>
                <span> {{ status }}</span>
            </div>
        </div>
    </button>
</template>
<script>
export default {
    props: {
        name: {
            type: String
        },
        date: {
            type: String
        },
        status: {
            type: String
        }
    },
    data() {
        return
    },
    name: 'Item'
}
</script>

<style scoped>
.container {
    display: flex;
    align-items: center;
    justify-content: space-between;

}
</style>