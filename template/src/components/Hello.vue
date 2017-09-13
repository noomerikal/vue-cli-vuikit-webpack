<template>
  <div class="uk-container uk-container-center uk-text-center uk-margin-large-top">
    <img src="./assets/logo.png">
    <h1>\{{ msg }}</h1>
    <h2>Essential Links</h2>
    <ul class="uk-subnav uk-flex-center">
      <li><a href="https://vuejs.org" target="_blank">Vue.js</a></li>
      <li><a href="https://vuikit.js.org" target="_blank">Vuikit</a></li>
      <li><a href="https://getuikit.com/" target="_blank">UIKit</a></li>
    </ul>
    <vk-button>vk-button test</vk-button>
  </div>
</template>

<script>
export default {
  name: 'hello',
  data{{#unless_eq lintConfig "airbnb"}} {{/unless_eq}}() {
    return {
      msg: 'Welcome to Your Vue Vuikit App'{{#if_eq lintConfig "airbnb"}},{{/if_eq}}
    }{{#if_eq lintConfig "airbnb"}};{{/if_eq}}
  }{{#if_eq lintConfig "airbnb"}},{{/if_eq}}
}{{#if_eq lintConfig "airbnb"}};{{/if_eq}}
</script>
