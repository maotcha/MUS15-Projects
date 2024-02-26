<script>
    import { goto } from '$app/navigation';
    import { onMount } from 'svelte';
    
    function redirect(select) {
        goto("/" + select.options[select.selectedIndex].value);
    }

    onMount(() => {
        let selectStyle = document.getElementById("styleSelect");
        
        if (selectStyle != null) {
            selectStyle.addEventListener("change",function(){redirect(selectStyle);})
        }
        
    });

</script>
<style>
    .main {
        display: flex;
        background-color: #3d3f52;
        width: 100%;
        height: 70px;
        border-bottom: solid;
        border-bottom-width: 1px;
        border-color: black;
        place-items: end
        
    }

    select {
        margin-left: 10px;
        margin-bottom: 8px;
        background-color: #a9a9b0;
        height: 30%;
        
    }

</style>
<div class="main">
    
    <select id="styleSelect">
        <option value="" selected>Select a Website Style</option>
        <option value="personal">Personal</option>
        <option value="professional">Professional</option>
    </select>
</div>