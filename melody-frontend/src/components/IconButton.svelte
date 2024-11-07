<script lang="ts">
    type Props = {
        iconPath: string
        text: string
    }

    let { iconPath, text }: Props = $props();
</script>

<!-- svelte-ignore a11y_missing_attribute -->
<div class="icon-button">
    <img class="icon-button-img" src={iconPath}>
    <div class="icon-button-text-container">
        <p class="icon-button-text">{text}</p>
    </div>
</div>

<style>
    .icon-button {
        width: 160px;
        display: flex;
        flex-direction: row;
        background-color: var(--background-color);
        align-items: center;
        user-select: none;
        border: 1px solid var(--border-color);
        border-radius: 4px;
        padding-left: 4px;
        padding-right: 4px;
    }

    .icon-button:active {
        scale: 0.975;
    }

    .icon-button-img {
        width: 32px;
        height: 32px;
    }

    .icon-button-text {
        font-size: 18px;
        margin-right: 6px;
        margin-top: 6px;
        margin-bottom: 6px;
    }

    .icon-button-text-container {
        display: flex;
        flex-direction: row;
        width: 100%;
        justify-content: center;
    }
</style>