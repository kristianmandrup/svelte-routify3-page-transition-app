<script>
  export let item;
  export let href;

  import Icon from "./Icon.svelte";
</script>

<li class="p-3 hover:bg-slate-100 hover:text-slate-900">
  <a {href} class="flex items-center">
    <Icon src={item.image} name={item.name} />
    <div class="text-xl" style:--transition-tag="h-{item.name}">
      {item.name}
    </div>
  </a>
</li>
