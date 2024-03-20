<script>
    import Cat from "$lib/assets/cat.jpg";
    import MainNav from '../../components/MainNav.svelte';
    import { onMount } from 'svelte';

    
 </script>
<style>
    .main {
        text-align: center;
        height: 100%;
        width: 100%;
        margin: 0px;
        padding: 0px;
    }

    .catPic{
        width:40%;
    }

    .header{
        
        margin: 10px;
    }

    .image {
        font-size: 15px;
        margin: 0px;
        color: orange;
    }

    .aboutMe {
        margin: 20px;
        font-size: 25px;
        color: palevioletred;
    }

    .moreaboutme {
        margin: 20px;
        font-size: 25px;
        color: rgb(251, 27, 184);
    }

    .lastone {
        margin: 20px;
        font-size: 25px;
        color: rgb(117, 223, 255);
    }

    .music{
        width: 100%;
        height: 380px;
        margin-top: 40px;
    }

    h1 {
        color: aqua;
        margin: 0px;
        
    }

    h2 {
        color: greenyellow;
        margin: 0px;
    }

    p {
        margin: 0px;
    }

</style>

<div class="main">
    <MainNav/>
    <div class="header">
        <h1>Hi, I'm April!</h1>
        <h2>Welcome to my Website!</h2>
    </div>
    
    <div class="image">
        <img class= "catPic" src={Cat} alt="cat pic"/>
        <p>(No, this is not an image of me. I just figured you'd rather see a picture of a cute cat than a picture of me)</p>
    </div>
   
    <div class="aboutMe">
        <p>I'm a UCSD student! I like CS! I (kinda) like EE! I like cats! Please give me a job/internship! Pretty Please! Click on this totally not sketchy <a target="_blank" href="https://docs.google.com/document/d/1-SZ7xHx1WK8bedwBdSk393WlmnosLlET-Oh0vy7Ml_U/edit?usp=sharing">link</a> to see my resume! Also, check out this awesome performance by Ghost!!!</p>
    </div>
   
    <div class="music">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/NmxFxBiCrL4?si=3CU0ne8uQcqwzVeK" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>

    <div class="moreaboutme">
        <p>Wasn't that sick!?!!? Ok, ok, ok, now check out this performance by Bring Me the Horizon. I promise it'll be the best thing you've heard all day!!!</p>
    </div>

    <div class="music">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/OGc9W-_C9u0?si=GWqlyioouyO6Jv-Y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>

    <div class="lastone">
        <p>Ok, this is the last one I promise. It's Coldplay! I love Coldplay! You love Coldplay! We all love Coldplay!</p>
    </div>

    <div class="music">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/kiqEEr7CK2g?si=bOz0bTjscl7zMQCn" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
    </div>
</div>
