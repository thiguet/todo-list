<template>
    <div class="">
        <input type="text" :value="value" @input.prevent="(evt) => onChangeValue(evt.target.value)" />
    </div>
</template>

<script>

// function debounce(func, timeout = 300){
//   let timer;
//   return (...args) => {
//     clearTimeout(timer);
//     timer = setTimeout(() => { func.apply(this, args); }, timeout);
//   };
// }

export default {
    // eslint-disable-next-line vue/multi-word-component-names
    name: "Search",
    props: {
        value: {
            type: String,
            required: true,
        },
        onChangeValue: {
            type: Function,
            required: true,
        }
    }

}
</script>

