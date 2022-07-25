<template>

<p v-text="newPlayers"></p>
{{players.length}}
<div v-if="players.length>0">
    {{players}}

</div>
<div v-else>
    no player found
</div>

<p v-html="`<h1 style='color:green'>${newPlayers}</h1>`"></p>


<ul>
    <li >
        {{players}}
    </li>
</ul>
<input type="text" :value="newPlayer">
<img :src="image">


</template>

<script>
export default {
    data() {

        return{
            players:[
                "ward", "moath","omar"

            ],
            newPlayer:"salem",
            image:"/src/assets/images.png"
            

           
        }

    }
   


}
</script>

<style>

</style>