<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    
    .titulo-principal.color-acento-botones
      .titulo-principal__numero
        span 1
      h1 Métodos o funciones 

    .bloque-texto-g.color-primario.p-3.p-sm-4.p-md-5
      .bloque-texto-g__img(
        :style="{'background-image': `url(${require('@/assets/curso/tema1/img01.png')})`}"
      )
      .bloque-texto-g__texto.p-5
        p.mb-0 
        span.text-black De acuerdo con Gonzáles y Pelissier (2002),
        |los métodos o funciones permiten segmentar el trabajo que hace un programa en subtareas o tareas más pequeñas,enfocadas en un fin específico, y se pueden utilizar cuantas veces se necesite;estas están separadas del programa principal, pero aportan a su objetivo.
    <br>
    <br>     
    .col-lg-4
      .cajon.color-acento-botones.p-4.mb-4
        p El uso de funciones da la capacidad de agrupar varias instrucciones de código bajo un solo nombre, y con el nombre de la función, es posible invocarlo las veces que se necesite, permitiendo usar esta función las veces que sean necesarias.
    .div.row.mt-4.mb-4
      .div.col-md-6
        img(src='@/assets/curso/tema1/1.svg', alt='Texto que describa la imagen')
      .div.col-md-6
        .h2.titulo-tercero Ejemplo 1:
        p La funcion se define con la siguiente sintaxis.
        .div.cajon.color-secundario.p-4.mb-4
          div.h5 Nota:
          | el símbolo “//” quiere decir que no hace parte del código, se lo utiliza para hacer comentarios sobre el código, por lo cual se pone en color azul.
        .ol.lista-ol
          img(src='@/assets/curso/tema1/zz.png', alt='Texto que describa la imagen')  


    .div.row.mt-4.mb-4

      .div.col-md-6
        p La función arroja como resultados los números 8 y 400.
        p En el ejemplo anterior, se observa la sintaxis de una función que arroja la media aritmética de dos o más números, pero es necesario recordar qué es la media aritmética. Según Paz (s. f.), “La media aritmética o promedio simple se calcula sumando los valores de interés y dividiendo entre el número de valores sumados”. Para el anterior caso, se suman 2 números y el resultado se divide entre 2, así:
        .div.col-md-4.mb-10.mb-md-0
          img(src='@/assets/curso/tema1/mate.png', alt='Texto que describa la imagen')  
      .div.col-md-6
        img(src='@/assets/curso/tema1/2.svg', alt='Texto que describa la imagen')

    <br>
    .col-lg-4
      .cajon.color-acento-botones.p-4.mb-4
        p-span Los autores, además, dicen que estos tienen 3 tipos de visibilidad: 
        p-span.text-black Public “Pública”, Private “Privada”, o Protected “Protegidas” 
        | , si no se especifica, se sobreentiende que es privada.

</template>

<script>
export default {
  name: 'Tema1',
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
