<script>
import { fade } from 'svelte/transition';
import StartRating from './StartRating.svelte';

  export let name;
  export let id;
  export let expreance;
  export let rating;
  export let url;
  export let description;
</script>

<style lang="scss">
 @import '../../../static/scss/mixin.scss';
 @import '../../../static/scss/_text.scss';

 .padding-bottom{
   padding-bottom:29px;
 }
  .box-shadow{
    @include shadow;
    @include border;
}


.card-body{
  .w-100{
   @include width;
  }

}

  .light-overlay,
  .dark-overlay,
  .gradient-overlay {
    position: relative;
    overflow: hidden;
  }
  .overflow-hidden {
    overflow: hidden !important;
  }

  .card-img,
  .card-img-top {
    border-top-left-radius: calc(0.4rem - 1px);
    border-top-right-radius: calc(0.4rem - 1px);
  }

  .img-fluid {
    max-width: 100%;
    height: auto;
  }
  .tile-link {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    cursor: pointer;
    z-index: 30;
  }
  .card-img-overlay-bottom {
    position: absolute;
    right: 1.25rem;
    bottom: 0.75rem;
    left: 1.25rem;
  }
  .z-index-20 {
    z-index: $z-index-20;
  }
  .text-sm {
    font-size: 0.875rem;
  }

  .align-items-center {
    -ms-flex-align: center !important;
    align-items: center !important;
  }
  .avatar.avatar-border-white {
    border: solid 2px #fff;
  }
  .avatar {
  @include avatar-layout;
  }
  .mr-2,
  .mx-2 {
    margin-right: 0.5rem !important;
  }
  .media-body {
    -ms-flex: 1;
    flex: 1;
  }
  .card-img-overlay-top {
    position: absolute;
    top: 0.75rem;
    right: 1.25rem;
    left: 1.25rem;
  }
  .text-right {
    text-align: right !important;
  }
  .card-fav-icon {
    display: inline-block;
    width: 2.5rem;
    height: 2.5rem;
    text-align: center;
    opacity: 0.5;
    color: #fff;
    border-radius: 50%;
    background: #343a40;
    line-height: 2.5rem;
  }
  .d-flex {
    display: flex !important;
}
  .z-index-40 {
    z-index: $z-index-40;
  }
  .card-fav-icon svg {
    vertical-align: middle;
    opacity: 1;
    stroke-width: 5;
  }
  .svg-icon {
    width: 18px;
    height: 18px;
    vertical-align: text-bottom;
    stroke: currentColor;
    stroke-width: 3;
    --layer1: currentColor;
    --layer2: currentColor;
  }
  .text-white {
    color: $lightest-gray !important;
  }

  svg {
    overflow: hidden;
    vertical-align: middle;
  }

.mb-3, .my-3 {
    margin-bottom: 1rem !important;
}

.text-sm {
    font-size: .875rem;
}

.mb-0, .my-0 {
    margin-bottom: 0 !important;
}
.flex-grow-1 {
    -ms-flex-positive: 1 !important;
    flex-grow: 1 !important;
}
.text-xs {
    font-size: .7rem;
}
.card-stars {
    min-width: 65px;
    margin-top: 2px;
}
.text-right {
    text-align: right !important;
}

.card-text:last-child {
    margin-bottom: 0;
}
.text-muted {
    color: #868e96 !important;
}

.md-3, .my-3 {
    margin-bottom: 12px !important;
}
</style>

<div class="col padding-bottom">
  <div class="card box-shadow" style="width: 240px; margin-right: 20px;">

    <div class="card-img-top overflow-hidden gradient-overlay">
      <img
        class="img-fluid"
        src="{url}"
        alt="Modern, Well-Appointed Room" />
      <a class="tile-link" href="detail-rooms.html" />
      <div class="card-img-overlay-bottom z-index-20">
        <div class="media text-white text-sm align-items-center">
          <img
            class="avatar avatar-border-white mr-2"
            src="https://d19m59y37dris4.cloudfront.net/directory/1-5/img/avatar/avatar-0.jpg"
            alt="Pamela" />
          <div class="media-body">Pamela</div>
        </div>
      </div>
      <div class="card-img-overlay-top text-right">
        <a
          class="card-fav-icon position-relative z-index-40"
          href="javascript: void();">
          <svg class="svg-icon text-white">
            <use xlink:href="#heart-1">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                viewBox="0 0 64 64"
                id="heart-1">
                <title>Heart</title>
                <desc>A line styled icon from Orion Icon Library.</desc>
                <path
                  data-name="layer1"
                  d="M47 5c-6.5 0-12.9 4.2-15 10-2.1-5.8-8.5-10-15-10A15 15 0 0
                  0 2 20c0 13 11 26 30 39 19-13 30-26 30-39A15 15 0 0 0 47 5z"
                  fill="none"
                  stroke="#101010"
                  stroke-miterlimit="10"
                  stroke-linejoin="round"
                  stroke-linecap="round"
                  style="stroke:var(--layer1, #101010)" />
              </svg>
            </use>
          </svg>
        </a>
      </div>
    </div>

    <div class="card-body">
      <!-- <h5 class="card-title">{name}</h5>
      <p class="card-text">{description}</p>
      <a href="#" class="btn btn-primary">{expreance}</a> -->
      <div class="w-100">
      <h6 class="card-title">
       <span transition:fade class="text--large-1--dark--bold">{name}</span>
      </h6>
      <div class="card-subtitle d-flex md-3" >
      <p class="flex-grow-1 mb-0  text--large--normaldark--normal">asdas</p>
      <p class="flex-shrink-1 mb-0 card-stars text-xs text-right">
      {#each Array(rating) as _ , i}
       <StartRating/>
      {/each}
      </div>
      <p class="card-text text-muted">
      <span class="h4 text-primary">{expreance}</span> Year Expreance</p>
      </div>
    </div>
  </div>
</div>
