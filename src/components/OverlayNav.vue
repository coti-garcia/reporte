<template>
  <b-navbar>
    <b-collapse
      class="default-nav justify-content-center"
      is-nav
      id="nav_collapse"
    >
      <b-navbar-nav class="navbar-nav d-block overlay-nav">
        <b-nav-item
          href="#presentacion"
          class="scroll"
          @click="toggleClass('removeClass', 'active')"
          ><span>Presentación</span></b-nav-item
        >
        <b-nav-item
          href="#cartas"
          class="scroll"
          @click="toggleClass('removeClass', 'active')"
          ><span>Cartas de presentación</span></b-nav-item
        >
        <b-nav-item
          href="#uc-devis-us"
          class="scroll"
          @click="toggleClass('removeClass', 'active')"
          ><span>UC Davis EE.UU</span></b-nav-item
        >
        <b-nav-item
          href="#relacion-historica"
          class="scroll"
          @click="toggleClass('removeClass', 'active')"
          ><span>Relación histórica</span></b-nav-item
        >
        <b-nav-item
          href="#uc-davis-chile"
          class="scroll"
          @click="toggleClass('removeClass', 'active')"
          ><span>UC Davis Chile</span></b-nav-item
        >
        <b-nav-item
          href="#mision"
          class="scroll"
          @click="toggleClass('removeClass', 'active')"
          ><span>Nuestra misión</span></b-nav-item
        >
        <b-nav-item
          href="#impacto"
          class="scroll"
          @click="toggleClass('removeClass', 'active')"
          ><span>Impacto</span></b-nav-item
        >
        <b-nav-item
          href="#quienes-somos"
          class="scroll"
          @click="toggleClass('removeClass', 'active')"
          ><span>Quiénes somos</span></b-nav-item
        >
        <b-nav-item
          href="#areas-trabajo"
          class="scroll"
          @click="toggleClass('removeClass', 'active')"
          ><span>Áreas de trabajo UC Davis Chile</span>
        </b-nav-item>
        <b-nav-item
          href="#alianzas"
          class="scroll"
          @click="toggleClass('removeClass', 'active')"
          ><span>Principales alianzas</span>
        </b-nav-item>
        <b-nav-item
          href="#proyectos"
          class="scroll"
          @click="toggleClass('removeClass', 'active')"
          ><span>Listado de principales proyectos</span>
        </b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {
  name: "OverlayNav",
  methods: {
    // offcanvas searchbox
    toggleClass(addRemoveClass, className) {
      const el = document.querySelector("#overlay-menu");
      if (addRemoveClass === "addClass") {
        el.classList.add(className);
      } else {
        el.classList.remove(className);
      }
    },
  },
};
</script>