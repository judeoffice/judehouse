<template>
  <v-app>
    <v-card class="overflow-hidden">
      <v-app-bar
        absolute
        color="white"
        elevate-on-scroll
        height="60px" 
        scroll-target="#scrolling-techniques-7"
        style="padding: 0px"
      >
        <v-row
          justify="center"
          no-gutters
          style="margin: 0px 240px; padding: 0px"
        >
          <v-btn
            color="primary"
            text
            class="my-2"
            style="font-size: 16px"
          >
            judehouse
          </v-btn>

          <v-spacer></v-spacer>

          <v-btn
            v-for="category in categories"
            :key="category.link"
            color="#4E5968"
            text
            class="my-2"
            style="font-size: 15px"
          >
            {{ category.caption }}
          </v-btn>

          <v-spacer></v-spacer>

          <v-btn
            color="#333D4B"
            text
            class="my-2"
            style="font-size: 16px"
          >
            KOR
          </v-btn>

          <v-divider
            class="my-4"
            vertical
          ></v-divider>

          <v-btn
            color="#B0B8C1"
            text
            class="my-2"
            style="font-size: 16px"
          >
            ENG
          </v-btn>
        </v-row>
      </v-app-bar>
      <v-sheet
        id="scrolling-techniques-7"
        class="overflow-y-auto"
        max-height="1200px"
        color="#F9FAFB"
      >
        <v-container style="height: 1500px;">
        </v-container>
      </v-sheet>
      <v-footer
        dark
        padless
      >
        <v-card
          flat
          tile
          color="#191F28"
          height="640px"
        >
          <v-card-text>
            <v-btn
              v-for="icon in icons"
              :key="icon"
              class="mx-4 white--text"
              icon
            >
              <v-icon size="24px">
                {{ icon }}
              </v-icon>
            </v-btn>
          </v-card-text>

          <v-card-text class="white--text pt-0">
            Phasellus feugiat arcu sapien, et iaculis ipsum elementum sit amet. Mauris cursus commodo interdum. Praesent ut risus eget metus luctus accumsan id ultrices nunc. Sed at orci sed massa consectetur dignissim a sit amet dui. Duis commodo vitae velit et faucibus. Morbi vehicula lacinia malesuada. Nulla placerat augue vel ipsum ultrices, cursus iaculis dui sollicitudin. Vestibulum eu ipsum vel diam elementum tempor vel ut orci. Orci varius natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus.
          </v-card-text>

          <v-divider></v-divider>

          <v-card-text class="white--text">
            {{ new Date().getFullYear() }} — <strong>Vuetify</strong>
          </v-card-text>
        </v-card>
      </v-footer>
    </v-card>
  </v-app>
</template>

<script>
  export default {
    data: () => ({
      categories: [
        { caption: '회사 소개', link: '1' },
        { caption: '고객센터', link: '2' },
        { caption: '자주 묻는 질문', link: '3' },
        { caption: '공동인증서 관리', link: '4' },
        { caption: '채용', link: '5' },
      ],
      icons: [
        'mdi-facebook',
        'mdi-twitter',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>

<style>

</style>