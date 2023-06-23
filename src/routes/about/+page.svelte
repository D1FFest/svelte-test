<div class="container">
    <div class="info">
        <div class="animate-background">
            <div class="container info-container">
                <div class="info-text">
                    <h1> 
                        <p class="animate-text-1">About me</p>
                    </h1>
                </div>
                <h2 class="subtitle">Lorem ipsum dolor, sit amet consectetur adipisicing elit. Accusamus dicta voluptas pariatur alias rerum assumenda eum eligendi aperiam. Officiis vel quia fugiat quidem adipisci autem dolorum, exercitationem amet perferendis excepturi. <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Accusamus dicta voluptas pariatur alias rerum assumenda eum eligendi aperiam. Officiis vel quia fugiat quidem adipisci autem dolorum, exercitationem amet perferendis excepturi.</p> <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Odio perspiciatis quidem quaerat possimus provident et! Omnis alias repudiandae ea cumque hic magnam perferendis, magni facilis quam voluptatibus, pariatur dolorem et.</p> </h2>
                <!-- svelte-ignore a11y-no-noninteractive-tabindex -->
                <div style="color: black;" class="scroll-button animate-scroll" tabindex="0">
                </div>
            </div>
        </div>
    </div>
</div>
<div class="background-div"></div>
<style>
    .info {
        text-align: center;
        position: relative;
    }
    .info-container {
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        text-align: left;
        align-items: start;
    }
    .container {
        max-width: 1400px;
        margin: 190px 0 0 2.5rem;
        margin-top: 250px;
    }
    .info h1 {
        font-size: 4rem;
        margin: 0;
    }
    .info h1 p {
        position: relative;
        font: inherit;
        margin: 0;
        text-align: left;
        line-height: 130%;
        width: fit-content;
        font-weight: 800;
        letter-spacing: -0.03em;
    }
    .info h2 {
        max-width: 65ch;
        font-weight: 200;
        margin-top: 0.50rem;
    }
    .background-div {
        margin-top: 150px;
        background-color: #ecebe8;
        width: 100%;
        height: 62vh;
        margin: -205px auto;
        margin-top: -390px;
    }
    .info .info-text {
        position: relative;  
    }
    .scroll-button {
        display: flex;
        border: none;
        outline: none;
        cursor: pointer;
    }
    .animate-text-1{
        position: relative;
        top: 0px;
    }
    .subtitle{
        position: relative;
        top: 50px;
    }
</style>