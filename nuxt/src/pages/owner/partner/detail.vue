<template>
  <div class="d-flex flex-column flex-grow-1">
    <div class="d-flex align-center py-1">
      <div>
        <div class="display-1">パートナー企業</div>
      </div>
      <v-spacer></v-spacer>
            <v-btn depressed >
              <v-icon>
                mdi-pencil-outline
              </v-icon>  
            </v-btn>
    </div>   
        <v-card>
            <v-row no-gutters>
                <v-col cols="12" sm="6">
                    <v-simple-table  
                        class="table"
                    >
                        <template v-slot:default>
                                <tbody>
                                 <br>
                                 <br>   
                                <tr>   
                                    <td class="text-left"><h3>パートナー企業名</h3></td>
                                    <td class="text-left">藤田工業</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>パートナー企業ID</h3></td>
                                    <td class="text-left">pa61</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>パートナー企業名（カナ）</h3></td>
                                    <td class="text-left">フジタコウギョウ</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>パートナー企業名(略称)</h3></td>
                                    <td class="text-left">ふじこー</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>郵便番号</h3></td>
                                    <td class="text-left">郵便番号</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>都道府県</h3></td>
                                    <td class="text-left">	大阪府じゆう</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>市町村</h3></td>
                                    <td class="text-left">	大阪市生野区中川</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>番地</h3></td>
                                    <td class="text-left">3-4</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>マンション名</h3></td>
                                    <td class="text-left">	LLマンション</td>
                                </tr>
                                <br>
                                <br>
                                <tr>  
                                    <td class="text-left"><h3>銀行名</h3></td>
                                    <td class="text-left"></td>
                                </tr>
                                <tr>  
                                    <td class="text-left"><h3>支店名</h3></td>
                                    <td class="text-left"></td>
                                </tr>
                                <tr>  
                                    <td class="text-left"><h3>口座種別</h3></td>
                                    <td class="text-left"></td>
                                </tr>
                                <br>
                                <br>
                                </tbody>
                        </template>
                    </v-simple-table>
            </v-col>
                <v-col cols="12" sm="6">
                    <v-simple-table>
                        <template v-slot:default>
                            <tbody>
                                <br>
                                <br>
                                <tr>
                                    <td class="text-left"><h3>電話番号1</h3></td>
                                    <td class="text-left">06-0088-6472</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>電話番号2</h3></td>
                                    <td class="text-left">06-0088-6472</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>電話番号2</h3></td>
                                    <td class="text-left">06-0088-6472</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>メールアドレス</h3></td>
                                    <td class="text-left">fujita@datumworks.jp</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>メールアドレス2</h3></td>
                                    <td class="text-left"></td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>メールアドレス3</h3></td>
                                    <td class="text-left"></td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>担当部署</h3></td>
                                    <td class="text-left">経営企画課</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>担当者</h3></td>
                                    <td class="text-left">長谷川</td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>代表者</h3></td>
                                    <td class="text-left">藤田　てつお</td>
                                </tr>
                                <br>
                                <br>
                                <tr>
                                    <td class="text-left"><h3>口座番号</h3></td>
                                    <td class="text-left"></td>
                                </tr>
                                <tr>
                                    <td class="text-left"><h3>口座名義</h3></td>
                                    <td class="text-left"></td>
                                </tr>
                                <br>
                                <br>
                                <br>
                                
                            </tbody>
                        </template>
                    </v-simple-table>
                </v-col>
             </v-row>  
        </v-card>           
    </div>
</template>


<script>
export default {
  data () {
    return {
      partner: [
        {
            id: '00',
            kigyou: '藤田工業',
            denwa: '090-9999-1111',
            mail: 'fujita@datumworks.jp',
            tantou:'藤田'
          },
          {
            id: '01',
            kigyou: '有田工業',
            denwa: '090-9999-1111',
            mail: 'fffkkkk@gmail.com',
            tantou:'有田'
          },
          {
            id: '02',
            kigyou: 'asfe',
            denwa: '090-9999-1111',
            mail: 'fffksawf@gmail.com',
            tantou:'小野'
          },
          {
            id: '03',
            kigyou: '株式会社瓶屋',
            denwa: '090-9999-1111',
            mail: 'fflll@gmail.com',
            tantou:'島田'
          },
          {
            id: '04',
            kigyou:"株式会社ベストモーション",
            denwa: '090-9999-1123',
            mail: 'fffkkkk@gmail.com',
            tantou:'藤田'
          },
          {
            id: '05',
            kigyou:"株式会社ベストモーション",
            denwa: '090-9999-1234',
            mail: 'fffkkkk@gmail.com',
            tantou:'長谷川'
          },
          {
            id: '06',
            kigyou:"株式会社 新保哲也アトリエ",
            denwa: '090-9999-1987',
            mail: 'filews@gmail.com',
            tantou:'森、藤波'
          },
          {
            id: '07',
            kigyou:"株式会社 新保哲也アトリエ",
            denwa: '090-9999-2378',
            mail: 'fffkkkk@gmail.com',
            tantou:'森、藤波'
          },
          {
            id: '08',
            kigyou: 'asfe',
            denwa: '090-9999-1111',
            mail: 'fffkkkk@gmail.com',
            tantou:'	加藤、浜田、酒井'
          },
          {
            id: '09',
            kigyou:"	Dari K株式会社",
            denwa: '090-9999-1111',
            mail: 'fffkkkk@gmail.com',
            tantou:'	加藤、浜田、酒井'
          },
      ]
    }
  },
  components: {
  },
  layout:"owner"
}
</script>
