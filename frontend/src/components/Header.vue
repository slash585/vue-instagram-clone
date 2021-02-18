<script>
import IconHome from '@/icons/home.svg'
import IconHomeFill from '@/icons/home-fill.svg'
import IconDirect from '@/icons/direct.svg'
import IconDirectFill from '@/icons/direct-fill.svg'
import IconExplore from '@/icons/explore.svg'
import IconExploreFill from '@/icons/explore-fill.svg'
import Avatar from '@/components/Avatar.vue'
import Container from './Container.vue'

export default {
  components:{
    Container,
    IconHome,
    IconHomeFill,
    IconDirect,
    IconDirectFill,
    IconExplore,
    IconExploreFill,
    Avatar
  }
}
</script>

<template lang="pug">
.header
  Container.header-inner
    router-link.logo(to="/") Instagram
    from.search
      input(type="text" placeholder="Search...")
    nav.navigation
      router-link(to="/")
        IconHomeFill(v-if="$route.name == 'Home'")
        IconHome(v-else)
      router-link(to="/direct")
        IconDirectFill(v-if="$route.name == 'Direct'")
        IconDirect(v-else)
      router-link(to="/explore")
        IconExploreFill(v-if="$route.name == 'Explore'")
        IconExplore(v-else)
      router-link(to="/profile")
        Avatar(:size="26")

</template>

<style scoped>

.header {
  border-bottom: 1px solid rgb(var(--b6a));
}

.header-inner {
  height: 60px;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  align-items: center;
}

.search {
    text-align: center;
}

.search input{
    height: 28px;
    width: 215px;
    border: 1px solid rgb(var(--b6a));
    border-radius: 4px;
    background-color: rgb(var(--b3f));
    padding-left: 20px;
    padding-right: 20px;
}

.logo {
    font-size: 1.6rem;
    font-weight: bold;

}

.navigation {
    display: flex;
    justify-content: flex-end;
    align-items: center;
}

.navigation a{
    margin-left: 20px;
}
</style>