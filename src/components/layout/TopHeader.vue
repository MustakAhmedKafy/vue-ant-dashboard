<script setup>
import { ref } from 'vue'
import { CaretDownOutlined, LoginOutlined } from '@ant-design/icons-vue'
const value = ref('')
const isFullScreen = ref(false)
const toggleFullScreen = () => {
  isFullScreen.value = !isFullScreen.value
  const element = document.documentElement
  if (isFullScreen.value) {
    if (element.requestFullscreen) {
      element.requestFullscreen()
    } else if (element.mozRequestFullScreen) {
      element.mozRequestFullScreen()
    } else if (element.webkitRequestFullscreen) {
      element.webkitRequestFullscreen()
    } else if (element.msRequestFullscreen) {
      element.msRequestFullscreen()
    }
  } else {
    if (document.exitFullscreen) {
      document.exitFullscreen()
    } else if (document.mozCancelFullScreen) {
      document.mozCancelFullScreen()
    } else if (document.webkitExitFullscreen) {
      document.webkitExitFullscreen()
    } else if (document.msExitFullscreen) {
      document.msExitFullscreen()
    }
  }
}
</script>

<template>
  <a-layout-header
    style="
      background: #fff;
      padding: 0;
      display: flex;
      align-items: center;
      justify-content: space-between;
    "
  >
    <a-menu>
      <a-space direction="vertical">
        <a-input v-model:value="value" placeholder="Search" />
      </a-space>
    </a-menu>

    <a-space>
      <a-menu
       
        style=""
        >
        <a-button  @click="toggleFullScreen" style="border: 0px; display: flex; align-items: center; margin-right: 10px; box-shadow: none;">
          <svg
          xmlns="http://www.w3.org/2000/svg"
          width="20"
          height="20"
          fill="currentColor"
          class="bi bi-fullscreen"
          viewBox="0 0 16 16"
        >
          <path
            d="M1.5 1a.5.5 0 0 0-.5.5v4a.5.5 0 0 1-1 0v-4A1.5 1.5 0 0 1 1.5 0h4a.5.5 0 0 1 0 1zM10 .5a.5.5 0 0 1 .5-.5h4A1.5 1.5 0 0 1 16 1.5v4a.5.5 0 0 1-1 0v-4a.5.5 0 0 0-.5-.5h-4a.5.5 0 0 1-.5-.5M.5 10a.5.5 0 0 1 .5.5v4a.5.5 0 0 0 .5.5h4a.5.5 0 0 1 0 1h-4A1.5 1.5 0 0 1 0 14.5v-4a.5.5 0 0 1 .5-.5m15 0a.5.5 0 0 1 .5.5v4a1.5 1.5 0 0 1-1.5 1.5h-4a.5.5 0 0 1 0-1h4a.5.5 0 0 0 .5-.5v-4a.5.5 0 0 1 .5-.5"
          /></svg>
        </a-button>
        </a-menu>
      <a-menu>
        <a-dropdown class="admin-dropdown" placement="bottom">
          <template #overlay>
            <a-menu style="margin-top: -8px">
              <a-menu-item key="ac" style="padding-right: 30px; padding-bottom: 10px">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="16"
                  height="16"
                  fill="currentColor"
                  class="bi bi-person"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M8 8a3 3 0 1 0 0-6 3 3 0 0 0 0 6m2-3a2 2 0 1 1-4 0 2 2 0 0 1 4 0m4 8c0 1-1 1-1 1H3s-1 0-1-1 1-4 6-4 6 3 6 4m-1-.004c-.001-.246-.154-.986-.832-1.664C11.516 10.68 10.289 10 8 10c-2.29 0-3.516.68-4.168 1.332-.678.678-.83 1.418-.832 1.664z"
                  />
                </svg>
                <span style="padding-left: 8px" class="gray-menu-item">Account</span>
              </a-menu-item>
              <a-divider class="divider" />
              <a-menu-item key="se" style="padding-right: 30px; padding-bottom: 10px">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="16"
                  height="16"
                  fill="currentColor"
                  class="bi bi-gear"
                  viewBox="0 0 16 16"
                >
                  <path
                    d="M8 4.754a3.246 3.246 0 1 0 0 6.492 3.246 3.246 0 0 0 0-6.492zM5.754 8a2.246 2.246 0 1 1 4.492 0 2.246 2.246 0 0 1-4.492 0z"
                  />
                  <path
                    d="M9.796 1.343c-.527-1.79-3.065-1.79-3.592 0l-.094.319a.873.873 0 0 1-1.255.52l-.292-.16c-1.64-.892-3.433.902-2.54 2.541l.159.292a.873.873 0 0 1-.52 1.255l-.319.094c-1.79.527-1.79 3.065 0 3.592l.319.094a.873.873 0 0 1 .52 1.255l-.16.292c-.892 1.64.901 3.434 2.541 2.54l.292-.159a.873.873 0 0 1 1.255.52l.094.319c.527 1.79 3.065 1.79 3.592 0l.094-.319a.873.873 0 0 1 1.255-.52l.292.16c1.64.893 3.434-.902 2.54-2.541l-.159-.292a.873.873 0 0 1 .52-1.255l.319-.094c1.79-.527 1.79-3.065 0-3.592l-.319-.094a.873.873 0 0 1-.52-1.255l.16-.292c.893-1.64-.902-3.433-2.541-2.54l-.292.159a.873.873 0 0 1-1.255-.52l-.094-.319zm-2.633.283c.246-.835 1.428-.835 1.674 0l.094.319a1.873 1.873 0 0 0 2.693 1.115l.291-.16c.764-.415 1.6.42 1.184 1.185l-.159.292a1.873 1.873 0 0 0 1.116 2.692l.318.094c.835.246.835 1.428 0 1.674l-.319.094a1.873 1.873 0 0 0-1.115 2.693l.16.291c.415.764-.42 1.6-1.185 1.184l-.291-.159a1.873 1.873 0 0 0-2.693 1.116l-.094.318c-.246.835-1.428.835-1.674 0l-.094-.319a1.873 1.873 0 0 0-2.692-1.115l-.292.16c-.764.415-1.6-.42-1.184-1.185l.159-.291A1.873 1.873 0 0 0 1.945 8.93l-.319-.094c-.835-.246-.835-1.428 0-1.674l.319-.094A1.873 1.873 0 0 0 3.06 4.377l-.16-.292c-.415-.764.42-1.6 1.185-1.184l.292.159a1.873 1.873 0 0 0 2.692-1.115l.094-.319z"
                  />
                </svg>
                <span style="padding-left: 8px" class="gray-menu-item">Settings</span>
              </a-menu-item>
              <a-divider class="divider" />
              <a-menu-item key="lg" style="padding-right: 30px; padding-bottom: 10px">
                <LoginOutlined />
                <span style="padding-left: 8px" class="gray-menu-item">Log out</span>
              </a-menu-item>
            </a-menu>
          </template>
          <div>
            <a-avatar focus :size="44"> </a-avatar>
            <span class="gray-menu-item" style="margin-left: 8px"
              >Mustak <CaretDownOutlined
            /></span>
          </div>
        </a-dropdown>
      </a-menu>
    </a-space>
  </a-layout-header>
</template>
<style scoped>
.ant-layout-header {
  padding-inline: 60px !important;
}

.ant-divider-horizontal {
  margin: 5px 0px !important;
}

.ant-menu-light.ant-menu-root.ant-menu-vertical {
  border: none;
}

/* Add media query for responsiveness */
@media screen and (max-width: 768px) {
  .ant-layout-header {
    padding-inline: 16px !important; /* Adjust padding for smaller screens */
  }
}
</style>
