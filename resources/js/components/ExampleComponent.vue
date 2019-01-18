<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-12">
                <div class="form-group">
                    <label for="greeting">Save Something:</label>
                    <input v-model="item" type="text" class="form-control" id="greeting" placeholder="Enter something">
                </div>

                <div class="form-group">
                    <button class="btn btn-block btn-info" v-on:click="addItem(item)">Save</button>
                </div>

                <ul v-for="item in items">
                    <li>{{ item }}</li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                item: '',

                items: [

                ]
            }
        },

        mounted() {

        },

        methods: {
            addItem(item) {
                this.items.push(item);
                this.item = '';
            }
        }
    }
</script>
