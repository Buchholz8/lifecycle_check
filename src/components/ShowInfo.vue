<template>
  <div class="uno_div">
    <p>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Minus earum
      quasi iste? Eaque ut tempore nostrum nulla voluptas amet ea officiis sit
      labore asperiores saepe adipisci, dolorum voluptate ipsum accusamus.
    </p>
  </div>
</template>

<script>
export default {
    data() {
        return {
            tweets: [`tweet1`, `tweet2`, `tweet3`],
            num_friends: 0,
            logged_in: true
        }
    },
    methods: {
        show_info : function(){
            let uno_div = document.querySelector(`.uno_div`);
            uno_div.insertAdjacentHTML (`beforeend` , `<p> Friends : ${this.num_friends} </p>`),
            uno_div.insertAdjacentHTML (`beforeend` , `<p> ${this.logged_in} </p>`)
            for(let i = 0 ; i < this.tweets.length ; i++){
                let uno_div = document.querySelector(`.uno_div`);
               uno_div.insertAdjacentHTML(`beforeend` , `<p> ${this.tweets[i]} </p>`)
            }
        }
    },
    mounted: function() {
        this.show_info();
    }
}
</script>

<style scoped>
</style>