<script>
  export let name;
  export let thumbnail;
  export let description;
  export let link;
</script>

<div class="flex p-4 m-2 bg-gray-100 rounded ">
  <div class="w-1/4">
    <img width="100px" class="rounded" alt="thumbnail for channel {name}" src={thumbnail} />
  </div>
  <div class="self-center flex-grow w-full px-4 text-xl">{description}</div>
  <div class="self-center m-2">
    <a
      class="p-2 text-white bg-red-600 rounded"
      href="{link}?sub_confirmation=1">
      Subscribe
    </a>
  </div>
</div>
