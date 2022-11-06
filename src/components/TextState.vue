<script>
export default {
    name: "TextState",
    data: function(){
        return{
            manOneObj:{
                name: 'khan',
                age: 27,
                designation: 'software engg'
            }
        }
    }
}
</script>

<template>

    <div>
        <h1 class="text-2xl">TextState Component: take state vaule</h1>
        <ul>
            <li>
                name: {{this.manOneObj.name}}
            </li>
            <li>
                name: {{this.manOneObj.age}}
            </li>
            <li>
                name: {{this.manOneObj.designation}}
            </li>
        </ul>
    </div>
</template>