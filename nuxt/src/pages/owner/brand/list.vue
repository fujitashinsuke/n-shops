<template>
  <div class="d-flex flex-column flex-grow-1">
    <div class="d-flex align-center py-1">
      <div>
        <div class="display-1">ブランド</div>
      </div>
      <v-spacer></v-spacer>
            <v-btn depressed class="ma-1">
              <v-icon color="#18FFFF">
                mdi-plus
              </v-icon>  
              新
            </v-btn>
        </div>  
        <v-simple-table>
        <template v-slot:default>
            <thead>
                <tr>
                  <th>ブランドID</th>
                  <th class="text-left">ブランド名</th>
                  <th class="text-right"></th>
                  <th class="text-left"></th>
                  <th class="text-right"></th>
                  <th class="text-right"></th>
                  <th class="text-right"></th>
                  <th class="text-right"></th>
                  <th class="text-right"></th>
                  <th class="text-right"></th>
                  <th class="text-right"></th>
                  <th class="text-right"></th>
                  <th class="text-right"></th>
                  <th class="text-right"></th>
                  <th class="text-right"></th>
                  <th class="text-right"></th>
                </tr>
            </thead>
                <tbody>
                  <tr v-for="item in brand" :key="item.name">
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
                      <td class="text-right">
                      </td>
                      <td class="text-right">
                      </td>
                      <td class="text-right">
                      </td>
                      <td class="text-right">
                      </td>
                      <td class="text-right">
                      </td>
                      <td class="text-right">
                      </td>
                      <td class="text-right">  
                      </td>
                      <td class="text-right">                       
                      </td>
                      <td class="text-right">                       
                      </td>
                      <td class="text-right">                       
                      </td>
                      <td class="text-right">   
                      </td>
                      <td class="text-right">
                      </td>
                      <td class="text-right">
                        <img :src="item.src">
                      </td>
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
      brand: [
        {
            id: '00',
            name: 'NINAS / ニナス',
            src: 'https://placehold.jp/80x80.png'
          },
          {
            id: '01',
            name: 'The Laundress / ザ･ランドレス',
            src: 'https://placehold.jp/80x80.png'
          },
          {
            id: '02',
            name: '	WEDGWOOD / ウェッジウッド',
            src: 'https://placehold.jp/80x80.png'
          },
          {
            id: '03',
            name: '	アマレーナ',
            src: 'https://placehold.jp/80x80.png'
          },
          {
            id: '04',
            name:"ワッフル・ケーキの店 エール・エル",
            src: 'https://placehold.jp/80x80.png'
          },
          {
            id: '05',
            name:	'グランマーブル',
            src: 'https://placehold.jp/80x80.png'
          },
          {
            id: '06',
            name:'パティスリーサンファソン',
            src: 'https://placehold.jp/80x80.png'
          },
          {
            id: '07',
            name:'john masters organics / ジョンマスターオーガニック',
            src: 'https://placehold.jp/80x80.png'
          },
          {
            id: '08',
            name: '	Dari K / ダリケー',
            src: 'https://placehold.jp/80x80.png'
          },
          {
            id: '09',
            name: 'TENERITA / テネリータ',
            src: 'https://placehold.jp/80x80.png'
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