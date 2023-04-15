<template>
  <div>
    <h3>Totally A Title</h3>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam dolorem,
      culpa beatae, officia ea fugiat, officiis totam esse quisquam repudiandae
      earum! Consequuntur commodi saepe nostrum impedit quidem et ipsam aperiam.
    </p>
    <h6>This was a cool thing i learned</h6>
    <p>
      Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto, ut! Libero
      reprehenderit, excepturi laudantium perferendis nihil recusandae
      voluptate, illum alias consectetur quisquam vero nesciunt! Deleniti
      corrupti possimus dolore non quidem?
    </p>
  </div>
</template>

<script>
export default {
    beforeCreate: function() {
        console.log(`this runs when 'before create' does`)
    },
    created: function() {
        console.log(`this runs when 'created' does`)
    },
    beforeMount: function() {
        console.log(`this runs when 'before mount' does`)
    },
    mounted: function() {
        console.log(`this runs when 'mounted' does`)
    }
};
</script>

<style scoped>
</style>