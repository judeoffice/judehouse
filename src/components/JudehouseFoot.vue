<template>
  <v-card
    flat
    tile
    color="#191F28"
    class="white--text text-center"
    width="100%"
  >
    <v-card-text style="font-size:15px; font-color:#B0B8C1">
      ㈜비바리퍼블리카
    </v-card-text>

    <v-card-text style="font-size:13px; font-color:#8B95A1">
      사업자 등록번호 : 120-88-01280 | 대표 : 이승건
    </v-card-text>

    <v-card-text style="font-size:13px; font-color:#8B95A1">
      호스팅 서비스 : 주식회사 비바리퍼블리카 | 통신판매업 신고번호 : 2014-서울강남-03377 사업자정보확인
    </v-card-text>

    <v-card-text style="font-size:13px; font-color:#8B95A1">
      06236 서울특별시 강남구 테헤란로 142, 12층 (역삼동, 아크플레이스)
    </v-card-text>

    <v-card-text>
      <v-btn
        v-for="term in terms"
        :key="term"
        elevation="0"
        text
        color="#6B7684"
        style="font-size:13px"
      >
        {{ term }}
      </v-btn>
    </v-card-text>
    
    <v-card-text>
      <v-btn
        v-for="icon in icons"
        :key="icon"
        class="mx-2"
        fab
        elevation="0"
        height="36px"
        width="36px"
        color="#525C68"
      >
        <v-icon
          color="#AFB2B5"
          size="20px"
        >
          {{ icon }}
        </v-icon>
      </v-btn>
    </v-card-text>
  </v-card>
</template>

<script>
  export default {
    name: 'JudehouseHead',
    data: () => ({
      terms: [
        '서비스 이용약관',
        '통합 금융정보 서비스 약관',
        '이용자의 권리 및 유의사항',
        '개인정보 처리방침',
        '위치기반서비스 이용약관',
        '가맹점 고지사항',
      ],
      icons: [
        'mdi-gmail',
        'mdi-github',
        'mdi-youtube',
        'mdi-linkedin',
        'mdi-instagram',
      ],
    }),
  }
</script>

<style>

</style>