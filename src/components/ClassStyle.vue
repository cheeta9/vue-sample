<template>
  <div>first</div>
  <div
    class="bold"
    :class="{ italic: isItalic, red: isRed }"
  >second</div>
  <div :class="{ italic: isItalic, blue: isBlue }">third</div>
  <div :class="fourthObject">fourth</div>
  <div :class="fifthObject">fifth</div>
  <div :class="[italicClass, blueClass]">sixth</div>
  <div :class="[{ italic: !isItalic }, blueClass]">seventh</div>
  <div :style="{ color: favoriteColor, fontSize: fontSize + 'px' }">eighth</div>
  <div :style="ninethObject">nineth</div>
</template>

<script>
export default {
  data() {
    return {
      isItalic: true,
      isRed: true,
      isBlue: false,
      fourthObject: { italic: false, blue: true },
      error1: 'fatal',
      italicClass: 'italic',
      blueClass: 'blue',
      favoriteColor: 'orange',
      fontSize: 30,
      ninethObject: { color: 'purple', fontSize: '25px' }
    }
  },
  computed: {
    fifthObject() {
      return {
        red: this.isRed && this.error1 === 'fatal'
      }
    }
  }
}
</script>
