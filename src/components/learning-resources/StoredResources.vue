<template>
<ul>
    <ResourceItem v-for="resource in resources" :key="resource.id" :title="resource.title" :description="resource.description" :link="resource.link">
    </ResourceItem>
</ul>
</template>

<script>
import ResourceItem from './ResourceItem';
export default {
    name: 'StoredResources',
    inject: ['resources'],
    components: {
        ResourceItem
    }
}
</script>

<style scoped>
ul {
    list-style: none;
    margin: 0;
    padding: 0;
    margin: auto;
    max-width: 40rem;
}
</style>
