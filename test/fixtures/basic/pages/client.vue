<template>
  <div>
    This page should not crash when rendered.
    <ClientOnly class="something">
      test
      <BreaksServer />
      <BreaksServer>Some slot content</BreaksServer>
    </ClientOnly>
    This should render.
    <div>
      <ClientOnly class="another">
        test
        <BreaksServer />
      </ClientOnly>
    </div>
  </div>
</template>
