<template>
  <div class="overflow-hidden bg-white border-2 rounded-lg shadow card border-neutral-200">
    <figure class="card__hd"><img src="/Image@2x.png" alt="Countryside-style living room"></figure>
    <div class="card__bd">
      <span class="text-sm text-green-700 rounded-full card__tag fill-green-50 outline outline-2 outline-green-200">Interior</span>
      <h1 class="text-lg font-semibold card__title text-neutral-900">Top 5 Liveing Room Inspirations</h1>
      <p class="text-base font-medium card__dec">Curated vibrants colors for your living, make it pop & calm in the same time.</p>
      <button class="text-indigo-700 card__btn" aria-label="Read more about top 5 liveing room inspirations."><span aria-hidden="true">Read more</span><svg aria-hidden="true" width="20" height="20" viewBox="0 0 20 20" fill="none" xmlns="http://www.w3.org/2000/svg">
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
