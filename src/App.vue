<template>
  <!-- <h1>i love vue</h1>
  <TButton label="tlačítko" class="my-class"/>
  <TList :listItems="fruits" /> -->
  <!-- <input :type="inputType" :disabled="isDisabled"/> -->
  <!-- <TInput label="first name" inputId="first" class="my-class"/>
  <TInput label="last name" inputId="last" />
  <TInput label="your age" inputId="age" inputType="number" isDisabled /> -->


  <!--
    - interpolace ({{  }})
    - datová komunikace rodič -> dítě (v-bind)
    - datová komunikace v obráceném směru
    - event listenery
    - podmíněné renderování
    - renderování v cyklu
    - routing
    - data store
    - podmíněné styly
    - form handling, input controls
  -->
  <button v-if="!(condition % 2)">Even</button>
  <button v-else>Odd</button>
  <!-- <button v-else>Another</button> -->
  <nav>
    <ul>
      <li>Home</li>
      <li>About</li>
    </ul>
  </nav>
  <HomePage />
  <AboutPage />
  <TButton label="moje tlačítečko" />
</template>

<script>

import TButton from '@/components/TButton.vue'
import TList from '@/components/TList.vue'
import TInput from '@/components/TInput.vue'
import HomePage from '@/pages/HomePage.vue'
import AboutPage from '@/pages/AboutPage.vue'

export default {
  name: 'App',
  data() {
    return {
      fruits: ['banán', 'švestka', 'jablko'],
      // inputType: 'number',
      // isDisabled: 0
      condition: 79
    }
  },
  components: { TButton, TList, TInput, HomePage, AboutPage }
}

</script>

