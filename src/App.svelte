<script>
  import ChannelRow from './ChannelRow.svelte';

  let data = [
    {
      name: 'Alexander Alemayhu',
      thumbnail: '/avatar/aa.jpeg',
      description: 'A personal channel where I share productivity stuff related to ⭐️ Anki and 🄽 Notion.',
      link: 'https://youtube.com/c/alexanderalemayhu'
    },
    {
      name: 'Japanese with Alexander',
      thumbnail: '/avatar/aa-jp.jpeg',
      description:
        'A place for me to document my journey learning Japanese and share what I learn with others.',
      link: 'https://www.youtube.com/channel/UCpqr_S8LyUfntQ3DXx96BdA'
    },
    {
      name: 'Alemayhu VODs',
      thumbnail: '/avatar/portrait_1.jpeg',
      description: 'Hour long exports from my Twitch channel 😊',
      link: 'https://www.youtube.com/c/AlemayhuVODS'
    }
  ];
</script>

<div class="flex flex-col w-full h-screen bg-blue-200">
  <div class="self-center py-4 align-center">
    <div class="flex flex-col justify-center">
      <img
        alt="Avatar of Alexander Alemayhu"
        class="self-center w-16 rounded-full"
        src="/avatar/portrait.png" />
    </div>
    <div class="py-2">
      <a class="text-white" href="https://twitter.com/aalemayhu">@aalemayhu</a>
    </div>
  </div>
  <div class="mx-2 text-center text-gray-700">
    <p>
      Below are links to my various YouTube channels, click on the red button to
      subscribe!
    </p>
  </div>
  <ul class="flex flex-col">
    {#each data as channel}
      <li class="self-center justify-center w-4/5 ">
        <ChannelRow {...channel} />
      </li>
    {/each}
  </ul>
</div>
