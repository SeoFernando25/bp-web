<script>
  import NewsLetterSignup from "$lib/components/NewsLetterSignup.svelte";
</script>

<img alt="" class="bb-img" src="bg.png" />

<div class="p-4">
  <div
    class="main-title text-4xl sm:text-4xl md:text-4xl lg:text-5xl xl:text-6xl "
  >
    Stop wasting hours trying to buy brick by brick! We automate it for you.
  </div>

  <div
    class="main-subtitle text-xl sm:text-2xl md:text-2xl lg:text-3xl xl:text-3xl pt-4 sm:pt-6 md:pt-8 lg:pt-10 xl:pt-12"
  >
    Bulk buy lego pieces straight from Lego <nobr>Pick-A-Brick</nobr> store!
  </div>
</div>

<div class="grid place-content-center items-center m-4">
  <NewsLetterSignup />
</div>

<div class="grid place-content-center items-center">
  <video
    playsinline
    controls
    class="w-screen lg:m-12 lg:w-[50vw]"
    poster="thumb.png"
  >
    <track kind="captions" />
    <source src="video.mp4" type="video/mp4" />
    Your browser does not support the video tag.
  </video>
</div>

<section class="moc-section flex place-content-center flex-col gap-4 pt-12">
  <div
    class="text-center font-bold text-xl sm:text-2xl md:text-2xl lg:text-3xl xl:text-3xl text-green-500"
  >
    MOC Gallery.
  </div>

  <div class="text-center font-extrabold text-2xl lg:text-5xl text-black">
    No more wasting time on buying bricks, more time building your MOC
    Collection.
  </div>

  <div class="p-8 grid grid-cols-2 lg:grid-cols-4 gap-16 items-center img-grid">
    <img src="https://pagemaker.b-cdn.net/media/66285/1792x1792.webp" />
    <img src="https://pagemaker.b-cdn.net/media/66286/1000x1000.png" />
    <img src="https://pagemaker.b-cdn.net/media/66300/980x691.webp" />
    <img src="https://pagemaker.b-cdn.net/media/66301/1498x1000.webp" />
    <img src="https://pagemaker.b-cdn.net/media/66302/1510x1000.webp" />
    <img src="https://pagemaker.b-cdn.net/media/66304/1000x1000.webp" />
    <img src="https://pagemaker.b-cdn.net/media/66305/1498x1000.webp" />
    <img src="https://pagemaker.b-cdn.net/media/66306/1500x998.webp" />
  </div>
</section>

<style>
  /* Main title centered bold extra large */
  .main-title {
    @apply text-center font-bold;
    max-width: 1280px;
    margin: 0 auto;
    hyphens: none;
    word-break: keep-all;
  }

  .main-subtitle {
    @apply text-center font-bold;
    max-width: 1280px;
    margin: 0 auto;
    hyphens: none;
    word-break: keep-all;
  }

  /* video {
    border-top: 1px solid #797f8c;
    border-bottom: 1px solid #797f8c;
  } */

  .bb-img {
    position: absolute;
    z-index: -1;
    opacity: 0.2;
    transform: translate(-10%, 10%);
    left: 0;
    top: 0;
    user-select: none;
    width: 50vh;
  }

  .moc-section {
    background: whitesmoke;
    min-height: 10rem;
  }

  /* .img-grid > img have same aspec ratio and size */
  .img-grid > img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
</style>
