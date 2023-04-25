<template>
    <H1> Welcome to HTML Binding </H1>
    {{ text }}
   
   <div v-html="tag">

   </div>
   <div v-html="tag2">

   </div>

</template>

 

<script>
export default{
    name: "HtmlBin",
    data(){
        return {
            text: "Rahul Sonwane",
            tag: "<h1>  Pritam Sonwane <h1/>",
            tag2:"<h2> pritam@gmail.com"
        }
    }
    
}
</script>