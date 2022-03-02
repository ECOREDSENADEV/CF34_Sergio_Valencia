<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    
    .titulo-principal.color-acento-botones
      .titulo-principal__numero
        span 2
      h1 Clases y objetos  
    .div.row.mt-5.mb-1
      .div.col-4
        img(src='@/assets/curso/tema2/1.png', alt='Texto que describa la imagen')
        <br>
      .div.col-8.mt-4
        .div.row
          .div.col-11
            .div.cajon.mb-4.mt-4
              p Las clases son contenedores de información basados en atributos y en métodos de construcción, los cuales pueden modificar y consultar; son suficientes para representar objetos con los cuales se procesa información, y se usan para hacer objetos que tienen un mismo comportamiento, estado e identidad.
        <br>
        .div.col-md-11
          .h2.titulo-tercero Ejemplo 2:
          p Se tiene una clase “personas” (Mario, Margarita y Alejandro), donde el comportamiento de las personas es leer, trabajar, jugar, etc.; pueden estar en estado despierto o dormido; sus propiedades pueden ser color de ojos, género, estado civil, etc.
          p Su sintaxis sería así:
          <br>
          p.mb-0 class Persona { 
          p.mb-0 # Propiedades 
          p.mb-0 # Métodos 
          p }
        div.row.mb-2
          div.col-md-2.p-0
            img(src='@/assets/curso/tema2/2.png', alt='Texto que describa la imagen')
          .div.col-md-9
            <br>
            <br>
            p.mb-3 <strong>Objeto:</strong> el objeto es una instancia de una clase, la cual puede crear varias instancias de la misma clase.
            p.mb-3 <strong>Ejemplo:</strong> existe una sola clase “Persona”, pero muchos objetos de tipo persona pueden ser instancias de esta clase.
    <br>
    <br>
        h2.text-center.mb-0 A continuación, observe la diferencia entre 
        h2.text-center clases y objetos con una analogía:
        <br>
        
    #MapaGroup01.row.justify-content-center.p-4.mb-4
      .col-lg-3.col-sm-4.mb-4
        button.buttom.color-primario.p-3.w-100.position-relative(data-bs-toggle='collapse' data-bs-target='.multi-collapse1' aria-expanded='true' aria-controls='.multi-collapse1')
          .row.justify-content-center
            .col-lg-8.col-sm-6.mb-4
              img(src='@/assets/curso/tema2/b1.png')
      .col-lg-3.col-sm-4.mb-4
        button.buttom.color-primario.p-3.w-100.position-relative(data-bs-toggle='collapse' data-bs-target='.multi-collapse2' aria-expanded='true' aria-controls='.multi-collapse2')
          .row.justify-content-center
            .col-lg-8.col-sm-6.mb-4
              img(src='@/assets/curso/tema2/b2.png')

      .col-lg-3.col-sm-4.mb-4
        button.buttom.color-primario.p-3.w-100.position-relative(data-bs-toggle='collapse' data-bs-target='.multi-collapse3' aria-expanded='true' aria-controls='.multi-collapse3')
          .row.justify-content-center
            .col-lg-8.col-sm-6.mb-4
              img(src='@/assets/curso/tema2/b3.png')      

      .col-lg-12.position-relative
        .multi-collapse1.collapse.show(data-bs-parent='#MapaGroup01')
          .col-md-2.mb-4
            h2.BG2 Analogía
          img(src='@/assets/curso/tema2/6.png', alt='Texto que describa la imagen')
      
        .multi-collapse2.collapse(data-bs-parent='#MapaGroup01')
          .row
            .col-md-7.mb-4.mb-md-0
              .col-md-2.mb-4
                h2.BG2 Ejemplo
              p En el siguiente ejemplo, se observará el código de un objeto. 
              p El símbolo “//” quiere decir que no hace parte del código, se lo utiliza para hacer comentarios sobre el código, por lo cual, se pone en color azul.
              .col-md-7.mb-4.mb-md-0
                img(src='@/assets/curso/tema2/42.png', alt='Texto que describa la imagen')
            .col-md-5
              figure
                img(src='@/assets/curso/tema2/41.png', alt='Texto que describa la imagen')
        .multi-collapse3.collapse(data-bs-parent='#MapaGroup01')
          .col-md-2.mb-4
            h2.BG2 Resultado
          p Si se corriera el código, daría este resultado.
          <br>
              img(src='@/assets/curso/tema2/8.png', alt='Texto que describa la imagen')


</template>

<script>
export default {
  name: 'Tema2',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
