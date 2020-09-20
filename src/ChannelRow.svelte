<script>
  export let name;
  export let thumbnail;
  export let description;
  export let link;
</script>

<div class="flex items-center p-4 m-2 bg-gray-100 rounded sm:items-start">
  <div class="w-1/4">
    <a href="{link}"><img width="100px" class="rounded" alt="thumbnail for channel {name}" src={thumbnail} /></a>
  </div>
  <div class="self-center flex-grow w-full p-4 text-xs sm:text-xl sm:p-2">{description}</div>
  <div class="self-center m-2">
    <a
      class="p-2 text-white bg-red-600 rounded hover:bg-red-900"
      href="{link}?sub_confirmation=1">
      Subscribe
    </a>
  </div>
</div>
