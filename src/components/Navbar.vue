<script setup>

</script>

<template>
  <header>
    <div class="topheader">

        <div class="leftbar">
            <span @click="">langauggio</span>
        </div>
        <nav class="centerbar">
            <a href=""><span>visit</span></a>
            <a href=""><span>art e news</span></a>
            <a href=""><span>hglogo</span></a>
            <a href=""><span>visit</span></a>
            <a href=""><span>visit</span></a>
            <img src="https://peakvisor.com/img/news/mount_fuji.jpg" alt="">

        </nav>
        <div class="rightbar">  
            <span class="buyticket">
                comprare
            </span>
        </div>

    </div>
    <h1 class="title">
        one museum
    </h1>

    
</header>
</template>

<style scoped lang="scss">
header{
    background-color:rgb(252, 227, 115);
    font-family:raisonne-demibold,Raisonne,Futura,Helvetica,Arial,sans-serif;
    padding: 10px 20px;
    .topheader{
    display: flex;
    justify-content: space-between;
        .leftbar{
            padding:30px 20px;
            span{
             border:2px solid rgba(48, 48, 48, 0.307);
             border-radius:30px;
             padding: 15px 10px;
             
            }
        }      
        .centerbar{
          padding:30px ;
          font-size:25px ;
          display: flex;
          gap: 15px;  
            img{
                max-width:100px;
            }
        }
        .rightbar{
        
        }
    }
}
a{
  text-decoration: none;
  color: black;
}

</style>
