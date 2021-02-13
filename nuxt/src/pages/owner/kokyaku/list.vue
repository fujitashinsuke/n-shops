<template>
  <div class="d-flex flex-column flex-grow-1">
    <div class="d-flex align-center py-1">
      <div>
        <div class="display-1">顧客一覧</div>
      </div>
      <v-spacer></v-spacer>
            <v-btn
                class="ma-1"
                rounded   
                depressed
            >
            <v-icon color="#18FFFF">
                mdi-sort-ascending
            </v-icon>
                並べ替え
            </v-btn>
            <v-btn
                rounded
                depressed
                class="ma-1"
            >
            <v-icon color="#18FFFF">
                mdi-filter
            </v-icon>
                絞り込み
            </v-btn>
            <v-btn
                class="ma-1"
                rounded   
                depressed
            >
            <v-icon color="#18FFFF">
                mdi-sort-ascending
            </v-icon>
                エクスポート
            </v-btn>
        </div>  
        <v-simple-table  
            class="table"
      >
        <template v-slot:default>
            <thead>
                <tr>
                  <th class="text-left">顧客ID</th>
                  <th class="text-left">登録者</th>
                  <th class="text-left">名前</th>
                  <th class="text-left">婚姻日</th>
                  <th class="text-left">住所</th>
                  <th class="text-left"></th>
                </tr>
            </thead>
                <tbody>
                  <tr v-for="item in kokyaku" :key="item.name">
                    <td>
                      <v-btn
                        rounded
                        depressed
                        height="22px"
                        color= "#B2EBF2"  
                      >
                        {{ item.id }}
                      </v-btn>  
                    </td>
                      <td class="text-left">{{ item.name }}</td>
                      <td class="text-left">{{ item.firstname}}</td>
                      <td class="text-left">{{ item.date }}</td>
                      <td class="text-left">{{ item.juusyo }}</td>
                      <td class="text-right">
                        <v-btn
                          depressed
                          color="#00E5FF"
                          shaped
                          width="180px"
                          height="40px"
                        >
                        <span class="shyousai">詳細表示</span>
                        </v-btn>
                      </td>
                      
                  </tr>
                </tbody>
          </template>
      </v-simple-table>
  </div>
</template>


<script>
export default {
  data () {
    return {
      kokyaku: [
        {
            id: '00',
            name: '藤田　比呂文',
            firstname: '藤田・伊藤',
            date: "2019/09/19",
            juusyo:'大阪府大阪市生野区2-3-4'
          },
          {
            id: '01',
            name: 'ユニオン 太郎',
            firstname: '山尾・住友',
            date: "2019/09/19",
            juusyo:'大阪府大阪市生野区2-3-4'
          },
          {
            id: '02',
            name: '森山 咲良',
            firstname: '・',
            date: "2019/09/19",
            juusyo:'大阪府大阪市生野区2-3-5'
          },
          {
            id: '03',
            name: 'ロベルト ベッカム',
            firstname: 'ロベ・ダラス',
            date: "2019/09/19",
            juusyo:'大阪府大阪市生野区2-3-4'
          },
          {
            id: '04',
            name: '迫田 紫穂',
            firstname: '田中・迫田',
            date: "2019/09/09",
            juusyo:'大阪府大阪市生野区2-7-4'
          },
          {
            id: '05',
            name: '中川 智子',
            firstname: '中川・中川',
            date: "2019/09/12",
            juusyo:'大阪府大阪市生野区2-3-4'
          },
          {
            id: '06',
            name: '戸田 真人',
            firstname: '戸田・山田',
            date: "2019/09/19",
            juusyo:'大阪府大阪市生野区2-3-4'
          },
          {
            id: '07',
            name: 'ユニオン 太郎',
            firstname: 'ユニオン',
            date: "",
            juusyo:''
          },
          {
            id: '08',
            name: 'ユニオン 太郎cc',
            firstname: 'aaa',
            date: "2019/09/20",
            juusyo:'大阪府大阪市生野区2-3-4'
          },
          {
            id: '09',
            name: 'ユニオン 太郎kk',
            firstname: 'llll',
            date: "",
            juusyo:'大阪府大阪市生野区2-3-4'
          },
      ]
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
</style>