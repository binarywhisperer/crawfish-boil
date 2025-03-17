<template>
  <div class="content-container">
    <div class="content">
      <section>
        <CrawfishBoilHeader/>
      </section>
      <section>
        <SpiceKreweLaunchDay/>
      </section>
      <section>
        <RSVPButton/>
      </section>
      <section>
        <WhatToExpect/>
      </section>
      <section>
        <SpiceKreweAwards/>
      </section>
      <section class="footer">Made by <a href="https://brycesharp.com">Bryce</a> 2025</section>
    </div>
  </div>
</template>

<script>
import RSVPButton from './components/RSVPButton.vue'
import SpiceKreweAwards from './components/SpiceKreweAwards.vue'
import SpiceKreweLaunchDay from './components/SpiceKreweLaunchDay.vue'
import CrawfishBoilHeader from './components/CrawfishBoilHeader.vue'
import WhatToExpect from './components/WhatToExpect.vue'

export default {
  name: 'App',
  components: {
    RSVPButton,
    SpiceKreweAwards,
    SpiceKreweLaunchDay,
    CrawfishBoilHeader,
    WhatToExpect,
  }
}
</script>

<style lang="scss">
.content-container {
  display: flex;
  justify-content: center;

  .content {
    max-width: 1200px;
    width: 100vw;
  }
}
.footer{
  padding: 0 0 0 0;
  margin: 0 0 0 0;
  background: #fefefe;
  color: rgba(0,0,0,.5);
  text-align: center;
}
</style>
