<style lang="scss">
   @import "../../static/scss/standeds.scss";
  
</style>

<script>
import CardItems from './UI/CardItem.svelte'; 

const chefDetails =[{
    id:1,
    name:'Pamela',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/avatar/avatar-0.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'12',
    rating:5
},{
    id:2,
    name:'Pamela',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/avatar/avatar-0.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'12',
    rating:5
},{
    id:3,
    name:'Pamela',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/avatar/avatar-0.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'12',
    rating:5
},{
    id:4,
    name:'Pamela',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/avatar/avatar-0.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'12',
    rating:5
}]
</script>
<section>
 <div class="row">
  {#each chefDetails  as item (item.id)}
  <CardItems  id={item.id}
      name={item.name}
      description={item.description}
      expreance={item.expreance}
       rating={item.rating}
      url={item.url}/>
  
  {/each}
 
 </div>
</section>