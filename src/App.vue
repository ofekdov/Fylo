<template>
  <section>
    <AppHeader />
    <RouterView/>
    <UserMsg/>
    <AppFooter/>
  </section>
</template>

<script>


import { userService } from './services/user.service'
import { store } from './store/store'

import AppHeader from './cmps/AppHeader.vue'
import UserMsg from './cmps/UserMsg.vue'
import AppFooter from './cmps/AppFooter.vue'

export default {

  created() {
    console.log('Vue App created')
    const user = userService.getLoggedinUser()
    if (user)  store.commit({type: 'setLoggedinUser', user})
  },
  components: {
    AppHeader,
    UserMsg,
    AppFooter
  },
}
</script>