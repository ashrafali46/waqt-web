<template>
  <div id="headerBox">
    <div id="headerText">Waqt</div>
    <font-awesome-icon
      id="headerSettings"
      class="iconButton"
      icon="cog"
      @click="$emit('show-dialog')"
    />
  </div>
</template>

<script>
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

export default {
  name: 'Headerbox',
  components: {
    FontAwesomeIcon
  }
};
</script>

<style lang="scss" scoped>
@import '../styles/base';

#headerBox {
  font-family: $base-font;
  color: #eee;
  padding: 20px;
  font-size: 20pt;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  #headerText {
    color: map-get($map: $theme, $key: text);
  }
}
</style>
