<template>
  <div class="card columns">
    <div class="card-content column is-three-fifths">
      <div class="media">
        <div class="media-left">
          <figure class="image is-1by1">
            <img :src="LogoPausa" alt="Placeholder image">
          </figure>
        </div>
        <div class="media-content">
          <h1 class="title is-1">L’alcol <br>dell’anima</h1>
          <div class="content">
            Un mattino, una ragazza di nome Andrea mi ha detto «Ho letto da qualche parte che la notte è l’alcool dell’anima. Inibisce le nostre protezioni. Come se dall’altra parte la luce del giorno, invece che mostrare, nascondesse solamente. Una grandissima bugia. Mi capisci?». Non ricordo cosa ho risposto, ma di certo devo aver pensato di comprenderla. […]
          </div>
        </div>
        <div class="media-right">
          <p class="subtitle is-6">Pausa caffè  |  12/02/2018</p>
        </div>
        <div class="media-bottom">
          <p class="subtitle is-6">Pordenone</p>
        </div>
      </div>
    </div>

    <div class="card-image column is-two-fifths">
      <figure>
        <img src="http://www.loppure.it/wp-content/uploads/2018/05/margaret-atwood-600x300.jpg" alt="Placeholder image">
      </figure>
    </div>
  </div>
</template>

<script>
  import LogoPausa from '../../assets/logos_category/loppure-pausa-caffe.svg';

  export default {
    name: 'Card',
    data() {
      return {
        LogoPausa
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "../../style/variables";

  .card {
    margin-left: 0;
    margin-right: 0;
    padding: 2rem;
    border-radius: 3px;
    overflow: hidden;
    transition: all 0.3s cubic-bezier(.25,.8,.25,1);
    box-shadow: none;

    &:hover {
    box-shadow: 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22);
     }

    &-content {
      padding: 0;

      & .content {
        column-count: 2;
      }
    }

    &-image {
      padding: 0;
      transition: all .8s ease-in-out;
      &:hover {
        width: 100%;
        transform: translateX(calc(-50% - 2rem));
        padding-right: 4rem;
        margin-right: 6rem;
      }

      & figure {
        height: 100%;
      }
      & img {
        width: auto;
        height: 100%;
        object-fit: cover;
        /*object-position: 0 0;*/
      }
    }
  }

  .media {
    position: relative;

    &-left {
      position: absolute;
      top: 0;
      left: 0;
      width: 3rem;
      padding: 0.5rem;
      background-color: $faded-brown;
      border-radius: 50%;
      overflow: hidden;
      transition: transform 0.5s ease-in-out;
      &:hover {
        transform: scale(1.5);
      }
    }

    &-right {
      position: absolute;
      top: 0;
      right: 2rem;
      & p {
        color: $grey-light;
      }
    }

    &-bottom {
      position: absolute;
      bottom: 0;
      left: 0;
      transform: rotate(-90deg);
      transform-origin: left top;
      & p {
        color: $grey-light;
      }
    }

    &-content {
      padding: 6rem 4rem 0rem 6rem;

      & h1 {
        font-family: $family-serif;
        padding-bottom: 2rem;
      }
    }
  }
</style>
