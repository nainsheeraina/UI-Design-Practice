<template>
  <q-layout view="lHh Lpr lFf">
    <q-header>
      <div class="row">
        <q-toolbar>
        <q-toolbar-title>
          <q-img src="src\statics\logo.png" style="width:50px;"></q-img>
        </q-toolbar-title>
        <div class="gt-sm">
          <q-btn label="Courses" flat class="q-mr-sm"></q-btn>
          <q-btn label="Register" rounded outline class="q-mr-sm"></q-btn>
          <q-btn label="Login" rounded outline></q-btn>
        </div>
        <div class="lt-md">
          <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="toggleLeftDrawer"
        /></div>
      </q-toolbar>

    </div>

    </q-header>
    <q-drawer
      v-model="leftDrawerOpen"
      bordered
    >
      <q-list>
        <q-item-label
          header
        >
          Essential Links
        </q-item-label>

        <EssentialLink
          v-for="link in essentialLinks"
          :key="link.title"
          v-bind="link"
        />
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
    <q-footer elevated>
        <q-toolbar>
          <q-toolbar-title><div class="text-center text-h6 text-bold">&copy;CodeHelp-2023</div></q-toolbar-title>
        </q-toolbar>
      </q-footer>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'
import EssentialLink from 'components/EssentialLink.vue'
import Courses from 'src/pages/Courses.vue'

const linksList = [
  {
    title: 'Courses',
    caption: 'Access All The Courses Here',
    icon: 'article',
    link: '#'
  },
  {
    title: 'Register',
    caption: 'Create Account From Here',
    icon: 'app_registration',
    link: '#'
  },
  {
    title: 'Login',
    caption: 'Login To Your Account From Here ',
    icon: 'login',
    link: '#'
  },
  {
    title: 'Forum',
    caption: 'Ask Your Queries',
    icon: 'record_voice_over',
    link: '#'
  }
]

export default defineComponent({
  name: 'MainLayout',

  components: {
    EssentialLink
  },

  setup () {
    const leftDrawerOpen = ref(false)

    return {
      essentialLinks: linksList,
      leftDrawerOpen,
      toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
})
</script>
