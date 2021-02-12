<template>
    <div>
        <h1>Hi! I am a reverse component!</h1>
        <h2>Enter text above and I will display it in reverse!</h2>
        {{reverseText(text)}}
    </div>
</template>

<script>
export default {
    name:'Reverse',
    props:["text"],

    methods:{
        reverseText(str){
            let arrStr = str.split("")
            let arrReverse = arrStr.reverse()
            let joinRev = arrReverse.join("")
            return joinRev;
        }
    },

}
</script>