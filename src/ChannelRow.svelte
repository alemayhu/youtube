<script>
  export let name;
  export let thumbnail;
  export let description;
  export let link;
</script>

<div class="bg-gray-100 flex  m-2 rounded p-4">
  <div class="w-1/4">
    <img width="100px" class="rounded" alt="thumbnail for channel {name}" src={thumbnail} />
  </div>
  <div class="flex-grow self-center text-xl px-4 w-full">{description}</div>
  <div class="self-center m-2">
    <a
      class="bg-red-600 p-2 rounded text-white"
      href="{link}?sub_confirmation=1">
      Subscribe
    </a>
  </div>
</div>
