<script lang="ts">
  import type { IconDefinition } from '@fortawesome/fontawesome-common-types';

  export let icon: IconDefinition;
  export let color: string;
  let path: string;
  let classes = '';
  let viewBox = '';
  $: viewBox = '0 0 ' + icon.icon[0] + ' ' + icon.icon[1];
  $: classes = 'fa-svelte ' + ($$props.class ? $$props.class : '');
  $: path = icon.icon[4] as string;
</script>

<style>
  .fa-svelte {
    width: 1em;
    height: 1em;
    overflow: visible;
    display: inline-block;
    color: var(--color);
  }
</style>

<svg
  aria-hidden="true"
  style="--color:{color}"
  class="{classes}"
  role="img"
  xmlns="http://www.w3.org/2000/svg"
  viewBox="{viewBox}">
  <path fill="currentColor" d="{path}"></path>
</svg>
