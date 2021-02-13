<template>
  <v-container fluid>
    <div class="d-flex flex-column flex-grow-1">
      <v-row no-gutters>
              <v-col cols="12" sm="3">
                  <img class="py-1" src="https://placehold.jp/234x234.png">
                  <div class="ml-5"><h3>味噌汁最中 赤みそ</h3></div>
                  <p class="ml-10">ic000180</p>
              </v-col>      
          <v-col cols="12" sm="9">
            <div class="d-flex align-center py-0">
              <div>
                <div class="display-1">基本情報</div>
              </div>
              <v-spacer></v-spacer>
              <v-btn
                depressed
                color="#00E5FF"
                shaped
                class="ma-1"
                to="/owner/item/basic"
              >
                <span class="shyousai">基本情報</span>
              </v-btn>
              <v-btn
                depressed
                color="#00E5FF"
                shaped
                to="/owner/item/details"
              >
                <span class="shyousai">詳細</span>
              </v-btn>
              <v-btn
                depressed
                color="#00E5FF"
                shaped
                class="ma-1"
              >
              <span class="shyousai">サムネイル</span>
              </v-btn>
              </div>
            <v-card>
                <v-row>
                   <v-col cols="12" sm="9">  
                        <v-dialog v-model="dialog" width="600px">
                            <template v-slot:activator="{ on, attrs }">
                                <img 
                                    class="ml-3"
                                    v-bind="attrs"
                                    v-on="on" 
                                    src="https://placehold.jp/133x133.png"
                                >  
                            </template>
                            <img src="https://placehold.jp/133x133.png">
                        </v-dialog>
                        <v-dialog v-model="dialog">
                            <template v-slot:activator="{ on, attrs }">
                                <img 
                                    class="ml-3"
                                    v-bind="attrs"
                                    v-on="on" 
                                    src="https://placehold.jp/133x133.png"
                                >  
                            </template>
                        </v-dialog>
                    </v-col>
                </v-row>
            </v-card>
          </v-col>
        </v-row>  
    </div>  
  </v-container>    
</template>


<script>
export default {
  data () {
    return {
        dialog:false
    }
  },
  components: {
  },
  layout:"owner"
}
</script>


<style>
.shyousai{
  color: #FFFFFF;
}
.jyouhou{
    border-bottom: 0 !important;
}
</style>