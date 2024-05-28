<script>
    import ImageGallery from "$lib/Image_Gallery.svelte";
    let currentTab = "Paintings";

    function switchTab(tab) {
        currentTab = tab;
    }
</script>

<div class="tabs">
    <button class="tab-button" on:click={() => switchTab("Paintings")}>
        Paintings
    </button>
    <button class="tab-button" on:click={() => switchTab("Blender")}>
        Blender
    </button>
    <button class="tab-button" on:click={() => switchTab("Inkscape")}>
        Inkscape
    </button>
    <button class="tab-button" on:click={() => switchTab("Ui")}>
        Web design
    </button>
    <button class="tab-button" on:click={() => switchTab("Projects")}>
        Projects
    </button>
</div>

<div class="tab-content">
    {#if currentTab === "Paintings"}
        <h3>Paintings</h3>
        <div class="image-container">
            <div class="image-column">
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
                <ImageGallery />
            </div>
            <div class="image-column">
                <img src="/Images/arch.png" alt="Grapes" class="images" />
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
            </div>
            <div class="image-column">
                <img src="/Images/painting.jpg" alt="Grapes" class="images" />
            </div>
            <div class="image-column">
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
            </div>
        </div>
    {:else if currentTab === "Blender"}
        <div class="image-container">
            <div class="image-column">
            <div class="sketchfab-embed-wrapper" style="width: 50%;">
                <iframe title="Rabbit" frameborder="0" allowfullscreen mozallowfullscreen="true" webkitallowfullscreen="true" allow="autoplay; fullscreen; xr-spatial-tracking" xr-spatial-tracking execution-while-out-of-viewport execution-while-not-rendered web-share src="https://sketchfab.com/models/4cf175ddd8d94c7f8705d0d3b9586e6e/embed">
                </iframe>
            </div>
            </div>
            <div class="image-column">
                <img src="/Images/arch.png" alt="Grapes" class="images" />
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
            </div>
            <div class="image-column">
                <img src="/Images/painting.jpg" alt="Grapes" class="images" />
            </div>
            <div class="image-column">
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
            </div>
        </div>
    {:else if currentTab === "Inkscape"}
        <div class="image-container">
            <div class="image-column">
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
                <ImageGallery />
            </div>
            <div class="image-column">
                <img src="/Images/arch.png" alt="Grapes" class="images" />
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
            </div>
            <div class="image-column">
                <img src="/Images/painting.jpg" alt="Grapes" class="images" />
            </div>
            <div class="image-column">
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
            </div>
        </div>
    {:else if currentTab === "Ui"}
        <div class="image-container">
            <div class="image-column">
                <img src="https://blog.hubspot.com/hs-fs/hubfs/telerik-homepage-update.png?t=1502725308401&width=1347&name=telerik-homepage-update.png" alt="Grapes" class="images" />
            </div>
            <div class="image-column">
                <img src="https://webneel.com/daily/sites/default/files/images/daily/02-2014/10-beautiful-websites.jpg" alt="Grapes" class="images" />
                <img src="https://agentestudio.com/uploads/ckeditor/pictures/1731/18.jpg" alt="Grapes" class="images" />
            </div>
            <div class="image-column">
                <img src="https://www.founderjar.com/wp-content/uploads/2021/03/Best-Website-Designs.jpg" alt="Grapes" class="images" />
            </div>
            <div class="image-column">
                <img src="https://th.bing.com/th/id/OIP.Xj9koV7MUUqya0yqIJWkPgHaFk?rs=1&pid=ImgDetMain" alt="Grapes" class="images" />
            </div>
        </div>
    {:else if currentTab === "Projects"}
        <div class="image-container">
            <div class="image-column">
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
                <ImageGallery 
                ImageSource="/Images/supper_froggy.png"/>
            </div>
            <div class="image-column">
                <img src="/Images/arch.png" alt="Grapes" class="images" />
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
            </div>
            <div class="image-column">
                <img src="/Images/painting.jpg" alt="Grapes" class="images" />
            </div>
            <div class="image-column">
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
            </div>
        </div>
    {/if}
</div>

<style>
    .tabs {
        display: flex;
        justify-content: center;
        margin-bottom: 20px;
    }

    .tab-button {
        display: inline-block;
        color: white;
        background-color: var(--blue);
        border-radius: var(--radius);
        padding-left: 20px;
        padding-right: 20px;
        padding-top: 15px;
        padding-bottom: 15px;
        transition: all var(--time) ease;
        text-decoration: none;
        font-size: 20px;
        text-transform: uppercase;
        margin-left: 20px;
        margin-right: 20px;
        border: none;
    }
    .tab-button:hover {
        cursor: pointer;
        transform: scale(var(--scale));
        margin-left: 20px;
        margin-right: 20px;
        filter: brightness(var(--hover-brightness));
    }
    .tab-button:active {
        transform: scale(var(--scale));
        margin-left: 20px;
        margin-right: 20px;
        filter: brightness(var(--hover-brightness));
    }
    .tab-content {
        border: 1px solid #ccc;
        padding: 16px;
    }
    .images {
        width: 100%;
        height: 100%;
        border-radius: var(--radius);
    }
    .image-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: flex-start;
        width: 75%;
        margin: 0 auto;
        align-items: flex-start;
        padding-top: 150px;
        background-color: var(--pale-blue-dark);
        border-radius: var(--radius);
    }
    .image-column {
        display: flex;
        flex-direction: column;
        width: 23%;
        margin-left: 1%;
        margin-right: 1%;
    }
</style>
