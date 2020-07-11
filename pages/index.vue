<template>
  <div class="container">
    <div>
      <!-- <p>{{ $store.state.message }}</p> -->
      <p>{{ $store.state.hello.message }}</p>
      <!-- <button @click="$store.commit('updateMessage')">Update</button> -->
      <!-- <button @click="$store.commit('updateMessage', 'Commit with payload')">Update</button> -->
      <!-- <button @click="$store.dispatch('updateMessageAction')">Dispatch</button> -->
      <!-- <button @click="$store.dispatch('updateMessageAction', 'Dispatch with payload')">Dispatch</button> -->
      <button
        @click="$store.dispatch('hello/updateMessageAction', 'Dispatch with payload')"
      >Dispatch</button>
    </div>
  </div>
</template>

<script>
export default {};
</script>

