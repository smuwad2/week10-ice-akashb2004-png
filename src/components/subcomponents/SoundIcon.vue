<script>
    export default { 
        data() {
            return {
                soundEmojis: ['🔇', '🔈', '🔉', '🔊']
            }
        },

        props :{
            level : {
                type : Number,
                required : true,
                validator : v => [0,1,2,3].includes(v)
            }
        }
        // TODO: add code to define a necessary prop
    }
</script>

<template>
    <!-- TODO: add your template code here. Use span element. --> 
    <span>{{ soundEmojis[level] }}</span>
</template>