<template>
    <div class="layout">
        <div class="cell a"><p>a</p></div>
        <div class="cell b"><p>b</p></div>
        <div class="cell c"><p>c</p></div>
        <div class="cell d"><p>d</p></div>
        <div class="cell e"><p>e</p></div>
        <div class="cell f"><p>f</p></div>
        <div class="cell g"><p>g</p></div>
        <div class="cell h"><p>h</p></div>
        <div class="cell i"><p>i</p></div>
        <div class="cell j"><p>j</p></div>
        <div class="cell k"><p>k</p></div>

        <md-tabs md-sync-route>
            <md-tab id="tab-home" md-label="Home" to="/components/tabs/home"></md-tab>
            <md-tab id="tab-pages" md-label="Pages" to="/components/tabs/pages"></md-tab>
            <md-tab id="tab-posts" md-label="Posts" to="/components/tabs/posts"></md-tab>
            <md-tab id="tab-settings" md-label="Settings" to="/components/tabs/settings"></md-tab>
            <md-tab id="tab-disabled" md-label="Disabled" md-disabled></md-tab>
        </md-tabs>

    </div>
  
</template>

<script>
export default {
  
}
</script>


<style scoped>
.layout{
    background: aliceblue;
    display: grid;
    grid-gap: 2px;
    grid-template-columns: repeat(5,1fr);
    grid-template-rows: repeat(3,1fr);

}

.cell{
    background-color:black;
    border-radius: 3px;
    color: #ffffff;
    padding: 20px;
    font-size: 40px;
}

.h{
    grid-column-start:2;
    grid-column-end: 4;
    grid-row-end: 2;
    grid-row-start: 1;
    background: olive;
}

.d{
    background:lightsalmon;
    grid-column: 3 /2;
    grid-row: 2 / 5
}

.b{
    grid-column: 1 / 2;
    grid-row: 2/4;
    background-color: maroon;
}



</style>
