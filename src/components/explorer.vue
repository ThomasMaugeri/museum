<script >



</script>

<template>
<div class="body">
    <div class="left">
        <div class="left-up">
            <img src="https://upload.wikimedia.org/wikipedia/commons/6/63/PhiladelphiaMuseumOfArt2017.jpg" alt="">
        </div>
        <div class="left-down">
            <img src="https://bdc2020.o0bc.com/wp-content/uploads/2023/02/Museum-of-Fine-Arts-Horses-of-Achilles-63ed3cbe3a5a1-scaled.jpeg" alt="">
        </div>       
    </div>
    <div class="right">
        <div class="right-up">
            <h1>locations</h1>
            
            <h2>One museum two locations</h2> 
            
            <p>Welcome to the Frans Hals Museum - The art museum of Haarlem - With art from the 16th and 17th centuries, modern and new art and a stimulating mix of both.</p>

        </div>
        <div class="right-down">
            skgvdgml
        </div>
    </div>
</div>

</template>

<style scoped lang="scss" >
.body{
    width: 100%;
    height: 1000px;
    display: flex;
    
    .left{
        width: 50%;
        display: fixed;
        img{
            width: 100%;
           height: 500px;
           display: block;
           
        }
    }
    .right{
        width: 50%;
        
        
        .right-up{
            background-color: red;
            height:750px;
            display: flex;
            flex-direction: column;
            gap:100px;
            h1{
                padding: 50px 50px;
            }
            p{
                
            }
        }
        .right-down{
            height: 1000px;
            background-color: purple;
            display:flex;
            flex-direction: column-reverse;
            
        }
    }
}


</style>
