<template>
  <div class="d-flex flex-column flex-grow-1">
    <div class="d-flex align-center py-1">
      <div>
        <div class="display-1">パートナー企業</div>
      </div>
      <v-spacer></v-spacer>
            <v-btn depressed class="ma-1">
              <v-icon color="#18FFFF">
                mdi-plus
              </v-icon>  
              新規作成
            </v-btn>
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
        </div>  
        <v-simple-table  
            class="table"
      >
        <template v-slot:default>
            <thead>
                <tr>
                  <th class="text-left">パートナー企業ID</th>
                  <th class="text-left">パートナー企業名</th>
                  <th class="text-left">電話</th>
                  <th class="text-left">メール</th>
                  <th class="text-left">担当者名</th>
                  <th class="text-left"></th>
                </tr>
            </thead>
                <tbody>
                  <tr v-for="item in partner" :key="item.name">
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
                      <td class="text-left">{{ item.kigyou }}</td>
                      <td class="text-left">{{ item.denwa}}</td>
                      <td class="text-left">{{ item.mail }}</td>
                      <td class="text-left">{{ item.tantou }}</td>
                      <td class="text-left">
                        <v-btn
                          depressed
                          color="#00E5FF"
                          shaped
                          to="/owner/partner/detail"
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
      partner: [
        {
            id: '0012345678910',
            kigyou: '藤田工業',
            denwa: '090-9999-1111',
            mail: 'fujita@datumworks.jp',
            tantou:'藤田'
          },
          {
            id: '0012345678910',
            kigyou: '有田工業',
            denwa: '090-9999-1111',
            mail: 'fffkkkk@gmail.com',
            tantou:'有田'
          },
          {
            id: '0012345678910',
            kigyou: 'asfe',
            denwa: '090-9999-1111',
            mail: 'fffksawf@gmail.com',
            tantou:'小野'
          },
          {
            id: '0012345678910',
            kigyou: '株式会社瓶屋',
            denwa: '090-9999-1111',
            mail: 'fflll@gmail.com',
            tantou:'島田'
          },
          {
            id: '0012345678910',
            kigyou:"株式会社ベストモーション",
            denwa: '090-9999-1123',
            mail: 'fffkkkk@gmail.com',
            tantou:'藤田'
          },
          {
            id: '0012345678910',
            kigyou:"株式会社ベストモーション",
            denwa: '090-9999-1234',
            mail: 'fffkkkk@gmail.com',
            tantou:'長谷川'
          },
          {
            id: '0012345678910',
            kigyou:"株式会社 新保哲也アトリエ",
            denwa: '090-9999-1987',
            mail: 'filews@gmail.com',
            tantou:'森、藤波'
          },
          {
            id: '0012345678910',
            kigyou:"株式会社 新保哲也アトリエ",
            denwa: '090-9999-2378',
            mail: 'fffkkkk@gmail.com',
            tantou:'森、藤波'
          },
          {
            id: '0012345678910',
            kigyou: 'asfe',
            denwa: '090-9999-1111',
            mail: 'fffkkkk@gmail.com',
            tantou:'	加藤、浜田、酒井'
          },
          {
            id: '0012345678910',
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


<style>
.shyousai{
  color: #FFFFFF;
}
</style>