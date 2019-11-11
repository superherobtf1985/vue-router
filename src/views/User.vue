<template>
  <div class="user">
    <h1>{{ this.$route.params.id }}</h1>
    <router-link :to="{name: 'first'}">First</router-link> |
    <router-link :to="{name: 'second'}">Second</router-link> |
    <p>{{ this.$route.query.q }}</p>
    <transition name="shake" mode="out-in">
      <router-view/>
    </transition>
  </div>
</template>

