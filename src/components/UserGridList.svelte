<style lang="scss">
   @import "../../static/scss/standeds.scss";
  
</style>

<script>
import CardItems from './UI/CardItem.svelte'; 

const chefDetails =[{
    id:1,
    name:'Nunna Sudheer Chowdary',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/photo/photo-1484154218962-a197022b5858.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'8',
    rating:5
},{
    id:2,
    name:'Kumar Nunna',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/photo/photo-1426122402199-be02db90eb90.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'9',
    rating:2
},{
    id:3,
    name:'Rishitha',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/photo/photo-1512917774080-9991f1c4c750.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'5',
    rating:4
},{
    id:4,
    name:'Mahi',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/photo/photo-1494526585095-c41746248156.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'6',
    rating:1
},
{
    id:5,
    name:'Pamela',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/photo/photo-1522771739844-6a9f6d5f14af.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'5',
    rating:3
},
{
    id:6,
    name:'Pamela',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/photo/photo-1494526585095-c41746248156.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'10',
    rating:2
},
{
    id:7,
    name:'Pamela',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/photo/photo-1494526585095-c41746248156.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'12',
    rating:1
},
{
    id:8,
    name:'Pamela',
    url:'https://d19m59y37dris4.cloudfront.net/directory/1-5/img/photo/photo-1488805990569-3c9e1d76d51c.jpg',
    description:'Modern, Well-Appointed Room',
    expreance:'2',
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