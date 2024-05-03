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
{/if}

<style>
    .image-container{
        background-color: var(--pale-purple-light);
        border-radius: 30px;
        padding: 15px;
        width: auto;
    }
    .button-container {
        background-color: var(--purple-hover);
        border-radius: var(--radius);
        margin-top: 30px;
    }
    .popup {
        position: fixed;
        top: 0;
        left: 0;
        width: 50%;
        height: 50%;
        background: rgba(0, 0, 0, 0.5);
        display: flex;
        justify-content: center;
        align-items: center;
        padding-left: 25%;
        padding-right: 25%;
        padding-top: 15%;
        padding-bottom: 15%;
        z-index: 5;
    }

    .popup-content {
      background: var(--pale-purple-dark);
      padding: 20px;
      border-radius: var(--radius);
      color: white;
    }
    .button {
        background-color: var(--purple);
        border: none;
        border-radius: var(--radius);
        height: 24px;
        color: white;
        transition: all var(--time) ease;
        display: flex;
        justify-content: center;
        font-size: 16px;
        line-height: 24px;
    }
    .button:hover {
        background-color: var(--purple-hover);
        transform: scale(var(--scale));
    }
    .close {
        background-color: var(--purple-hover);
        border: none;
        border-radius: var(--radius);
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
