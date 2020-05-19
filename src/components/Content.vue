<template lang="pug">
    #Content
        table(cellpadding="0" cellspacing="0" border='1')
            tr(v-for="(c, index) in categries" :key="index")
                td {{ c.name }}
                td
                    img(:src="c.item1")
                td
                    img(:src="c.item2")
</template>

<script>
export default {
  data () {
    return {
      categries: [
        {
          name: '流行皮件',
          item1: './img/0403.jpg',
          item2: './img/0404.jpg'
        },
        {
          name: '流行鞋區',
          item1: './img/0405.jpg',
          item2: './img/0406.jpg'
        },
        {
          name: '流行飾品',
          item1: './img/0407.jpg',
          item2: './img/0408.jpg'
        }
      ]
    }
  }
}
</script>
