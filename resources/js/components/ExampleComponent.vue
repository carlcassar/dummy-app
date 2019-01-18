<template>
    <div class="container">
        <div class="row justify-content-center">
            <div class="col-md-12">
                <form>
                    <div class="form-group">
                        <label for="greeting">Greeting:</label>
                        <input v-model="greeting" type="greeting" class="form-control" id="greeting" placeholder="Enter a greeting">
                    </div>
                </form>

                <h2>{{ greeting }}</h2>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                greeting: ''
            }
        },

        mounted() {

        },

        methods: {

        }
    }
</script>
