<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="fas fa-sitemap" titulo="Síntesis")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
      p A continuación, se presenta una síntesis de la temática estudiada en el componente formativo. 
      .row.justify-content-center
        .col-lg-10.mb-5.bgs.p-4.brad
          figure
            img(src="@/assets/curso/sintesis.svg", alt="Síntesis  sobre la formulación de alimento balanceado en aves, organizado en siete áreas principales: fisiología digestiva en aves granívoras, requerimientos nutricionales y plan alimentario, materias primas para la alimentación avícola, formulación de raciones balanceadas, elaboración del alimento balanceado, control de calidad e inocuidad, y bienestar animal y normativa. Cada área incluye los componentes, procesos y criterios necesarios para el diseño, producción, evaluación y cumplimiento de estándares en la fabricación de alimentos destinados a la nutrición avícola.")
        .col-auto
          a.anexo.mb-5(:href="obtenerLink('/downloads/Sintesis.pdf')" target="_blank")
            .anexo__icono
              img(src="@/assets/bullets/icono-pdf.svg")
            .anexo__texto
              p Anexo. Síntesis

</template>

<script>
export default {
  name: 'Sintesis',
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
