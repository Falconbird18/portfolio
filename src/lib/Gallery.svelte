<script>
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
        <div class="image-container">
            <div class="image-column">
                <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
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
        <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
    {:else if currentTab === "Inkscape"}
        <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
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
        <img src="/Images/grapes.jpg" alt="Grapes" class="images" />
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
        margin: 10px;
        border-radius: var(--radius);
    }
    .image-container {
        display: flex;
        flex-wrap: wrap;
        justify-content: flex-start;
        width: 75%;
        margin: 0 auto;
        align-items: flex-start;
    }
    .image-column {
        display: flex;
        flex-direction: column;
        width: 23%;
        margin-left: 1%;
        margin-right: 1%;
        gap: 10px;
    }
</style>
