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
    <p class="icon-button-text">{text}</p>
</div>

<style>
    .icon-button {
        display: flex;
        flex-direction: row;
        align-items: center;

        border: 1px solid red;
    }

    .icon-button-img {
        width: 48px;
        height: 48px;
        margin-right: 16px;
    }

    .icon-button-text {
        font-size: 24px;
    }
</style>