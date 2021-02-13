<template>
  <div class="d-flex flex-column flex-grow-1">
    <div class="d-flex align-center py-1">
      <div>
        <div class="display-1">お問い合わせ</div>
      </div>
      <v-spacer></v-spacer>
        <v-btn-toggle
                rounded
                tile
                dense
                shaped
        >
            <v-btn plain text> 
                対応中
            </v-btn>
            <v-btn plain text>
              完了
            </v-btn>
          </v-btn-toggle>
        </div>  
      <v-card>
      <v-container fluid>
        <v-alert
          border="left"
          color="cyan accent-2"
          outlined
          colored-border
          class="s"
        >
          <v-card-title>
            藤田比呂文様
            <v-card-subtitle>最新メッセージ：2019/10/08 15:13:35</v-card-subtitle>
            <v-spacer></v-spacer>
            <v-btn
              depressed
              color="#00E5FF"
              shaped
              width="180px"
              height="40px"
            >
              <span class="message">メッセージを見る</span>
            </v-btn>
          </v-card-title>
        </v-alert>
        <v-alert
          border="left"
          color="cyan accent-2"
          outlined
          colored-border
          class="s"
        >
          <v-card-title>
            中川智子 様 
            <v-card-subtitle>最新メッセージ：2019/10/08 15:13:35</v-card-subtitle>
            <v-spacer></v-spacer>
            <v-btn
              depressed
              color="#00E5FF"
              shaped
              width="180px"
              height="40px"
            >
              <span class="message">メッセージを見る</span>
            </v-btn>
          </v-card-title>
        </v-alert>
        <v-alert
          border="left"
          color="cyan accent-2"
          outlined
          colored-border
          class="s"
        >
          <v-card-title>
            迫田紫穂 様 
            <v-card-subtitle>最新メッセージ：2019/10/08 15:13:35</v-card-subtitle>
            <v-spacer></v-spacer>
            <v-btn
              depressed
              color="#00E5FF"
              shaped
              width="180px"
              height="40px"
            >
              <span class="message">メッセージを見る</span>
            </v-btn>
          </v-card-title>
        </v-alert>
        <v-alert
          border="left"
          color="cyan accent-2"
          outlined
          colored-border
          class="s"
        >
          <v-card-title>
            森山咲良 様
            <v-card-subtitle>最新メッセージ：2019/10/08 15:13:26</v-card-subtitle>
            <v-spacer></v-spacer>
            <v-btn
              depressed
              color="#00E5FF"
              shaped
              width="180px"
              height="40px"
            >
              <span class="message">メッセージを見る</span>
            </v-btn>
          </v-card-title>
        </v-alert>
        <v-alert
          border="left"
          color="cyan accent-2"
          outlined
          colored-border
          class="s"
        >
          <v-card-title>
              ユニオン太郎 様 
            <v-card-subtitle>最新メッセージ：2019/10/08 15:14:03</v-card-subtitle>
            <v-spacer></v-spacer>
            <v-btn
              depressed
              color="#00E5FF"
              shaped
              width="180px"
              height="40px"
            >
              <span class="message">メッセージを見る</span>
            </v-btn>
          </v-card-title>
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
</style>