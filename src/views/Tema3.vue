<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    
    .titulo-principal.color-acento-botones
      .titulo-principal__numero
        span 3
      h1 Integración de aplicaciones (XML, SOAP, WSDL y UDDI)

    .div.row.mt-5.mb-1
      .div.col-5.mb-4
        img(src='@/assets/curso/tema3/1.png', alt='Texto que describa la imagen')
      .div.col-7.mt-4
        .div.row
          .div.col-11
            .div.cajon.mb-4.mt-4
              p Los servicios web permiten la nueva generación de aplicaciones basadas en Internet. Estos servicios admiten la comunicación de Internet de aplicación a aplicación, es decir, las aplicaciones en diferentes ubicaciones de la red se pueden integrar para funcionar como si fueran parte de un único sistema de software grande. Ejemplos de aplicaciones que los servicios web hacen posibles incluyen transacciones comerciales automatizadas y acceso directo (sin navegador) a dispositivos de escritorio y de mano, a las reservas, el comercio de acciones y los sistemas de seguimiento de pedidos.
        .div.col-md-11.mt-4
          p Han surgido varios estándares clave que, juntos, forman la base de los servicios web: XML (Extensible Markup Language), WSDL (Web Services Definition Language), SOAP (Simple Object Access Protocol) y UDDI (Universal Description, Discovery, and Integration). Además, se ha especificado ebXML (Electronic Business XML) para facilitar la integración automatizada de procesos comerciales entre socios comerciales.
     
    #t_3_1.titulo-segundo.mb-4.mt-4
      .h4 3.1 XML "Extensible Markup Language") 
    .div.row.mt-4.mb-4
      .div.col-3
        img(src='@/assets/curso/tema3/2.svg', alt='Texto que describa la imagen')
      .div.col-lg-9.BG03
        .div.row
          .div.col-1
            img(src='@/assets/curso/tema3/3.png', alt='Texto que describa la imagen')
        .div.row
          .div.col-1
          .div.col-10
            p.mb-2.mt-2.ms-5.text-white XML (Extensible Markup Language) es un lenguaje de marcas que define un conjunto de reglas para la codificación de documentos, se utiliza para estructurar información en cualquier fichero que contenga texto y es muy usado en el medio, debido a que es un estándar abierto y libre, creado por el consorcio World Wide Web, W3C. 
            <br>
        .div.row
          .div.col-9
          .div.col-3
            h4.text-white Según Bianco (2005)
    .div.row.mt-4
      .div.col-7.mt-4
        p Además, argumenta que el lenguaje XML proporciona una estructura para definir elementos, crear un formato y generar un lenguaje personalizado. Estos archivos están conformados en dos partes prolog y body:
        .div.row
          .div.col-6.mt-5
            img(src='@/assets/curso/tema3/4.png', alt='Texto que describa la imagen')
          .div.col-6.mt-5
            img(src='@/assets/curso/tema3/6.png', alt='Texto que describa la imagen')

      .div.col-5
        img(src='@/assets/curso/tema3/5.png', alt='Texto que describa la imagen')
    .div.col-12
      .cajon.color-acento-botones.p-4.mb-4.mt-4
        p El XML es de simple uso, por lo cual se utiliza para varios servicios web, haciendo posible una forma independiente de almacenar datos para que puedan ser compartidos por diferentes aplicaciones, logrando una óptima compatibilidad entre dispositivos.
    h3 <strong>Estructura</strong>
    .div.row.BG5
      .div.col-5
        img(src='@/assets/curso/tema3/7.png', alt='Texto que describa la imagen')
      .div.col-7.mt-4
        .div.row
          .div.col-11
            .div.cajon.mb-4.mt-4
              p El mismo autor afirma que el Prólogo va en la primera línea de código, aquí se declara que el documento es XML y qué versión se está utilizando. Vea el siguiente ejemplo: 
          h3.mt-4 Ejemplo 3:
          .div.row.mb-2
            .div.col-12
              .div.row-11.p-1.bg3
                p.mb-4.mt-4 <strong>?xml version=“1.0”?></strong> “Declaración normal, sirve para cualquier documento, solo especifica la versión”
          .div.row.mb-4
            .div.col-12              
              .div.row-11.p-1.bg3                
                p.mb-4.mt-4 <strong>?xml versión= “1.0” encoding= “ISO-8859-1” standalone= “yes”?></strong> “Aquí está la versión y también se agrega el tipo de codificación y el Standalone, que se refiere a que es un documento autónomo”
          p.mb-2 En el cuerpo es donde va la programación. Hay que tener en cuenta un elemento principal llamado raíz, dentro del cual se encuentran el resto de los elementos. Este elemento es el “padre” de todos los demás elementos, y de él se derivan las ramas del árbol hasta el nivel más bajo.
          p Hay que tener en cuenta que XML es muy diferente de HTML, por ejemplo: 


</template>

<script>
export default {
  name: 'Tema3',
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
