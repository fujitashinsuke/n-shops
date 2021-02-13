<template>
  <v-app>
    <div
      v-shortkey="['ctrl', '/']"
      class="d-flex flex-grow-1"
      @shortkey="onKeyup"
    >
      <!-- Navigation -->
      <v-navigation-drawer
        v-model="drawer"
        app
        floating
        class="elevation-1"
        :right="$vuetify.rtl"
        :light="menuTheme === 'light'"
        :dark="menuTheme === 'dark'"
      >
        <!-- Navigation menu info -->
        <template v-slot:prepend>
          <div class="pa-2">
            <div class="title font-weight-bold text-uppercase primary--text">N-Shops</div>
            <div class="overline grey--text">{{ product.version }}</div>
          </div>
        </template>

        <!-- Navigation menu -->
        <v-list max-width="300px">
        <v-list-item
          v-for="[icon, text, url] in links"
          :key="icon"
          :to="url"
          link
        >
          <v-list-item-icon>
            <v-icon>{{ icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ text }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>

        <!-- Navigation menu footer -->
        <template v-slot:append>
          <!-- Footer navigation links -->
          <!-- REMOVE ME - Shop Demo purposes -->
        </template>
      </v-navigation-drawer>

      <!-- Toolbar -->
      <v-app-bar
        app
        :color="isToolbarDetached ? 'surface' : undefined"
        :flat="isToolbarDetached"
        :light="toolbarTheme === 'light'"
        :dark="toolbarTheme === 'dark'"
      >
        <v-card class="flex-grow-1 d-flex" :class="[isToolbarDetached ? 'pa-1 mt-3 mx-1' : 'pa-0 ma-0']" :flat="!isToolbarDetached">
          <div class="d-flex flex-grow-1 align-center">

            <!-- search input mobile -->
            <v-text-field
              v-if="showSearch"
              append-icon="mdi-close"
              placeholder="Search"
              prepend-inner-icon="mdi-magnify"
              hide-details
              solo
              flat
              autofocus
              @click:append="showSearch = false"
            ></v-text-field>

            <div v-else class="d-flex flex-grow-1 align-center">
              <v-app-bar-nav-icon @click.stop="drawer = !drawer"></v-app-bar-nav-icon>

              <v-spacer class="d-none d-lg-block"></v-spacer>

              <!-- search input desktop -->

              <v-spacer class="d-block d-sm-none"></v-spacer>

              <v-btn class="d-block d-sm-none" icon @click="showSearch = true">
                <v-icon>mdi-magnify</v-icon>
              </v-btn>


              <toolbar-user />
            </div>
          </div>
        </v-card>
      </v-app-bar>

      <v-main>
        <v-container class="fill-height" :fluid="!isContentBoxed">
          <v-layout>
            <nuxt />
          </v-layout>
        </v-container>
      </v-main>
    </div>
  </v-app>
</template>

<script>
import { mapState } from 'vuex'

// navigation menu configurations
import config from '../configs'

import MainMenu from '../components/navigation/MainMenu'
import ToolbarUser from '../components/toolbar/Toolbarowner'
import ToolbarApps from '../components/toolbar/ToolbarApps'
import ToolbarLanguage from '../components/toolbar/ToolbarLanguage'
import ToolbarCurrency from '../components/toolbar/ToolbarCurrency'
import ToolbarNotifications from '../components/toolbar/ToolbarNotifications'

export default {
  components: {
    MainMenu,
    ToolbarUser,
    ToolbarApps,
    ToolbarLanguage,
    ToolbarCurrency,
    ToolbarNotifications
  },
  data() {
    return {
      drawer: null,
      showSearch: false,
      links: [
        [ 'mdi-home', 'TOP', "/owner/owner"],
        ['mdi-gift', 'コレクション',"/owner/colection/list"],
        ['mdi-gift', '特集',"/owner/tokushyu/list"],
        ['mdi-account-supervisor-circle', 'パートナー', "/owner/partner/list"],
        ['mdi-account-supervisor-circle-outline', 'ブランド', "/owner/brand/list"],
        ['mdi-package-variant-closed ', 'アイテム', "/owner/item/list"],
        ['mdi-account-details', '顧客', "/owner/kokyaku/list"],
        ['mdi-cart', '注文履歴', "/owner/chumonrireki/list"],
        ['mdi-email', 'お問い合わせ', "/owner/otoiawase/list"],  
      ],
      navigation: config.navigation
    }
  },
  computed: {
    ...mapState('app', ['product', 'isContentBoxed', 'menuTheme', 'toolbarTheme', 'isToolbarDetached'])
  },
  methods: {
    onKeyup(e) {
      this.$refs.search.focus()
    }
  }
}
</script>

<style scoped>
.buy-button {
  box-shadow: 1px 1px 18px #ee44aa;
}
</style>
