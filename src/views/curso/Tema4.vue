<template lang="pug">
.curso-main-container.pb-3
  BannerInterno(:subTitulo="'4. Relación entre desarrollo económico, equidad social y protección ambiental     '")
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    .row.mb-4
      .col-12.col-lg-7(data-aos="fade-right")
        span Reducir las desigualdades dentro de los países y entre ellos, es fundamental para el desarrollo sostenible. Este objetivo promueve políticas inclusivas que aseguren que todas las personas, independientemente de u raza, género, etnia, situación económica o discapacidad, tengan las mismas oportunidades de acceso a recursos y servicios. Aunque el crecimiento económico ha mejorado el nivel de vida en muchas regiones, la desigualdad económica ha aumentado, lo que genera exclusión y tensiones sociales. Este objetivo aboga por medidas que promuevan la inclusión financiera, la equidad en el acceso a la educación y la salud, y la reducción de las barreras para la movilidad social y económica.
      .col-5.d-none.d-lg-block(data-aos="fade-left")
        img.h-100(src='@/assets/curso/unidad/img-31.png', alt='Texto que describa la imagen')

    .row.bg-amarillo.bg-full-width.py-4.mb-5
      div.px-5.pb-md-3.py-4.d-flex
        .d-none.d-xl-block.col-xl-5.mx-auto.mt-4.mt-xl-0(data-aos="fade-left")
          img.h-100(src='@/assets/curso/unidad/img-32.png', alt='Texto que describa la imagen')
        .col-12.col-xl-7.d-flex.ps-4.ps-xl-5.align-items-center.flex-column(data-aos="fade-right")
          h2.mb-4.pb-2.me-auto Desarrollo económico - Equidad social - Protección ambiental
          p.mb-5 El desarrollo sostenible se fundamenta en el equilibrio entre tres pilares esenciales: el desarrollo económico, la equidad social y la protección ambiental. Estos elementos, lejos de actuar de manera independiente, están intrínsecamente conectados, y su interacción define la posibilidad de construir un futuro sostenible. Mientras que el desarrollo económico genera oportunidades y mejora la calidad de vida, su impacto puede ser perjudicial si no se gestiona con responsabilidad, afectando tanto al medio ambiente como a la justicia social. En el PDF Desarrollo económico - Equidad social - Protección ambiental,  exploraremos cómo estas tres dimensiones interactúan, destacando la importancia de políticas y prácticas que maximicen sus sinergias, para lograr un progreso inclusivo y respetuoso con los límites del planeta.
          a.d-flex.me-auto.w-fit.bg-white.box-shadow.cursor-pointer(data-aos="zoom-in" :href="obtenerLink('/downloads/Anexos_Relación entre desarrollo económico, equidad social y protección ambiental.pdf')" target="_blank")
            img.h-100(style="width: 48px" src='@/assets/componentes/pdf-icon-square.svg', alt='Texto que describa la imagen')
            p.text-small.fs-14px.my-auto.px-2 <strong>Anexo.</strong> Desarrollo económico - Equidad social - Protección ambiental
             
    .bg-full-width.border-top-9-azul
      .px-4.px-md-5.pt-5.pb-0
        h2 Material complementario
        .row
          .col-12.col-md-6.col-lg-8
            p.text-small
            p.d-flex.my-4
              img.me-3.mb-auto.mt-1(src='@/assets/componentes/book.svg' :style="{'max-width':'16px'}")
              a.text-small.text-primary(target="_blank", href="https://elibro.net/es/lc/tecnologicadeloriente/titulos/41035") González Parodi, G. A. (2012). Reflexiones del desarrollo local sostenible: ( ed.). Ediciones y Gráficos Eón. 
            p.d-flex.my-4
              img.me-3.mb-auto.mt-1(src='@/assets/componentes/book.svg' :style="{'max-width':'16px'}")
              a.text-small.text-primary(target="_blank", href="https://elibro.net/es/lc/tecnologicadeloriente/titulos/68547") Vásquez, Y. & Petersen, J. (2017). Ensayos para un modelo de desarrollo sostenible: un cambio estructural: ( ed.). CLACSO.
          .col-12.col-md-6.col-lg-3
            figure
              img(src='@/assets/componentes/material-complementario.svg', alt='Texto que describa la imagen')


    .bg-full-width.border-top.actividad(style='background-color: #ebf1f5; border-top: 5px solid #f5c145 !important')
      .p-4.p-md-5
        #Actividad
          <Actividad :cuestionario='cuestionario'/>
</template>

<script>
import BannerInterno from '../../components/plantilla/BannerInterno'
export default {
  name: 'Tema4',
  components: {
    BannerInterno,
  },
  data: () => ({
    cuestionario: {
      tema: 'Desarrollo Sostenible - Unidad 1',
      titulo: 'Ponte a prueba',
      introduccion:
        'Demuestra lo que aprendiste en esta unidad y pon a prueba tus conocimientos.',
      barajarPreguntas: true,
      preguntas: [
        {
          id: 1,
          texto:
            '¿Qué relación existe entre el concepto de equidad social y el desarrollo sostenible?',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'La equidad social es un pilar del desarrollo sostenible, esencial para garantizar justicia e inclusión.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'La equidad social se centra exclusivamente en garantizar derechos económicos.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'La equidad social se refiere únicamente a la igualdad de género.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'No existe una relación directa entre ambos conceptos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 2,
          texto: '¿Qué distingue la sustentabilidad de la sostenibilidad?',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'La sustentabilidad es un enfoque más operativo centrado en recursos naturales.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'La sostenibilidad excluye el desarrollo económico.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'La sustentabilidad se limita a acciones individuales y la sostenibilidad a acciones globales.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'No hay diferencias entre ambos términos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 3,
          texto:
            '¿Qué implica el principio de responsabilidad global y local en el desarrollo sostenible?',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Adoptar acciones exclusivamente globales para la sostenibilidad.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Reconocer que la sostenibilidad es responsabilidad de los gobiernos nacionales.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Coordinar acciones locales y globales para enfrentar desafíos sostenibles.',
              esCorrecta: true,
            },
            {
              id: 'd',
              texto:
                'Enfocarse en las soluciones locales sin considerar el impacto global.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 4,
          texto:
            '¿Qué diferencia el desarrollo sostenible de otros modelos de desarrollo económico?',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Su enfoque exclusivo en el crecimiento económico.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto:
                'Su integración de equidad social y protección ambiental con el crecimiento económico.',
              esCorrecta: true,
            },
            {
              id: 'c',
              texto: 'Su limitación al contexto nacional.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Su rechazo al progreso tecnológico.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
        {
          id: 5,
          texto:
            '¿Qué importancia tiene el Informe Brundtland para el concepto de desarrollo sostenible?',
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Introdujo la noción de "necesidades esenciales" y límites ambientales.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto:
                'Rechazó la integración de la equidad social en el desarrollo.',
              esCorrecta: false,
            },
            {
              id: 'c',
              texto:
                'Propuso que solo los países desarrollados adoptaran la sostenibilidad.',
              esCorrecta: false,
            },
            {
              id: 'd',
              texto: 'Se centró únicamente en problemas ambientales.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto: '¡Muy bien! Ha acertado la respuesta.',
          mensaje_incorrecto: 'Lo sentimos, su respuesta no es la correcta.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
}
</script>

<style lang="sass">
.material-complementario
  padding-top: 3rem
  border-top: 9px solid $color-sistema-e
</style>
