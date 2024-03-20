<script>
    import MainNav from '../../components/MainNav.svelte';
    import { onMount } from 'svelte';
    import Pic from '$lib/assets/headshot.jpg';
    import Github from '$lib/assets/github.svg';
    import Insta from '$lib/assets/insta.png';
    import Linked from '$lib/assets/linkedin.png';
    import Twitter from '$lib/assets/x.jpg';
    
 </script>
<style>
    .main {
        text-align: center;
        height: 100%;
        width: 100%;
        margin: 0px;
        padding: 0px;
        
        
    }

    .body {
        display: flex;
        flex-direction: row;
        height: 80%;
        margin: auto;
        margin-top: 60px;
        width: 90%;
        
    }
    
    .aprilPic{
        margin-right: 20px;
        height: 90%;
    }
    .image{
        
        height: 100%;
        flex-basis: 35%;
        display:flex;
        flex-direction: row-reverse;
    }

    .content {
        display: flex;
        flex-direction: column;
        margin-top: 30px;
        height: 70%;
        flex-basis: 65%;
        
    }

    .name {
        font-size: 60px;
        font-family: ui-serif, Georgia, Cambria, "Times New Roman", Times, serif;
        font-weight: 200;
    }

    .greeting {
        margin-bottom: 20px; 
    }

    .github {
        height: 30px;
    }

    .about, .hobbies, .contact {
        margin-bottom: 20px;
        margin-top: 20px;
        font-size: 20px;
    }

    .links {
        display: flex;
        flex-direction: row;
        width: 100%;
        
        place-content: center;
        
    }

    .music {
        
        width: 80%;
        margin: auto;
    }

    h1 {
        
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
    <div class="body">
        <div class="image">
            <img class= "aprilPic" src={Pic} alt="pic of me"/>
        </div>
        <div class="content">
            <div class="greeting">
                <h1 style="font-size: 20px">Hello, I'm</h1>
                <h1 class="name">April Hsu</h1>
            </div>
            <div class="about">
                <p>
                    I'm a 3rd year CE student at UCSD. I've taken classes in circuit analysis, advanced data structures, systems and signals, algorithms, and more. I am also self-taught in web development: I have experience with HTML, CSS, Javascript, Django, Svelte, and Tailwind. 
                </p>
            </div>
            <div class="hobbies">
                <p>
                    In my free time, I enjoy reading, knitting, cooking, gaming, and more. I'm also a big enjoyer of music, from C-pop to rock to metal. In fact, I've included one of my current favorite playlists below. Give it a listen and let me know what you think!
                </p>
            </div>
            <div class="music">
                <iframe style="border-radius:12px" src="https://open.spotify.com/embed/playlist/0S3vImVdXdqPNGKJ2MvA68?utm_source=generator&theme=0" width="100%" height="152" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
            </div>
            <div class="contact">
                <p>
                    If you want to get in touch, feel free to check me out on any of the platforms below!
                </p>
            </div>
            <div class="links">
                <a class="github" href="https://github.com/maotcha?tab=repositories"><img src={Github} alt="Github link" style="height:25px; margin:8px;"></a>
                <a class="insta" href="https://www.instagram.com"><img src={Insta} alt="Insta link" style="height:25px; margin:8px;"></a>
                <a class="linkedin" href="https://www.linkedin.com"><img src={Linked} alt="LinkedIn link" style="height:25px; margin:8px;"></a>
                <a class="twitter" href="https://twitter.com"><img src={Twitter} alt="Twitter link" style="height:25px; margin-top:8px; margin-bottom:8px; margin-right:4px; margin-left:4px;"></a>
            </div>
        </div>
    </div>
    
</div>
