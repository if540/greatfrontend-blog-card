<template>
    <div class="card bg-white border-neutral-200 border-2 shadow overflow-hidden rounded-lg">
      <div class="card__hd"><img src="/Image@2x.png" alt="田園風格客廳"></div>
      <div class="card__bd">
        <div class="card__tag text-sm text-green-700 fill-green-50 outline outline-2 outline-green-200 rounded-full">Interior</div>
        <h1 class="card__title text-lg text-neutral-900 font-semibold">Top 5 Liveing Room Inspirations</h1>
        <p class="card__dec text-base font-medium">Curated vibrants colors for your living, make it pop & calm in the same time.</p>
        <button class="card__btn text-indigo-700" ><span>Read more</span><svg width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M13.4763 9.16658L9.00634 4.69658L10.1848 3.51807L16.6667 9.99992L10.1848 16.4817L9.00634 15.3032L13.4763 10.8332H3.33334V9.16658H13.4763Z" fill="#4338CA"/>
          </svg>
        </button>
      </div>
    </div>
</template>

<style lang="scss">
.card {
  max-width: 340px;
  margin: 0 auto;
  font-family: 'Noto Sans', Arial, Helvetica, sans-serif;

  // structure
  &__hd {
    overflow: hidden;
  }
  &__bd {
    display: flex;
    flex-direction: column;
    align-items: stretch;
    padding: 24px 16px;
  }

  // component
  &__tag {
    align-self: flex-start;
    padding: 2px 8px;
  }
  &__title {
    margin-top: 8px;
  }
  &__dec {
    margin-top: 12px;
    margin-bottom: 24px;
  }
  &__btn {
    display: flex;
    align-items: center;
    align-self: flex-start;
    padding: 0 6px;
    gap: 8px;
    box-shadow: 0px 0px 0px 4px transparent;
    border-radius: 4px;
    transition: box-shadow .5s;
    &:hover {
      color: #3730A3;
    }
    &:focus:not(:disabled) {
      box-shadow: 0px 0px 0px 4px rgba(68, 76, 231, 0.12);
    }
    &:disabled {
      color: #A3A3A3;
      svg path {
        fill: #A3A3A3;
      }
    }
  }
}
</style>
