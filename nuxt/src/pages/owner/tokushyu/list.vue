<template>
  <div class="d-flex flex-column flex-grow-1">
    <div class="d-flex align-center py-1">
      <div>
        <div class="display-1">特集</div>
      </div>
      <v-spacer></v-spacer>
            <v-btn depressed>
              <v-icon color="#18FFFF">
                mdi-plus
              </v-icon>  
              新規作成
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
            <v-card>
        <v-container fluid>
          <v-row dense>
            <v-col
              v-for="card in cards"
              :key="card.title"
              cols="3"
            >
              <v-card>
                <v-img
                  :src="card.src"
                  class="white--text align-end"
                  max-height="503"
                >
                  <v-card-title v-text="card.title"></v-card-title>
                  <v-card-subtitle class="white--text align-end" v-text="card.subtitle"></v-card-subtitle>
                </v-img>
              </v-card>
            </v-col>
          </v-row>
        </v-container>
      </v-card>
  </div>
</template>

<script>
export default {
    data: () => ({
    cards: [
      { title: 'オープン記念!今なら1配送先当たり税抜3,000円以上購入で送料無料♪', src: 'https://placehold.jp/336x336.png',subtitle:'公開日 2019.08.13 - 2019.09.23'},
      { title: 'パーツ参考', src: 'https://placehold.jp/336x336.png',subtitle:'公開日 2019.08.13 - 2019.09.23'},
      { title: '大切な人へこだわりのギフトを 引き出物・引き菓子専門店 オクターブ', src: 'https://placehold.jp/336x153.png',subtitle:'公開日 2019.08.13 - 2019.09.23'},
      { title: '全商品から自由に組み合わせ可能！ふたりだけのギフトセットを贈ろう', src: 'https://placehold.jp/336x336.png', subtitle:'公開日 2019.08.13 - 2019.09.23'},
      { title: '手作りにこだわる京都有名デニッシュ店「グランマーブル」人気の秘密', src: 'https://placehold.jp/336x503.png', subtitle:'公開日 2019.08.13 - 2019.09.23'},
      { title: 'オクターブのタクヒキ(宅配引き出物)', src: 'https://placehold.jp/336x336.png', subtitle:'公開日 2019.08.13 - 2019.09.23'},
      { title: '神戸発のワッフルケーキ専門店「R.L(エール・エル)」', src: 'https://placehold.jp/336x503.png', subtitle:'公開日 2019.08.13 - 2019.09.23'},
      { title: '兵庫県宝塚市の「洋菓子工房　華菓」', src: 'https://placehold.jp/336x336.png', subtitle:'公開日 2019.08.13 - 2019.09.23'},
    ]
  }),
  components: {
  },
  layout:"owner"
}
</script>
