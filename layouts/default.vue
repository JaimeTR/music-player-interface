<template>
  <div class="flex">
    <AppSidebar>
      <GroupSidebar title="Menu">
        <ApSidebarItem active>Home</ApSidebarItem>
        <ApSidebarItem>Search</ApSidebarItem>
        <ApSidebarItem>Discover</ApSidebarItem>
        <ApSidebarItem>Albums</ApSidebarItem>
        <ApSidebarItem>Artists</ApSidebarItem>
      </GroupSidebar>
      <GroupSidebar title="Library">
        <ApSidebarItem>Recent</ApSidebarItem>
        <ApSidebarItem>Favourites</ApSidebarItem>
        <ApSidebarItem>Local</ApSidebarItem>
      </GroupSidebar>
      <GroupSidebar title="Playlist">
        <ApSidebarItem>Create new</ApSidebarItem>
        <ApSidebarItem>Pop punk</ApSidebarItem>
        <ApSidebarItem>Rocks</ApSidebarItem>
      </GroupSidebar>
      <GroupSidebar title="General">
        <ApSidebarItem>Settings</ApSidebarItem>
        <ApSidebarItem>Log out</ApSidebarItem>
      </GroupSidebar>
    </AppSidebar>
    <div class="flex-auto flex">
      <nav class="h-20 fixed top-0 w-full bg-opacity-50"></nav>
      <Nuxt class="flex-auto mt-20" />
    </div>
  </div>
</template>

<script>
import AppSidebar from '@/components/layout/AppSidebar'
import ApSidebarItem from '@/components/layout/ApSidebarItem'
import GroupSidebar from '@/components/layout/GroupSidebar'

export default {
  components: {
    AppSidebar,
    ApSidebarItem,
    GroupSidebar,
  },
  data() {
    return {
      menuOptions: [{ key: 1 }],
    }
  },
}
</script>
