<template>
  <div class="d-flex flex-column flex-grow-1">
    <div class="d-flex align-center py-1">
      <div>
        <div class="display-1">アイテム一覧</div>
      </div>
      <v-spacer></v-spacer>
            <v-btn
                class="ma-1"
                rounded   
                depressed
                to="/owner/item/setitem"
            >
            <v-icon color="#18FFFF">
                mdi-plus
            </v-icon>
                セットアイテム新規登録
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
                  <th class="text-left">商品ID</th>
                  <th class="text-left">商品名</th>
                  <th class="text-right">販売価格(税抜き)</th>
                  <th class="text-right">下代価格(税抜き)</th>
                  <th class="text-left">パートナー</th>
                  <th class="text-right"></th>
                </tr>
            </thead>
                <tbody>
                  <tr v-for="item in item" :key="item.name">
                    <td class="text-left">
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
                      <td class="text-right">{{ item.price}}</td>
                      <td class="text-right">{{ item.gedai }}</td>
                      <td class="text-left">{{ item.partner }}</td>
                      <td class="text-right">
                        <v-btn
                          depressed
                          color="#00E5FF"
                          shaped
                          to="/owner/item/basic"
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
      item: [
        {
            id: '00',
            name: '味噌汁最中 赤みそ',
            price: '350円',
            gedai: "210円",
            partner:'株式会社オオトモ'
          },
          {
            id: '01',
            name: '味噌汁最中 白みそ',
            price: '1200円',
            gedai: "210円",
            partner:'株式会社オオトモ'
          },
          {
            id: '02',
            name: '	胡蝶 桃 / / 削り節×6 + スープ×2 + ふりかけ×5',
            price: '1000円',
            gedai: "350円",
            partner:'株式会社オオトモ'
          },
          {
            id: '03',
            name: '胡蝶 朱金 / 削り節×6 + スープ×2 + ふりかけ×5',
            price: '800円',
            gedai: "220円",
            partner:'株式会社オオトモ'
          },
          {
            id: '04',
            name: '祝 竹オレンジ / 削り節×10',
            price: '1000円',
            gedai: "310円",
            partner:'株式会社まるじょう'
          },
          {
            id: '05',
            name: 'smile 白 / 醤油 + 削り節2種×2 + ふりかけ + スープ×2',
            price: '3500円',
            gedai: "230円",
            partner:'株式会社まるじょう'
          },
          {
            id: '06',
            name: 'HAPPY smile 白 / ポン酢醤油 + 削り節2種×2 + ふりかけ + スープ×2',
            price: '1200円',
            gedai: "410円",
            partner:'株式会社まるじょう'
          },
          {
            id: '07',
            name: 'ありがとう smile 白 / だし + 削り節2種×2 + ふりかけ + スープ',
            price: '800円',
            gedai: "350円",
            partner:'株式会社まるじょう'
          },
          {
            id: '08',
            name: '祝 白 / 削り節×10',
            price: '1500円',
            gedai: "320円",
            partner:'株式会社まるじょう'
          },
          {
            id: '09',
            name: '祝 白 / 削り節×10',
            price: '1000円',
            gedai: "120円",
            partner:'株式会社オオトモ'
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
