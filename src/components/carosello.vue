<script >
 export default{
     data(){
        return{
            obs:0,
            Arrimg:[
            'https://www.google.com/imgres?imgurl=https%3A%2F%2Fartgallery.yale.edu%2Fsites%2Fdefault%2Ffiles%2Fstyles%2Fopengraph%2Fpublic%2F2023-01%2Fag-doc-2281-0036-pub.jpg%3Fh%3D147a4df9%26itok%3D3138ahl0&tbnid=XRjujFPohxlmZM&vet=12ahUKEwjQ45Ce5_WDAxU4ov0HHa0DDpUQMygJegQIARBl..i&imgrefurl=https%3A%2F%2Fartgallery.yale.edu%2Fresearch-and-learning%2Fcuratorial-areas&docid=903dNOrNIs3jeM&w=1200&h=630&q=art%20museum&ved=2ahUKEwjQ45Ce5_WDAxU4ov0HHa0DDpUQMygJegQIARBl',
            'https://www.google.com/imgres?imgurl=https%3A%2F%2Fi.guim.co.uk%2Fimg%2Fmedia%2F24b0e2a9f495c9844826afdffe46cafbf2b168f1%2F0_228_3500_2101%2Fmaster%2F3500.jpg%3Fwidth%3D700%26quality%3D85%26auto%3Dformat%26fit%3Dmax%26s%3D698b616ed07970392754e4032f3d5722&tbnid=yQj8l3PU57Og-M&vet=12ahUKEwjQ45Ce5_WDAxU4ov0HHa0DDpUQMygEegQIARBb..i&imgrefurl=https%3A%2F%2Fwww.theguardian.com%2Ftravel%2F2020%2Fmar%2F23%2F10-of-the-worlds-best-virtual-museum-and-art-gallery-tours&docid=bNUGKWpxD84OQM&w=700&h=420&q=art%20museum&ved=2ahUKEwjQ45Ce5_WDAxU4ov0HHa0DDpUQMygEegQIARBb',
            'https://www.google.com/imgres?imgurl=https%3A%2F%2Fd26jxt5097u8sr.cloudfront.net%2Fs3fs-public%2F2021-12%2F2021-11-18_Hamilton_WtC_Visitors_27.jpg&tbnid=1x5PmhXmAMOMoM&vet=12ahUKEwjQ45Ce5_WDAxU4ov0HHa0DDpUQMygFegQIARBd..i&imgrefurl=https%3A%2F%2Fwww.denverartmuseum.org%2Fen%2Fart&docid=JUP96QCDyZUQvM&w=3000&h=2001&q=art%20museum&ved=2ahUKEwjQ45Ce5_WDAxU4ov0HHa0DDpUQMygFegQIARBd',
            'https://www.google.com/url?sa=i&url=https%3A%2F%2Ffristartmuseum.org%2F&psig=AOvVaw14m03c24kBlt-vgNFJ90qs&ust=1706178201228000&source=images&cd=vfe&opi=89978449&ved=0CBIQjRxqFwoTCKiYn5_n9YMDFQAAAAAdAAAAABAD',
            ]
        }
        
     },
     methods:{
        leftarrow(){  
            this.obs -- 
        }, 
        rightarrow(){
            this.obs ++
        }
     }
 }

</script>


<template>
<div class="main-carosello">
    <h1>what's on</h1>
    <div class="carosello">
        <div class="left-arrow" @click="">
            <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor" class="bi bi-arrow-left-square" viewBox="0 0 16 16">
            <path fill-rule="evenodd" d="M15 2a1 1 0 0 0-1-1H2a1 1 0 0 0-1 1v12a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1zM0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2zm11.5 5.5a.5.5 0 0 1 0 1H5.707l2.147 2.146a.5.5 0 0 1-.708.708l-3-3a.5.5 0 0 1 0-.708l3-3a.5.5 0 1 1 .708.708L5.707 7.5z"/>
            </svg>
        </div>
        <div class="imgcar" v-for="(n,i) in Arrimg " :key="i" >
            <img v-if="obs == i" :src="this.Arrimg[i]" alt="">
        </div>
        <div class="right-arrow">
            <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" fill="currentColor" class="bi bi-arrow-right-square" viewBox="0 0 16 16">
            <path fill-rule="evenodd" d="M15 2a1 1 0 0 0-1-1H2a1 1 0 0 0-1 1v12a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1zM0 2a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v12a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2zm4.5 5.5a.5.5 0 0 0 0 1h5.793l-2.147 2.146a.5.5 0 0 0 .708.708l3-3a.5.5 0 0 0 0-.708l-3-3a.5.5 0 1 0-.708.708L10.293 7.5z"/>
            </svg>

        </div>
    </div>
    <span>
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-calendar3" viewBox="0 0 16 16">
        <path d="M14 0H2a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2M1 3.857C1 3.384 1.448 3 2 3h12c.552 0 1 .384 1 .857v10.286c0 .473-.448.857-1 .857H2c-.552 0-1-.384-1-.857z"/>
        <path d="M6.5 7a1 1 0 1 0 0-2 1 1 0 0 0 0 2m3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2m3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2m-9 3a1 1 0 1 0 0-2 1 1 0 0 0 0 2m3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2m3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2m3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2m-9 3a1 1 0 1 0 0-2 1 1 0 0 0 0 2m3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2m3 0a1 1 0 1 0 0-2 1 1 0 0 0 0 2"/>
        </svg> 
        view all events
    </span>
    
</div>

</template>


<style scoped lang="scss" >
.main-carosello{
 background-color: rgb(204,166,154);
 padding: 200px;
 display:flex ;
 flex-direction: column;
 align-items: center;
 gap: 100px;
  h1{
    
  }

  .carosello{
    display: flex;
    width:100%;
    justify-content: space-between;
    .left-arrow{

    }
  }
   span{
   background-color: black;
   color: gold; 
   padding:10px;
   border-radius: 50px;
   font-size: 20px;
  }
}

</style>
