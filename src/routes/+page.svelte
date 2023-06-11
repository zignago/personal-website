<script>
    import { goto } from '$app/navigation';
  
    function goToHomePage() {
        goto('/');
    }
  
    function goToContactPage() {
        goto('/contact');
    }
</script>

<div class="background-box"></div>

<header>
    <div class="header-container">
        <h1>Gian Zignago</h1>
        <nav>
            <ul>
                <li><a on:click={goToHomePage}>Home</a></li>
                <li><a on:click={goToContactPage}>Contact</a></li>
            </ul>
        </nav>
    </div>
</header>

<body>
</body>

<main>
    <div class="divider"></div>

    <div class="circle-image">
        <img src="/public/images/profile_picture.png" alt="Picture of me" class="image">
    </div> 

    <div class="divider"></div>

    <h2>Hi, I'm Gian.<br>I'm interested in finding mathematical solutions to some of the toughest problems in backend software development.</h2>

    <div class="divider"></div>

    <div class="container">
        <div class="box">
            <div class="box-content">
                <p><em>Currently</em></p>
                <p><strong>SWE</strong> at Cisco Meraki</p>
                <p><strong>Graduate Student</strong> at UCLA</p>
            </div>
        </div>
        <div class="box">
            <div class="box-content">
                <p><em>Past</em></p>
                <p><strong>Researcher</strong> at University of Missouri College of Engineering</p>
                <p><strong>SWE</strong> at Johns Hopkins University Applied Physics Lab</p>
                <p><strong>Network Research Engineer </strong> at MITRE</p>
                <p><strong>Software Architect</strong> at Missouri S&T Mars Rover Design Team</p>
                <p><strong>Satellite Communication Lead</strong> at Missouri S&T Satellite Research Team</p>
            </div>
        </div>
    </div>

    <div class="divider"></div>

    <p>Contact me<br></p>

</main>


<style>
    .background-box {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 128px; /* Adjust the height as needed */
        background-color: #FF8200; /* Same color as the header */
        z-index: -1; /* Place it behind the other content */
    }
  
    header {
        /*background-color: #00356b;*/
        background-color: #FF8200;
        padding: 20px;
        box-sizing: border-box;
        margin-top: 50px;
    }

    .header-container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        max-width: 1000px;
        margin: 0 auto;
    }

    main {
        /* display: flex;
        justify-content: space-between;
        align-items: center; */
        max-width: 1000px;
        margin: 0 auto;
    }

    h1 {
        font-family: "Spectral", sans-serif;
        font-weight: 700;
        margin: 0;
        /*color: #FF6600;*/
        color: #FFFFFF;
    }

    h2 {
        font-family: "DM Sans",sans-serif;
        font-weight: 70;
        font-size: 35px;
        margin: 0;
        /*color: #FF6600;*/
        color: #000000;
    }

    nav ul {
        font-family: "DM Sans",sans-serif;
        
        list-style-type: none;
        margin: 0;
        padding: 0;
    }

    nav li {
        display: inline;
        margin-left: 10px;
    }

    nav a {
        text-decoration: none;
        color: #FFFFFF;
    }

    .circle-image {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 200px;
        height: 200px;
        border-radius: 50%;
        overflow: hidden;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
    }

    .circle-image img {
        max-width: 120%;
        max-height: 120%;
    }

    .container {
        display: flex;
    }

    .box {
        width: 50%;
        padding: 20px;
        margin-right: 10px;
    }

    .box-content {
        font-family: "DM Sans",sans-serif;
        border: 10px solid #ffffff;
        background-image: linear-gradient(#eeeeee80 1px, transparent 1px),
                        linear-gradient(90deg, #eeeeee80 1px, transparent 1px);
        background-size: 10px 10px;
        padding: 10px;
        background-color: #FFffff;
    }

    .divider {
        height: 0px;
        background-color: #ccc;
        margin: 40px 0;
    }

    body {
        background-color: #ecebe6;
    }
</style>
