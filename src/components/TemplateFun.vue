<template>
    <div >
        <button @click="toggle_post" > Toggle logged in status</button>
        <div v-if="show_post === true">
             <h4> {{blog_title}} </h4>
        <p> {{blog_content}} </p>
        <img :src="blog_image_url" />
        <button @click="hack_post"> Click Me</button>
        
        </div>
        <div v-else>
        <p>Please Sign in</p>
        </div>
        
    </div>
    
</template>

<script>
    export default {
       data() {
        return {
            show_post: true,
            blog_content: `This is blog content`,
            blog_title: `Cool Blog`,
            blog_image_url: `https://images.pexels.com/photos/15828302/pexels-photo-15828302.jpeg?auto=compress&cs=tinysrgb&w=1600&lazy=load`
        }
       } ,
       methods: {
        hack_post: function(){
            this.blog_content += `this is hacked content` 
        },
        toggle_post: function() {
            this.show_post = !this.show_post
        },
       }
       

    }
</script>

<style scoped>
img{
    height: 100px;
    width: 100px;
}
</style>