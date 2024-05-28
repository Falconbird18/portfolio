<script>
    import { fade } from "svelte/transition";

    export let buttonText = "Toggle Popup";
    export let closeButtonText = "Close";
    export let popupText = "Popup";
    export let width = "95%";
    export let imageSource = "/Images/arch.png";
    export let imageAlt = "Architecture";
    export let artworkTitle = "Architecture";

    let isPopupVisible = false;

    function togglePopup() {
        isPopupVisible = !isPopupVisible;
    }
</script>

<div class="button-container">
    <button on:click={togglePopup} class="button" style:width
        >{buttonText}</button
    >
</div>
{#if isPopupVisible}
<div class="darken">
    <div class="popup" in:fade={{ duration: 300 }} out:fade={{ duration: 300 }}>
        <div
            class="popup-content"
            in:fade={{ duration: 300 }}
            out:fade={{ duration: 300 }}
        >
            <p>{popupText}</p>
            <div class="image-container">
                <img src={imageSource} alt={imageAlt} class="image" />
            </div>
            <br />
            <p>title: {artworkTitle}</p>
            <button on:click={togglePopup} class="close"
                >{closeButtonText}</button
            >
        </div>
    </div>
</div>
{/if}

<style>
    .darken{
        position: fixed;
        background-color: rgba(0,0,0,0.5);
        width: 100%;
        height: 100%;
        display: flex;
        top: 0px;
        left: 0px;
        z-index: 6;
    }
    .image-container {
        background-color: var(--pale-purple-light);
        border-radius: 30px;
        padding: 15px;
        width: auto;
    }
    .button-container{
        background-color: var(--purple);
        border-radius: 30px;
        margin-top: 30px;
        filter: brightness(var(--hover-brightness));
    }
    .popup {
        position: fixed;
        display: flex;
        justify-content: center;
        align-items: center;
        padding-left: 25%;
        padding-right: 25%;
        padding-top: 15%;
        padding-bottom: 15%;
        z-index: 5;
        transform: scale(0.75,0.75);
    }

    .popup-content {
        background: var(--pale-purple-dark);
        padding: 20px;
        border-radius: 30px;
        color: white;
    }
    .button {
        text-transform: uppercase;
        background-color: var(--purple);
        border: none;
        border-radius: 30px;
        height: 24px;
        color: white;
        transition: all var(--time) ease;
        display: flex;
        justify-content: center;
        font-size: 16px;
        line-height: 24px;
        filter: none;
        z-index: 4;
    }
    .button:hover {
        transform: scale(var(--scale));
        filter: brightness(var(--hover-brightness));
    }
    .close {
        background-color: var(--purple-hover);
        border: none;
        border-radius: 30px;
        color: white;
        padding: 15px;
        text-transform: uppercase;
        transition: all var(--time) ease;
    }
    .close:hover {
        background-color: var(--purple-hover);
        transform: scale(var(--scale));
    }
    .image {
        width: 75%;
        height: auto;
        padding: 20px;
        border-radius: 30px;
    }
</style>
