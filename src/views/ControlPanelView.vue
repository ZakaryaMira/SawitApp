<template>
  <NavComponent />
  <ControlPanelMainSection />
  <ControlPanelSearchBar />
  <UserPersonalCampagneList />
</template>
<script>
import NavComponent from '@/components/NavComponent/NavComponent.vue'
import ControlPanelMainSection from '@/components/ControlPanelComponents/ControlPanelMainSection.vue'
import ControlPanelSearchBar from '@/components/ControlPanelComponents/ControlPanelSearchBar.vue'
import UserPersonalCampagneList from '@/components/ControlPanelComponents/UserPersonalCampagneList.vue'
export default {
  components: {
    NavComponent,
    ControlPanelMainSection,
    ControlPanelSearchBar,
    UserPersonalCampagneList,
  },
}
</script>
