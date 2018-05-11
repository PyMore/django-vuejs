<template>
    <div>
        <md-toolbar class="md-large md-primary">
            <div class="md-toolbar-row">

               <div class="md-toolbar-row md-toolbar-offset">
                    <h3 class="md-title">Are you ready?</h3>
                </div>

                <div class="md-toolbar-section-end">
                    <md-button class="md-icon-button">
                        <md-icon>more_vert</md-icon>
                    </md-button>
                </div>

            </div>

        </md-toolbar>        

        <md-tabs class="md-primary" md-alignment="fixed">
            <md-tab id="tab-home" md-icon="home">
            </md-tab>
            <md-tab id="tab-pages" md-icon="pages">
            </md-tab>
            <md-tab id="tab-favorites" md-icon="favorite"></md-tab>
            <md-tab id="tab-favorites4" md-icon="favorite"></md-tab>

        </md-tabs>


    <div class="section">
    <md-card>
      <md-card-header>
        <div class="md-title">Card without hover effect</div>
      </md-card-header>

      <md-card-content>
        <form action="">
            
            <md-datepicker v-model="selectedDate" />
            </md-field>

            <md-field>
            <label>Hours</label>
            <md-input v-model="number" type="number"></md-input>
            </md-field>

            <md-field>
            <label>Comment</label>
            <md-textarea v-model="autogrow" md-autogrow></md-textarea>
            </md-field>


            <div class="md-layout-item">
                <md-field>
                <label for="font">Font</label>
                <md-select v-model="font" name="font" id="font" md-dense>
                    <md-option value="arial">Arial</md-option>
                    <md-option value="calibri">Calibri</md-option>
                    <md-option value="cambria">Cambria</md-option>
                    <md-option value="comic-sans">Comic Sans</md-option>
                    <md-option value="consolas">Consolas</md-option>
                    <md-option value="courier">Courier</md-option>
                    <md-option value="droid-sans">Droid Sans</md-option>
                    <md-option value="georgia">Georgia</md-option>
                    <md-option value="helvetica">Helvetica</md-option>
                    <md-option value="impact">Impact</md-option>
                    <md-option value="roboto">Roboto</md-option>
                    <md-option value="segoe-ui">Segoe UI</md-option>
                    <md-option value="times-new-roman">Times New Roman</md-option>
                    <md-option value="ubuntu">Ubuntu</md-option>
                    <md-option value="verdana">Verdana</md-option>
                </md-select>
                </md-field>
            </div>


            <md-button type="submit" class="md-primary md-raised">Open Snackbar</md-button>

        </form>        
      </md-card-content>

    </md-card>

    </div>



    </div>
</template>

<script>
    
</script>


<style  scoped>
    md-toolbar{
        background-color: blue;
    }


  .section {
    margin-top: 3em;
    margin-left: 25%;
    max-width: 50%;
  }
</style>
