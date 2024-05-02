<template>
    <header class="top-0 bg-white z-10 p-0.5">
      <nav class="py-2 px-4">
        <div class="container mx-auto px-4 flex justify-between items-center">
          <div class="flex items-center">
            <MyHeaderAppLogo />
          </div>
          <div class="menu">
            <MyHeaderGuestMenu />
          </div>
        </div>
      </nav>
    </header>
  </template>

<style scoped>
@media (min-width: 544px) {
  .container {
    max-width: 576px;
  }
}

@media (min-width: 768px) {
  .container {
    max-width: 720px;
  }
}

@media (min-width: 992px) {
  .container {
    max-width: 940px;
  }
}

@media (min-width: 1200px) {
  .container {
    max-width: 1140px;
  }
}
</style>