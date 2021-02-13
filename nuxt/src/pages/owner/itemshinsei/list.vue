<template>
  <div class="d-flex flex-column flex-grow-1">
    <div class="d-flex align-center py-0">
      <div>
        <div class="display-1">アイテム申請</div>
      </div>
      <v-spacer></v-spacer>
            <div class="kensaku">
                <v-text-field
                    prepend-inner-icon="mdi-magnify"
                    label="商談アイテム確認"
                    placeholder="商談アイテム確認"
                    solo
                    flat
                    outlined
                    dense
                >
                </v-text-field>
            </div>
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
      <v-card>
      <v-container fluid>
        <v-alert
          border="left"
          color="red darken-1"
          outlined
          colored-border
        >
          <v-expansion-panels  flat>
                <v-expansion-panel>
                <v-expansion-panel-header>
                            <v-row no-gutters>
                                <v-col cols="12" sm="6">
                                  <h4>申請日時：2021年01月27日 17:52:14　SHIN-CYA-KI KYU-SU HITORI（IVORY）</h4>
                                </v-col>
                            </v-row>
                            <v-row
                                no-gutters
                            >
                            <v-col cols="12" sm="6">
                              <h4>(株式会社アールピースファクトリー)</h4>
                            </v-col>  
                            </v-row>                  
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                    <v-row no-gutters>
                        <v-col cols="3">
                            <img src="https://placehold.jp/234x234.png">
                            <v-row justify="center">
                      <v-col cols="6">
                        <v-btn
                          small
                          shaped
                          outlined
                          depressed
                        >
                        <v-icon>mdi-pencil-outline</v-icon>
                        </v-btn>
                      </v-col>
                    </v-row>                    
                        </v-col>
                        <v-col cols="5">
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                              <span class="name">ブランド名</span>
                            </v-btn>  
                            <br>
                            <br>
                            AR Piece
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">価格・在庫</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>販売価格</h4></td>
                                            <td class="text-right syouhinn">4300円</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>下代価格</h4></td>
                                            <td class="text-right syouhinn">2795円</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>卸掛率</h4></td>
                                            <td class="text-right syouhinn">65%</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>有効期限(開始日)</h4></td>
                                            <td class="text-right syouhinn">2021/01/25</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>有効期限(終了日)</h4></td>
                                            <td class="text-right syouhinn">2021/01/26</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>申込期日</h4></td>
                                            <td class="text-right syouhinn">納品日 50日前 0000まで</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>キャンセル期日</h4></td>
                                            <td class="text-right syouhinn">納品日 0日前 0000まで</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>最小ロット数</h4></td>
                                            <td class="text-right syouhinn">1個</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>在庫アラート数</h4></td>
                                            <td class="text-right syouhinn">残り0個になったらアラート</td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">パートナー企業情報</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>取扱パートナー企業名</h4></td>
                                            <td class="text-right syouhinn">株式会社アールピースファクトリー</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>取扱パートナー企業名ID</h4></td>
                                            <td class="text-right syouhinn"></td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>パートナー商品名</h4></td>
                                            <td class="text-right syouhinn">SHIN-CYA-KI KYU-SU HITORI（IVORY）</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>パートナー管理ID</h4></td>
                                            <td class="text-right syouhinn"></td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                        </v-col>
                         <v-col cols="4">
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">サイズ</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>幅(cm)</h4></td>
                                            <td class="text-right syouhinn">10.5</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>奥行き(cm)</h4></td>
                                            <td class="text-right syouhinn">10.5</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>高さ(cm)</h4></td>
                                            <td class="text-right syouhinn">11</td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">アイテム紹介</span>
                            </v-btn>
                             <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>１</h4></td>
                                        </tr>
                                        </tbody>
                                </template>
                             </v-simple-table> 
                             <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">(詳細項目A)</span>
                            </v-btn>
                            <br>
                            <br>
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">(詳細項目B)</span>
                            </v-btn>   
                            <br>
                            <br>
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">ハッシュタグ</span>
                            </v-btn>                       
                       </v-col>     
                    </v-row>   
                    <v-row justify="center">
                      <v-col cols="3">
                        <v-btn
                         depressed
                         outlined
                         color="red"
                        >
                        承認しない
                        </v-btn>
                        <v-btn 
                          class="ma-1"
                          depressed
                          color="red"
                        >
                        <div class="message">承認する</div>
                        </v-btn>
                      </v-col>
                    </v-row>      
                </v-expansion-panel-content>
                </v-expansion-panel>
            </v-expansion-panels>
        </v-alert>
        <v-alert
          border="left"
          color="red darken-1"
          outlined
          colored-border
        > 
            <v-expansion-panels  flat>
                <v-expansion-panel>
                <v-expansion-panel-header>
                            <v-row no-gutters>
                                <v-col cols="10">
                                  <h4>申請日時：2021年01月27日 17:55:09　SHIN-CYA-KI KYU-SU HITORI（BLACK)</h4>
                                </v-col>
                            </v-row>
                            <v-row
                                no-gutters
                            >
                            <v-col cols="9">
                              <h4>(株式会社アールピースファクトリー)</h4>
                            </v-col>  
                            </v-row>                  
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                    <v-row no-gutters>
                        <v-col cols="3">
                            <img src="https://placehold.jp/234x234.png">
                    <v-row justify="center">
                      <v-col cols="6">
                        <v-btn
                          small
                          shaped
                          outlined
                          depressed
                        >
                        <v-icon>mdi-pencil-outline</v-icon>
                        </v-btn>
                      </v-col>
                    </v-row>      
                            
                        </v-col>
                        <v-col cols="5">
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                              <span class="name">ブランド名</span>
                            </v-btn>  
                            <br>
                            <br>
                            AR Piece
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">価格・在庫</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>販売価格</h4></td>
                                            <td class="text-right syouhinn">4300円</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>下代価格</h4></td>
                                            <td class="text-right syouhinn">2795円</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>卸掛率</h4></td>
                                            <td class="text-right syouhinn">65%</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>有効期限(開始日)</h4></td>
                                            <td class="text-right syouhinn">2021/01/25</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>有効期限(終了日)</h4></td>
                                            <td class="text-right syouhinn">2021/01/26</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>申込期日</h4></td>
                                            <td class="text-right syouhinn">納品日 50日前 0000まで</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>キャンセル期日</h4></td>
                                            <td class="text-right syouhinn">納品日 0日前 0000まで</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>最小ロット数</h4></td>
                                            <td class="text-right syouhinn">1個</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>在庫アラート数</h4></td>
                                            <td class="text-right syouhinn">残り0個になったらアラート</td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">パートナー企業情報</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>取扱パートナー企業名</h4></td>
                                            <td class="text-right syouhinn">株式会社アールピースファクトリー</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>取扱パートナー企業名ID</h4></td>
                                            <td class="text-right syouhinn"></td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>パートナー商品名</h4></td>
                                            <td class="text-right syouhinn">SHIN-CYA-KI KYU-SU HITORI（IVORY）</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>パートナー管理ID</h4></td>
                                            <td class="text-right syouhinn"></td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                        </v-col>
                         <v-col cols="4">
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">サイズ</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>幅(cm)</h4></td>
                                            <td class="text-right syouhinn">10.5</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>奥行き(cm)</h4></td>
                                            <td class="text-right syouhinn">10.5</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>高さ(cm)</h4></td>
                                            <td class="text-right syouhinn">11</td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">アイテム紹介</span>
                            </v-btn>
                             <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>１</h4></td>
                                        </tr>
                                        </tbody>
                                </template>
                             </v-simple-table> 
                             <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">(詳細項目A)</span>
                            </v-btn>
                            <br>
                            <br>
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">(詳細項目B)</span>
                            </v-btn>   
                            <br>
                            <br>
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">ハッシュタグ</span>
                            </v-btn>                       
                       </v-col>     
                    </v-row>   
                    <v-row justify="center">
                      <v-col cols="3">
                        <v-btn
                         depressed
                         outlined
                         color="red"
                        >
                        承認しない
                        </v-btn>
                        <v-btn 
                          class="ma-1"
                          depressed
                          color="red"
                        >
                        <div class="message">承認する</div>
                        </v-btn>
                      </v-col>
                    </v-row>      
                </v-expansion-panel-content>
                </v-expansion-panel>
            </v-expansion-panels>
        </v-alert>  
        <v-alert
          border="left"
          color="red darken-1"
          outlined
          colored-border
        >
            <v-expansion-panels  flat>
                <v-expansion-panel>
                <v-expansion-panel-header>
                            <v-row no-gutters>
                                <v-col cols="10">
                                  <h4>申請日時：2021年01月27日 17:57:37　SHIN-CYA-KI KYU-SU HITORI（RED)</h4>
                                </v-col>
                            </v-row>
                            <v-row
                                no-gutters
                            >
                            <v-col cols="9">
                              <h4>(株式会社アールピースファクトリー)</h4>
                            </v-col>  
                            </v-row>                  
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                    <v-row no-gutters>
                        <v-col cols="3">
                            <img src="https://placehold.jp/234x234.png">
                            <v-row justify="center">
                      <v-col cols="6">
                        <v-btn
                          small
                          shaped
                          outlined
                          depressed
                        >
                        <v-icon>mdi-pencil-outline</v-icon>
                        </v-btn>
                      </v-col>
                    </v-row>      
                            
                        </v-col>
                        <v-col cols="5">
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                              <span class="name">ブランド名</span>
                            </v-btn>  
                            <br>
                            <br>
                            AR Piece
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">価格・在庫</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>販売価格</h4></td>
                                            <td class="text-right syouhinn">4300円</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>下代価格</h4></td>
                                            <td class="text-right syouhinn">2795円</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>卸掛率</h4></td>
                                            <td class="text-right syouhinn">65%</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>有効期限(開始日)</h4></td>
                                            <td class="text-right syouhinn">2021/01/25</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>有効期限(終了日)</h4></td>
                                            <td class="text-right syouhinn">2021/01/26</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>申込期日</h4></td>
                                            <td class="text-right syouhinn">納品日 50日前 0000まで</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>キャンセル期日</h4></td>
                                            <td class="text-right syouhinn">納品日 0日前 0000まで</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>最小ロット数</h4></td>
                                            <td class="text-right syouhinn">1個</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>在庫アラート数</h4></td>
                                            <td class="text-right syouhinn">残り0個になったらアラート</td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">パートナー企業情報</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>取扱パートナー企業名</h4></td>
                                            <td class="text-right syouhinn">株式会社アールピースファクトリー</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>取扱パートナー企業名ID</h4></td>
                                            <td class="text-right syouhinn"></td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>パートナー商品名</h4></td>
                                            <td class="text-right syouhinn">SHIN-CYA-KI KYU-SU HITORI（IVORY）</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>パートナー管理ID</h4></td>
                                            <td class="text-right syouhinn"></td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                        </v-col>
                         <v-col cols="4">
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">サイズ</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>幅(cm)</h4></td>
                                            <td class="text-right syouhinn">10.5</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>奥行き(cm)</h4></td>
                                            <td class="text-right syouhinn">10.5</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>高さ(cm)</h4></td>
                                            <td class="text-right syouhinn">11</td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">アイテム紹介</span>
                            </v-btn>
                             <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>１</h4></td>
                                        </tr>
                                        </tbody>
                                </template>
                             </v-simple-table> 
                             <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">(詳細項目A)</span>
                            </v-btn>
                            <br>
                            <br>
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">(詳細項目B)</span>
                            </v-btn>   
                            <br>
                            <br>
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">ハッシュタグ</span>
                            </v-btn>                       
                       </v-col>     
                    </v-row>   
                    <v-row justify="center">
                      <v-col cols="3">
                        <v-btn
                         depressed
                         outlined
                         color="red"
                        >
                        承認しない
                        </v-btn>
                        <v-btn 
                          class="ma-1"
                          depressed
                          color="red"
                        >
                        <div class="message">承認する</div>
                        </v-btn>
                      </v-col>
                    </v-row>      
                </v-expansion-panel-content>
                </v-expansion-panel>
            </v-expansion-panels>
        </v-alert>  
        <v-alert
          border="left"
          color="red darken-1"
          outlined
          colored-border
        >
            <v-expansion-panels  flat>
                <v-expansion-panel>
                <v-expansion-panel-header>
                            <v-row no-gutters>
                                <v-col cols="10">
                                  <h4>申請日時：2021年01月27日 18:27:24　SHIN-CYA-KI CYA-SARA（BLACK)</h4>
                                </v-col>
                            </v-row>
                            <v-row
                                no-gutters
                            >
                            <v-col cols="9">
                              <h4>(株式会社アールピースファクトリー)</h4>
                            </v-col>  
                            </v-row>                  
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                    <v-row no-gutters>
                        <v-col cols="3">
                            <img src="https://placehold.jp/234x234.png">
                            <v-row justify="center">
                      <v-col cols="6">
                        <v-btn
                          small
                          shaped
                          outlined
                          depressed
                        >
                        <v-icon>mdi-pencil-outline</v-icon>
                        </v-btn>
                      </v-col>
                    </v-row>      
                            
                        </v-col>
                        <v-col cols="5">
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                              <span class="name">ブランド名</span>
                            </v-btn>  
                            <br>
                            <br>
                            AR Piece
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">価格・在庫</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>販売価格</h4></td>
                                            <td class="text-right syouhinn">4300円</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>下代価格</h4></td>
                                            <td class="text-right syouhinn">2795円</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>卸掛率</h4></td>
                                            <td class="text-right syouhinn">65%</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>有効期限(開始日)</h4></td>
                                            <td class="text-right syouhinn">2021/01/25</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>有効期限(終了日)</h4></td>
                                            <td class="text-right syouhinn">2021/01/26</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>申込期日</h4></td>
                                            <td class="text-right syouhinn">納品日 50日前 0000まで</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>キャンセル期日</h4></td>
                                            <td class="text-right syouhinn">納品日 0日前 0000まで</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>最小ロット数</h4></td>
                                            <td class="text-right syouhinn">1個</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>在庫アラート数</h4></td>
                                            <td class="text-right syouhinn">残り0個になったらアラート</td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">パートナー企業情報</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>取扱パートナー企業名</h4></td>
                                            <td class="text-right syouhinn">株式会社アールピースファクトリー</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>取扱パートナー企業名ID</h4></td>
                                            <td class="text-right syouhinn"></td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>パートナー商品名</h4></td>
                                            <td class="text-right syouhinn">SHIN-CYA-KI KYU-SU HITORI（IVORY）</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>パートナー管理ID</h4></td>
                                            <td class="text-right syouhinn"></td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                        </v-col>
                         <v-col cols="4">
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">サイズ</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>幅(cm)</h4></td>
                                            <td class="text-right syouhinn">10.5</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>奥行き(cm)</h4></td>
                                            <td class="text-right syouhinn">10.5</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>高さ(cm)</h4></td>
                                            <td class="text-right syouhinn">11</td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">アイテム紹介</span>
                            </v-btn>
                             <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>１</h4></td>
                                        </tr>
                                        </tbody>
                                </template>
                             </v-simple-table> 
                             <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">(詳細項目A)</span>
                            </v-btn>
                            <br>
                            <br>
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">(詳細項目B)</span>
                            </v-btn>   
                            <br>
                            <br>
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">ハッシュタグ</span>
                            </v-btn>                       
                       </v-col>     
                    </v-row>   
                    <v-row justify="center">
                      <v-col cols="3">
                        <v-btn
                         depressed
                         outlined
                         color="red"
                        >
                        承認しない
                        </v-btn>
                        <v-btn 
                          class="ma-1"
                          depressed
                          color="red"
                        >
                        <div class="message">承認する</div>
                        </v-btn>
                      </v-col>
                    </v-row>      
                </v-expansion-panel-content>
                </v-expansion-panel>
            </v-expansion-panels>
        </v-alert>  
        <v-alert
          border="left"
          color="red darken-1"
          outlined
          colored-border
        >
            <v-expansion-panels  flat>
                <v-expansion-panel>
                <v-expansion-panel-header>
                            <v-row no-gutters>
                                <v-col cols="10">
                                  <h4>申請日時：2021年01月27日 17:52:14　SHIN-CYA-KI KYU-SU HITORI（IVORY）</h4>
                                </v-col>
                            </v-row>
                            <v-row
                                no-gutters
                            >
                            <v-col cols="9">
                              <h4>(株式会社アールピースファクトリー)</h4>
                            </v-col>  
                            </v-row>                  
                </v-expansion-panel-header>
                <v-expansion-panel-content>
                    <v-row no-gutters>
                        <v-col cols="3">
                            <img src="https://placehold.jp/234x234.png">
                            <v-row justify="center">
                      <v-col cols="6">
                        <v-btn
                          small
                          shaped
                          outlined
                          depressed
                        >
                        <v-icon>mdi-pencil-outline</v-icon>
                        </v-btn>
                      </v-col>
                    </v-row>      
                            
                        </v-col>
                        <v-col cols="5">
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                              <span class="name">ブランド名</span>
                            </v-btn>  
                            <br>
                            <br>
                            AR Piece
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">価格・在庫</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>販売価格</h4></td>
                                            <td class="text-right syouhinn">4300円</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>下代価格</h4></td>
                                            <td class="text-right syouhinn">2795円</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>卸掛率</h4></td>
                                            <td class="text-right syouhinn">65%</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>有効期限(開始日)</h4></td>
                                            <td class="text-right syouhinn">2021/01/25</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>有効期限(終了日)</h4></td>
                                            <td class="text-right syouhinn">2021/01/26</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>申込期日</h4></td>
                                            <td class="text-right syouhinn">納品日 50日前 0000まで</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>キャンセル期日</h4></td>
                                            <td class="text-right syouhinn">納品日 0日前 0000まで</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>最小ロット数</h4></td>
                                            <td class="text-right syouhinn">1個</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>在庫アラート数</h4></td>
                                            <td class="text-right syouhinn">残り0個になったらアラート</td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">パートナー企業情報</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>取扱パートナー企業名</h4></td>
                                            <td class="text-right syouhinn">株式会社アールピースファクトリー</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>取扱パートナー企業名ID</h4></td>
                                            <td class="text-right syouhinn"></td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>パートナー商品名</h4></td>
                                            <td class="text-right syouhinn">SHIN-CYA-KI KYU-SU HITORI（IVORY）</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>パートナー管理ID</h4></td>
                                            <td class="text-right syouhinn"></td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                        </v-col>
                         <v-col cols="4">
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">サイズ</span>
                            </v-btn>  
                            <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>幅(cm)</h4></td>
                                            <td class="text-right syouhinn">10.5</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>奥行き(cm)</h4></td>
                                            <td class="text-right syouhinn">10.5</td>
                                        </tr>
                                        <tr>
                                            <td class="syouhinn"><h4>高さ(cm)</h4></td>
                                            <td class="text-right syouhinn">11</td>
                                        </tr>
                                        </tbody>
                                </template>
                            </v-simple-table>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">アイテム紹介</span>
                            </v-btn>
                             <v-simple-table>
                                <template v-slot:default>
                                        <tbody>
                                        <tr>
                                            <td class="syouhinn"><h4>１</h4></td>
                                        </tr>
                                        </tbody>
                                </template>
                             </v-simple-table> 
                             <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">(詳細項目A)</span>
                            </v-btn>
                            <br>
                            <br>
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">(詳細項目B)</span>
                            </v-btn>   
                            <br>
                            <br>
                            <br>
                            <br>
                            <v-btn
                                rounded
                                depressed
                                height="22px"
                                color= "#B2EBF2"  
                            >
                            <span class="name">ハッシュタグ</span>
                            </v-btn>                       
                       </v-col>     
                    </v-row>   
                    <v-row justify="center">
                      <v-col cols="3">
                        <v-btn
                         depressed
                         outlined
                         color="red"
                        >
                        承認しない
                        </v-btn>
                        <v-btn 
                          class="ma-1"
                          depressed
                          color="red"
                        >
                        <div class="message">承認する</div>
                        </v-btn>
                      </v-col>
                    </v-row>      
                </v-expansion-panel-content>
                </v-expansion-panel>
            </v-expansion-panels>
        </v-alert>  
      </v-container>
    </v-card>
  </div>
</template>

<script>
export default {
    layout:"owner",
}
</script>

<style>
.message{
  color: #FFFFFF;
}
.kensaku{
    margin-top: 30px;
}
.syouhinn{
    border-bottom: 0 !important;
}
.name{
  color: #999;
}
.s{
  background-color: red;
}
</style>