<template>
<div class = "contacts-wrapper">
  <pageTitle title="Contacts"></pageTitle>
  <div class="contacts">
    <p>私の<a href="https://twitter.com/plus_kyoto" target="_blank">Twitter</a>もしくはMail (naokikishi.kyoto[at]gmail.com)からお問い合わせください。</p>
  </div>
</div>
</template>

<script>
import pageTitle from '@/components/pageTitle'

export default {
  name: 'Contacts',
  title: 'Contacts -',
  components: {
    pageTitle
  },
  data () {
    return {
    }
  }
}
</script>

<style lang="scss" scoped>
@import '@/assets/styles/_color.scss';
@import '@/assets/styles/_mixin.scss';

.contacts-wrapper{
  text-align: center;
}

.contacts{
  @include box-shadow;
  width : 800px;
  border-radius: 50px;
  margin: 20px auto;
  color : $text-color;
}

@media (max-width : 1000px){
  .contacts{
    width : 80%;
    word-break:break-all;
  }
}

p{
  padding : 40px 20px;
}

a{
  text-decoration: none;
}
</style>
