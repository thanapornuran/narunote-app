<template>
  <div class="layout">
    <NuxtLayout />
  </div>
  <div class="page">
    <NuxtPage class="body-page" />
  </div>
</template>

<style>
  @import url('./assets/css/main.css');

  body {
    font-family: 'RobotoItalic', sans-serif;
    background-color: var(--background-color);
    width: 100%;
    color: #fffffe;
  }

  .layout {
    width: 240px;
    /* Fixed width for sidebar */
    height: 100vh;
    display: flex;
    flex-direction: column;
    position: fixed;
    left: 0;
    top: 0;
    border-right: 1px solid #e0e0e0;
    z-index: 10;
  }

  .page {
    margin-left: 240px;
    padding: 1.5%;
    width: calc(100vw - 240px);
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: start;
    color: var(--haedline-color);
  }

  .body-page {
    border-radius: 15px;
    width: 100%;
    height: 100%;
    padding: 1.5%;
    background-color: #55423d;
    color: var(--haedline-color);
  }
</style>