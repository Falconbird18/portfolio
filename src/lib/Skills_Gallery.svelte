<script>
    import ImageGallery from "$lib/Image_Gallery.svelte";
</script>

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
<style>
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