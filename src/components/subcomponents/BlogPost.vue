<script>
    export default {
        // Add code if/as necessary
        // Hint: Add properties subject, entry and mood
        computed : {
            feel (){
                return "/assets/" + this.mood.toLowerCase() + ".png"
            }
        },

        props : {
            id: String,
            subject: String,
            entry: String,
            mood: String,
        }
    }
</script>


<template>
    <!-- TODO: add your template code here. Use boostrap card --> 
    <div class="card mx-auto" style="width: 24 rem;">
        <img :src="feel" class="card-img-top" alt="Image cap"></img>
        <div class="card-body">
            <h5 class="card-title">Blog {{ id }} Subject {{ subject }}</h5>
            <p class="card-text"> {{ entry }}</p>
            <hr size="10" no shade></hr>
            <br></br>
        </div>
    </div>
</template>

