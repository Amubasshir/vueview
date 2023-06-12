<template>
  <base-card>
    <base-button
      @click="setSelectedTab('stored-resources')"
      :mode="selectedTab === 'stored-resources' ? 'flat' : null"
      >Stored Resources</base-button
    >
    <base-button
      @click="setSelectedTab('add-resource')"
      :mode="selectedTab === 'add-resource' ? 'flat' : null"
      >Add Resources</base-button
    >
  </base-card>
  <component :is="selectedTab"></component>
</template>

<script>
import AddResource from './AddResource.vue';
import StoredResources from './StoredResources.vue';
export default {
  components: {
    StoredResources,
    AddResource,
  },
  data() {
    return {
      selectedTab: 'stored-resources',
      storedResources: [
        {
          id: 'welcomeqqq',
          name: 'welcomeqqqq 2',
          details: 'welcome to the new movie',
          link: 'http://movie.com',
        },
        {
          id: 'zawelcomeqqq',
          name: 'welcomeqqqq 211',
          details: 'welcome xzc zczcsdto the new movie',
          link: 'http://movie2.com',
        },
      ],
    };
  },
  provide() {
    return {
      resources: this.storedResources,
    };
  },
  methods: {
    setSelectedTab(tab) {
      this.selectedTab = tab;
    },
  },
};
</script>
