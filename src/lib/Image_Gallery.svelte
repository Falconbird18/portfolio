<script>
    import { fade } from "svelte/transition";

    export let closeButtonText = "Close";
    export let popupYear = "2008";
    export let ImageSource = "/Images/grapes.jpg";
    export let imageAlt = "Architecture";
    export let text = "Architecture";

    let isPopupVisible = false;

    function togglePopup() {
        isPopupVisible = !isPopupVisible;
    }
</script>

    <button on:click={togglePopup} class="button">
    <img src="{ImageSource}" alt="{imageAlt}" class="image">    
    </button
    >
{#if isPopupVisible}
    <div class="popup" in:fade={{ duration: 300 }} out:fade={{ duration: 300 }}>
        <div
            class="popup-content"
            in:fade={{ duration: 300 }}
            out:fade={{ duration: 300 }}
        >
            <p>{popupYear}</p>
            <div class="container">
                <img src={ImageSource} alt={imageAlt} class="image-popup" />
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
        z-index: 501;
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
        width: 100%;
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
    .image{
        width: 100%;
        height: auto;
        z-index: 500;
        border-radius: var(--radius);
    }
    .image-popup{
        width: 75%;
        height: 75%;
    }
</style>
