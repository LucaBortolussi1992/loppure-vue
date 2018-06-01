<template>
  <div class="card">
    <div class="card-content">
      <div class="media">
        <div class="media-left">
          <figure class="image is-48x48">
            <img :src="LogoPausa" alt="Placeholder image" style="width: 50px">
          </figure>
        </div>
        <div class="media-content">
          <p class="title is-4">L’alcol dell’anima</p>
          <p class="subtitle is-6">Pausa caffè</p>
        </div>
      </div>

      <div class="content">
        Un mattino, una ragazza di nome Andrea mi ha detto «Ho letto da qualche parte che la notte è l’alcool dell’anima. Inibisce le nostre protezioni. Come se dall’altra parte la luce del giorno, invece che mostrare, nascondesse solamente. Una grandissima bugia. Mi capisci?». Non ricordo cosa ho risposto, ma di certo devo aver pensato di comprenderla. […]
      </div>
    </div>

    <div class="card-image">
      <figure class="image">
        <img src="http://www.loppure.it/wp-content/uploads/2018/05/Notte-stellata--600x338.jpg" alt="Placeholder image">
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
  .card {
    border-radius: 8px;
    overflow: hidden;
    transition: all 0.3s cubic-bezier(.25,.8,.25,1);

    &:hover {
    box-shadow: 0 14px 28px rgba(0,0,0,0.25), 0 10px 10px rgba(0,0,0,0.22);
     }
  }
</style>
