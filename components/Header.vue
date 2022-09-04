<template>
  <header>
    <NuxtLink to="/"><img src="" alt="logo" /></NuxtLink>
    <nav>
      <ul>
        <li>
          <NuxtLink to="/nosotros">Nosotros</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/nosotros">Donaciones & Actividades</NuxtLink>
        </li>
        <li>
          <NuxtLink to="/nosotros">Contacto</NuxtLink>
        </li>
        <li>
          <Donate />
        </li>
      </ul>
    </nav>
  </header>
</template>

<style scoped>
header {
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 60;
  background-color: white;
}
</style>
