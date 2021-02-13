<template>
  <v-container>
    <div class="d-flex flex-column flex-grow-1">
          <div class="d-flex align-center py-1">
              <div>
                  <div class="display-1">セットアイテム登録</div>
              </div>
          </div>
      <v-simple-table>
                    <template v-slot:default>
                      <tbody>
                        <tr class="jyouhou">
                          <td><h4>販売価格(税抜)</h4></td>
                          <td><span class="ml-1">350円</span></td>                  
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
    </div>
  </v-container>  
</template>

<script>
export default {
    data: () => ({
  }),
  components: {
  },
  layout:"owner"
}
</script>
