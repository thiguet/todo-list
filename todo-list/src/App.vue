<script setup lang="ts">
import Item from './components/Item.vue'
</script>

<template>
    <div id="container">
        <ul>
            <li>
                <button>
                    <Item name="Buy groceries" date="22/01/2023 at 1:00 PM " status="Pendente"> </Item>
                </button>
            </li>
            <li>
                <button>
                    <Item name="Finish homework" date="22/02/2023 at 7:00 AM " status="Pendente"> </Item>
                </button>
            </li>
            <li>
                <button>
                    <Item name="Call mon" date="12/05/2023 at 4:00 PM" status="Pendente "> </Item>
                </button>
            </li>
            <li>
                <button>
                    <Item name="go for a run" date="30/03/2023 at 9:00 AM " status="Pendente"> </Item>

                </button>
            </li>
            <li>
                <button>
                    <Item name="Read a book" date="02/05/2023 at 8:00 PM " status="Completed"> </Item>
                </button>
            </li>
            <li>
                <button>
                    <Item name="Write a-blog post" date="12/01/2023 at 5:00 AM " status="Pendente"> </Item>

                </button>
            </li>
            <li>
                <button>
                    <Item name="Attend a meeting" date="08/01/2023 at 1:00 PM " status="Pendente"> </Item>
                </button>
            </li>
            <li>
                <button>
                    <Item name="Clean the House" date="23/01/2023 at 3:00 AM " status="Completed"> </Item>
                </button>
            </li>
            <li>
                <button>
                    <Item name="Ptractice Playing Guitar" date="17/01/2023 at 6:00 AM " status="Completed"> </Item>
                </button>
            </li>





        </ul>
    </div>
</template>
<style>
ul {
    list-style-type: none;
}

button {
    border-radius: 5px;
    border: none;
    background-color: white;
    text-align: start;
    cursor: pointer
}
</style>