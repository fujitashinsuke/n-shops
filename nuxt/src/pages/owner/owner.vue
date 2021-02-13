<template>
  <div class="d-flex flex-column flex-grow-1">
    <div class="d-flex align-center py-1">
      <div>
        <div class="display-1">お知らせ</div>
      </div>
      <v-spacer></v-spacer>
        <v-btn-toggle
                rounded
                tile
                dense
                shaped
            >
            <v-btn plain text> 
                未読
            </v-btn>
            <v-btn plain text>
                既読
            </v-btn>
            </v-btn-toggle>
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
      <v-row no-gutters>
        <v-col>
          <v-simple-table  
                class="table"
                fixed-header 
                height="400px"
          >
            <template v-slot:default>
                <thead>
                    <tr>
                      <th class="text-left">件名</th>
                      <th class="text-left">本文</th>
                      <th class="text-left">日時</th>
                      <th class="text-right"></th>
                    </tr>
                </thead>
                    <tbody>
                      <tr v-for="item in oshirase" :key="item.name">
                        <td>
                          <v-icon color="#FFEB3B">
                            mdi-alert
                          </v-icon>
                            {{ item.name }}
                        </td>
                          <td class="text-left">{{ item.honbun }}</td>
                          <td class="text-left">{{ item.date }}</td>
                          <td class="text-right">
                            <v-btn
                              depressed
                              color="#00E5FF"
                              shaped
                              width="180px"
                              height="40px"
                              to="/owner/itemshinsei/list"
                            >
                            <span class="shyousai">詳細表示</span>
                            </v-btn>
                          </td>
                      </tr>
                    </tbody>
              </template>
          </v-simple-table>
        </v-col>
      </v-row>   
    </div>
</template>

<script>
export default {
    layout:"owner",
  data () {
    return {
      oshirase: [
        {
            name: 'アイテム申請がありました',
            honbun: '【道具＆籠目つなぎ】の申請がありました ご確認ください',
            date:"2002-09-18"
          },
          {
            name: 'アイテム申請がありました',
            honbun: '【道具＆籠目つなぎ】の申請がありました ご確認ください',
            date:"2012-09-18"
          },
          {
            name: 'アイテム申請がありました',
            honbun: '【道具＆籠目つなぎ】の申請がありました ご確認ください',
            date:"2002-09-18"
          },
          {
            name: 'アイテム申請がありました',
            honbun: '【道具＆籠目つなぎ】の申請がありました ご確認ください',
            date:"2002-09-18"
          },
          {
            name: 'アイテム申請がありました',
            honbun: '【道具＆籠目つなぎ】の申請がありました ご確認ください',
            date:"2001-09-18"
          },
          {
            name: 'アイテム申請がありました',
            honbun: '【道具＆籠目つなぎ】の申請がありました ご確認ください',
            date:"2090-09-18"
          },
          {
            name: 'アイテム申請がありました',
            honbun: '【道具＆籠目つなぎ】の申請がありました ご確認ください',
            date:"2099-09-18"
          },
          {
            name: 'アイテム申請がありました',
            honbun: '【道具＆籠目つなぎ】の申請がありました ご確認ください',
            date:"1119-09-18"
          },
          {
            name: 'アイテム申請がありました',
            honbun: '【道具＆籠目つなぎ】の申請がありました ご確認ください',
            date:"2009-09-18"
          },
          {
            name: 'アイテム申請がありました',
            honbun: '【道具＆籠目つなぎ】の申請がありました ご確認ください',
            date:"2039-09-18"
          },
      ]
    }
  }
}
</script>

<style>
.shyousai{
  color: white;
}
</style>