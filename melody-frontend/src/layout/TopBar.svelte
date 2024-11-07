<script>
    import newInstanceIcon from "../assets/icons/new_instance.svg"
    import settingsIcon from "../assets/icons/settings.svg"
    import helpIcon from "../assets/icons/help.svg"
    import updateIcon from "../assets/icons/update.svg"

	import IconButton from "../components/IconButton.svelte";
</script>

<div class="top-bar">
    <IconButton iconPath={newInstanceIcon} text="New Instance" />
    <IconButton iconPath={settingsIcon} text="Settings" />
    <IconButton iconPath={helpIcon} text="Help" />
    <IconButton iconPath={updateIcon} text="Update" />
</div>


<style>
    .top-bar {
        display: flex;
        flex-direction: row;
        align-items: center;
        background-color: var(--item-color);
        gap: 8px;
        padding-top: 8px;
        padding-bottom: 8px;
        padding-left: 8px;
        border-bottom: 1px solid var(--border-color)
    }
</style>