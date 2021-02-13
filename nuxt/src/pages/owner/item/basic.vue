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
                rounded
                depressed
                height="22px"
                class="ml-2"
                color= "#B2EBF2"  
              >
                <span class="name">アイテムカテゴリ</span>
              </v-btn>
              <br>
              <br>
              <v-btn
                class="ml-2"
                rounded
                depressed
                height="22px"
                color= "#B2EBF2"  
              >
                <span class="name">アイテムタグ</span>
              </v-btn>
              <br>
              <br>
             <span class="ml-2">#お味噌汁</span>
             <br>
             <br>
              <v-btn
                class="ml-2"
                rounded
                depressed
                height="22px"
                color= "#B2EBF2"  
              >
                <span class="name">価格・在庫</span>
              </v-btn>
              <v-row>
                <v-col cols="12" sm="6">
                  <v-simple-table>
                    <template v-slot:default>
                      <tbody>
                        <tr class="jyouhou">
                          <td><h4>販売価格(税抜)</h4></td>
                          <td><span class="mr-12">350円</span></td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>下代価格(税抜)</h4></td>
                          <td>210円</td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>卸掛率</h4></td>
                          <td>60%</td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>有効期限(開始日)</h4></td>
                          <td>2019/09/01</td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>有効期限(終了日)</h4></td>
                          <td>2999/12/31</td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>申込期日</h4></td>
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
                          <td><h4>キャンセル期日</h4></td>
                          <td></td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>最小ロット数</h4></td>
                          <td>1</td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>在庫アラート数</h4></td>
                          <td>残り0個になったらアラート</td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>数量</h4></td>
                          <td>非表示にする</td>                  
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
                      <tbody>
                        <tr class="jyouhou">
                          <td><h4>取扱パートナー企業名</h4></td>
                          <td><span class="mr-9">株式会社オオトモ</span></td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>取扱パートナー企業CD</h4></td>
                          <td>pa</td>                  
                        </tr>
                        <tr class="jyouhou">              
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
                          <td><h4>パートナー商品名</h4></td>
                          <td><span class="mr-9">味噌汁最中（赤みそ）</span></td>                  
                        </tr>
                        <tr class="jyouhou">
                          <td><h4>パートナー管理ID</h4></td>
                          <td></td>                  
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
