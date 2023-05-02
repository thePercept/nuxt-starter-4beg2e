<template>
  <header>
    <nuxt-link :to="localePath('/')">
          <div>
            <img
              class="ancorp-logo-type"
              :src="require('@/assets/imgs/ancorpofficiallogo.webp')"
              alt="ANCORP LOGO"
            />
          </div>
        </nuxt-link>  
        <div>
              <nuxt-link :to="localePath('/')">Home &nbsp;|</nuxt-link>
              <nuxt-link :to="localePath('/news-and-events/')">News & Events</nuxt-link>
        </div>  
  </header>
 
</template>

<script>
export default {
  name:'siteHeader'
}
</script>
<style>
.ancorp-logo-type{
  width: 32rem;
}

</style>