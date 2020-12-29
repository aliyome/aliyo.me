<script lang="ts">
  import Icon from './Icon.svelte';
  import { faTwitter } from '@fortawesome/free-brands-svg-icons';
</script>

<style global lang="postcss">
  @tailwind base;
  @tailwind components;
  @tailwind utilities;
</style>

<main class="p-6 text-gray-800">
  <h1 class="text-xl">aliyome</h1>
  <hr />
  <a
    href="https://twitter.com/aliyome"
    target="_blank"
    rel="noopener noreferer">
    <Icon icon="{faTwitter}" color="#1DA1F2" />
  </a>
</main>
