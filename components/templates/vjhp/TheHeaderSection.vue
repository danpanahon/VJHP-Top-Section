<template>
  <div id="wrapper">
    <header id="header">
      <span class="logo">
        <img src="/marketing/img/vjhp/logo.svg" alt />
      </span>
      <h2>{{ header_section_welcome_message }}</h2>
      <h1>{{ header_section_main_heading }}</h1>
      <h3>{{ header_section_heading_subtitle }}</h3>
      <!-- <ul class="items-list gameslider">
        <li>
          <a href="#">
            <img src="/marketing/img/vjhp/game1.svg" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="/marketing/img/vjhp/game2.svg" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="/marketing/img/vjhp/game3.svg" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="/marketing/img/vjhp/game4.svg" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="/marketing/img/vjhp/game5.svg" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="/marketing/img/vjhp/game6.svg" />
          </a>
        </li>
      </ul> -->
      <h4>{{ header_section_best_deal_caption }}</h4>
      <div class="chest">
        <a href="#">
          <img src="/marketing/img/vjhp/chest.svg" />
        </a>
      </div>
      <p>{{ header_section_best_deal_small_caption }}</p>
      <a class="button primary" v-bind:href="header_section_register_button_url">{{ header_section_register_button }}</a>
      <p>
        {{ header_section_account_text }}
        <a v-bind:href="header_section_account_login">{{ header_section_account_login_url }}</a>
      </p>
      <style>
        :root {
          --bg-image: url('{{ images.promo_bg_desktop }}');
          --bg-image-m: url('{{ images.promo_bg_mobile }}');
          --game-logo: url('{{ images.promo_game_logo }}');
        }
      </style>
    </header>
  </div>
</template>
<script>
export default {
  name: 'TheHeaderSection',
  props: {
    header_text: {
      type: String,
      required: true,
    },
    header_button_redirect_url: {
      type: String,
      required: true,
    },
    header_login_account_text: {
      type: String,
      required: true,
    },
    header_login_account_text_redirect_url: {
      type: String,
      required: true,
    },
    homepage_title: {
      type: String,
      required: true,
    },
    login_header_text: {
      type: String,
      required: true,
    },
    login_header_redirect_url: {
      type: String,
      required: true,
    },
    header_section_welcome_message: {
      type: String,
      required: true,
    },
    header_section_main_heading: {
      type: String,
      required: true,
    },
    header_section_heading_subtitle: {
      type: String,
      required: true,
    },
    header_section_game_slider_url_1: {
      type: String,
      required: true,
    },
    header_section_game_slider_url_2: {
      type: String,
      required: true,
    },
    header_section_game_slider_url_3: {
      type: String,
      required: true,
    },
    header_section_game_slider_url_4: {
      type: String,
      required: true,
    },
    header_section_game_slider_url_5: {
      type: String,
      required: true,
    },
    header_section_game_slider_url_6: {
      type: String,
      required: true,
    },
    header_section_best_deal_caption: {
      type: String,
      required: true,
    },
    header_section_best_deal_small_caption: {
      type: String,
      required: true,
    },
    header_section_register_button: {
      type: String,
      required: true,
    },
    header_section_register_button_url: {
      type: String,
      required: true,
    },
    header_section_account_text: {
      type: String,
      required: true,
    },
    header_section_account_login: {
      type: String,
      required: true,
    },
    header_section_account_login_url: {
      type: String,
      required: true,
    }
  },
};
</script>

<style>
</style>