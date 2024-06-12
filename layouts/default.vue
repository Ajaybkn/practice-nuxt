<template>
  <div>
    <header>
      <nav>
        <NuxtLink to="/">
          Go TO Home
          <ul>
            <li>
              <NuxtLink to="/"> Home </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/about"> About </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/products"> Products </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/feedback"> Feedback </NuxtLink>
            </li>
          </ul>
        </NuxtLink>
      </nav>
    </header>
    <div>
      <slot />
    </div>
  </div>
</template>
<style>
.router-link-exact-active {
  color: red;
}
</style>
