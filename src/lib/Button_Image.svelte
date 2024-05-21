<script>
    import { fade } from "svelte/transition";

    export let closeButtonText = "Close";
    export let popupYear = "2008";
    export let buttonImageSource = "/Images/marker.svg";
    export let imageSource = "/Images/baby.svg";
    export let imageAlt = "Architecture";
    export let text = "Architecture";
    export let MarkerText = "2024 Oil Paints";

    let isPopupVisible = false;

    function togglePopup() {
        isPopupVisible = !isPopupVisible;
    }
</script>

<button
    on:click={togglePopup}
    class="button"
>
    <div class="image">
        <img src={buttonImageSource} alt={imageAlt} class="new-image"/>
        <p class="marker-text">{MarkerText}</p>
    </div>
</button>
{#if isPopupVisible}
    <div class="popup" in:fade={{ duration: 300 }} out:fade={{ duration: 300 }}>
        <div
            class="popup-content"
            in:fade={{ duration: 300 }}
            out:fade={{ duration: 300 }}
        >
            <p>{popupYear}</p>
            <div class="container">
                <img src={imageSource} alt={imageAlt} class="image-popup" />
            </div>
            <br />
            <p>{text}</p>
            <button on:click={togglePopup} class="close"
                >{closeButtonText}</button
            >
        </div>
    </div>
{/if}

<style>
    .container {
        background-color: var(--pale-green-light);
        border-radius: 30px;
        padding: 15px;
        width: auto;
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
        background: var(--pale-green-dark);
        padding: 20px;
        border-radius: 30px;
        color: black;
    }
    .button {
        background-color: rgba(0, 0, 0, 0);
        border: none;
        display: flex;
        justify-content: center;
        filter: unset;
        width: 75%;
        transition: all var(--time) ease;
    }
    .button:hover {
        transform: scale(var(--scale));
        filter: brightness(var(--hover-brightness));
    }
    .close {
        background-color: var(--green-hover);
        border: none;
        border-radius: 30px;
        color: white;
        padding: 15px;
        text-transform: uppercase;
        transition: all var(--time) ease;
    }
    .close:hover {
        background-color: var(--green-hover);
        transform: scale(var(--scale));
    }
    .image {
        width: 10%;
        height: auto;
        z-index: 500;
    }
    .new-image{
        width: 100%;
    }
    .image-popup {
        width: 75%;
        height: auto;
    }
    .marker-text {
        font-size: 25px;
        color: #5e666e;
        transform: translate(40px, -160px);
        z-index: 501;
        max-width: 55%;
        justify-content: center;
    }
</style>
