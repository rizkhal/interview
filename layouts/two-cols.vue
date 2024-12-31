<template>
  <div class="slidev-layout">
    <div class="grid grid-cols-2 gap-16">
      <div class="prose">
        <slot name="default" />
      </div>
      <div class="prose">
        <img
          v-if="$attrs.image"
          :src="$attrs.image"
          class="max-w-full h-[480px] block mx-auto"
          alt="Responsive Image"
        />
        <slot name="right" v-else />
      </div>
    </div>
  </div>
</template>
