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
                to="/owner/item/samuneiru"
              >
              <span class="shyousai">サムネイル</span>
              </v-btn>
              </div>
              <v-card>
                <br>
                <br>  
              <v-btn
                class="ml-2"
                rounded
                depressed
                height="22px"
                color= "#B2EBF2"  
              >
                <span class="name">サイズ</span>
              </v-btn>
              <v-row>
                <v-col cols="12" sm="6">
                  <v-simple-table>
                    <template v-slot:default>
                      <tbody>
                        <tr class="jyouhou">
                          <td><h4>幅(cm)</h4></td>
                          <td><span class="mr-12">8</span></td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>奥行き(cm)</h4></td>
                          <td>6.5</td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>高さ(cm)</h4></td>
                          <td>6.5</td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td></td>
                          <td></td>                  
                        </tr>
                      </tbody>
                    </template>
                  </v-simple-table>  
                </v-col>
                <v-col cols="12" sm="6">
                  <v-simple-table>
                    <template v-slot:default>
                      <tbody>
                        <tr class="jyouhou">
                          <td><h4>重さ(g)</h4></td>
                          <td><span class="mr-12"></span></td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>熨斗対応可否</h4></td>
                          <td>不可</td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td></td>
                          <td></td>                  
                        </tr>  
                      </tbody>
                    </template>
                  </v-simple-table>  
                </v-col>
              </v-row>  
              <v-btn
                class="ml-2"
                rounded
                depressed
                height="22px"
                color= "#B2EBF2"  
              >
                <span>パートナー企業情報</span>
              </v-btn>
              <v-row>
                <v-col cols="12" sm="6">
                  <v-simple-table>
                    <template v-slot:default>
                    </template>
                  </v-simple-table>  
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
    return {}
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
