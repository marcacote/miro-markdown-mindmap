import './assets/style.css';

<script setup lang="ts">
  async function addSticky() {
    const stickyNote = await miro.board.createStickyNote({
      content: 'Hello, World!',
    });

    await miro.board.viewport.zoomTo(stickyNote);
  }
  addSticky()
</script>

<template>
    <div id="root">
      <div class="grid wrapper">
        <div class="cs1 ce12">
          <img src="/src/assets/congratulations.png" alt="" />
        </div>
        <div class="cs1 ce12">
          <h1>Congratulations!</h1>
          <p>You've just created your first Miro app!</p>
          <p>
            To explore more and build your own app, see the Miro Developer
            Platform documentation.
          </p>
        </div>
        <div class="cs1 ce12">
          <a
              class="button button-primary"
              target="_blank"
              href="https://developers.miro.com"
          >
            Read the documentation
          </a>
        </div>
      </div>
    </div>
</template>

<style>
</style>
