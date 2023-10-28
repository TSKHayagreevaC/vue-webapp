<script setup>
  import Completion from './components/Completion.vue';
  import DeclerativeRendering from './components/DeclerativeRendering.vue';
  import AttributeBinding from './components/AttributeBinding.vue';
  import EventListeners from './components/EventListeners.vue';
  import FormBinding from './components/FormBinding.vue';
  import ConditionalRendering from './components/ConditionalRendering.vue';
  import ListRendering from './components/ListRendering.vue';
  import ComputedProperty from './components/ComputedProperty.vue';
  import LifecycleAndTemplateRef from './components/LifecycleAndTemplateRef.vue';
  import Watchers from './components/Watchers.vue';
  import ParentComponent from './components/ParentComponent.vue';
  import ParentComponentWithProps from './components/ParentComponentWithProps.vue';
  import ParentComponentWithEmits from './components/ParentComponentWithEmits.vue';
  import ParentComponentWithSlot from './components/ParentComponentWithSlot.vue';
</script>

<template>

  <div>
    <h3>Vue.js</h3>
    <h6>The Progressive JavaScript Framework</h6>
    <p>An approachable, performant and versatile framework for building web user interfaces.</p>
  </div>

  <div>
    <h3>Hello World..!</h3>
  </div>

  <DeclerativeRendering />

  <AttributeBinding />

  <EventListeners />

  <FormBinding />

  <ConditionalRendering />

  <ListRendering />

  <ComputedProperty />

  <LifecycleAndTemplateRef />

  <Watchers />

  <ParentComponent />

  <ParentComponentWithProps />

  <ParentComponentWithEmits />

  <ParentComponentWithSlot />

  <Completion />

</template>

<style>
div {
  border: 1px solid grey;
  border-radius: 5px;
  margin: 0.6rem;
  padding: 1rem;
  overflow: auto;
}
</style>
