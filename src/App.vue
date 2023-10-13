<template>
  <div
    class="flex flex-col min-h-screen font-Roboto bg-weather-primary"
  >
    <SiteNavigation />
    <RouterView class="flex-1" v-slot="{ Component }">
      <Transition name="page">
        <component :is="Component" />
      </Transition>
    </RouterView>
  </div>
</template>

<script setup>
import { RouterView } from "vue-router";
import SiteNavigation from "./components/SiteNavigation.vue";
</script>

<style type="text/css">
.page-enter-active {
  transition: 600ms ease all;
}
.page-enter-from {
  opacity: 0;
}
</style>
<style type="text/css">

body {
  margin: 0; /* 1 */
  line-height: inherit; /* 2 */
}


fieldset {
  margin: 0;
  padding: 0;
}

legend {
  padding: 0;
}

ol,
ul,
menu {
  list-style: none;
  margin: 0;
  padding: 0;
}

.container {
  width: 100%;
  margin-right: auto;
  margin-left: auto;
  padding-right: 2rem;
  padding-left: 2rem;
}

@media (min-width: 768px) {

  .container {
    max-width: 768px;
  }
}
.absolute {
  position: absolute;
}
.relative {
  position: relative;
}
.sticky {
  position: -webkit-sticky;
  position: sticky;
}
.top-0 {
  top: 0px;
}
.left-0 {
  left: 0px;
}
.top-\[66px\] {
  top: 66px;
}
.mx-8 {
  margin-left: 2rem;
  margin-right: 2rem;
}
.mb-2 {
  margin-bottom: 0.5rem;
}
.mb-12 {
  margin-bottom: 3rem;
}
.mb-8 {
  margin-bottom: 2rem;
}
.mb-4 {
  margin-bottom: 1rem;
}
.mt-32 {
  margin-top: 8rem;
}
.mt-8 {
  margin-top: 2rem;
}
.flex {
  display: flex;
}
.h-auto {
  height: auto;
}
.h-\[50px\] {
  height: 50px;
}
.h-screen {
  height: 100vh;
}
.h-\[100px\] {
  height: 100px;
}
.h-\[75px\] {
  height: 75px;
}
.min-h-screen {
  min-height: 100vh;
}
.w-\[150px\] {
  width: 150px;
}
.w-full {
  width: 100%;
}
.w-auto {
  width: auto;
}
.max-w-screen-md {
  max-width: 768px;
}
.max-w-\[50\%\] {
  max-width: 50%;
}
.max-w-\[40\%\] {
  max-width: 40%;
}
.max-w-\[50px\] {
  max-width: 50px;
}
.max-w-\[75px\] {
  max-width: 75px;
}
.max-w-\[300px\] {
  max-width: 300px;
}
.flex-1 {
  flex: 1 1 0%;
}
.transform {
  transform: translate(var(--tw-translate-x), var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y));
}
@-webkit-keyframes pulse {

  50% {
    opacity: .5;
  }
}
@keyframes pulse {

  50% {
    opacity: .5;
  }
}
.animate-pulse {
  -webkit-animation: pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
          animation: pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
}
.cursor-pointer {
  cursor: pointer;
}
.flex-col {
  flex-direction: column;
}
.items-end {
  align-items: flex-end;
}
.items-center {
  align-items: center;
}
.justify-end {
  justify-content: flex-end;
}
.justify-center {
  justify-content: center;
}
.gap-10 {
  gap: 2.5rem;
}
.gap-4 {
  gap: 1rem;
}
.gap-2 {
  gap: 0.5rem;
}
.gap-3 {
  gap: 0.75rem;
}
.self-start {
  align-self: flex-start;
}
.self-end {
  align-self: flex-end;
}
.overflow-x-scroll {
  overflow-x: scroll;
}
.whitespace-nowrap {
  white-space: nowrap;
}
.rounded-md {
  border-radius: 0.375rem;
}
.border {
  border-width: 1px;
}
.border-b {
  border-bottom-width: 1px;
}
.border-white {
  --tw-border-opacity: 1;
  border-color: rgb( 255 255 / var(--tw-border-opacity));
}
.border-opacity-10 {
  --tw-border-opacity: 0.1;
}
.bg-weather-primary {
  --tw-bg-opacity: 1;
  background-color:  rgb(251 180 215 / var(--tw-bg-opacity));
}
.bg-black {
  --tw-bg-opacity: 1;
  background-color: rgb(0 0 0 / var(--tw-bg-opacity));
}
.bg-white {
  --tw-bg-opacity: 1;
  background-color: rgb(255 255 255 / var(--tw-bg-opacity));
}
.bg-weather-secondary {
  --tw-bg-opacity: 1;
  background-color: rgb(0 78 113 / var(--tw-bg-opacity));
}
.bg-transparent {
  background-color: transparent;
}
.bg-opacity-30 {
  --tw-bg-opacity: 0.3;
}
.bg-gradient-to-r {
  background-image: linear-gradient(to right, var(--tw-gradient-stops));
}
.from-gray-100 {
  --tw-gradient-from: #000000;
  --tw-gradient-to: rgb(243 244 246 / 0);
  --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
}
.object-cover {
  -o-object-fit: cover;
     object-fit: cover;
}
.p-4 {
  padding: 1rem;
}
.py-12 {
  padding-top: 3rem;
  padding-bottom: 3rem;
}
.px-8 {
  padding-left: 2rem;
  padding-right: 2rem;
}
.py-2 {
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
}
.px-6 {
  padding-left: 1.5rem;
  padding-right: 1.5rem;
}
.py-6 {
  padding-top: 1.5rem;
  padding-bottom: 1.5rem;
}
.px-3 {
  padding-left: 0.75rem;
  padding-right: 0.75rem;
}
.px-1 {
  padding-left: 0.25rem;
  padding-right: 0.25rem;
}
.pt-4 {
  padding-top: 1rem;
}
.font-Roboto {
  font-family: Roboto, sans-serif;
}
.text-4xl {
  font-size: 2.25rem;
  line-height: 2.5rem;
}
.text-sm {
  font-size: 0.875rem;
  line-height: 1.25rem;
}
.text-8xl {
  font-size: 6rem;
  line-height: 1;
}
.text-xl {
  font-size: 1.25rem;
  line-height: 1.75rem;
}
.text-3xl {
  font-size: 1.875rem;
  line-height: 2.25rem;
}
.text-xs {
  font-size: 0.75rem;
  line-height: 1rem;
}
.text-2xl {
  font-size: 1.5rem;
  line-height: 2rem;
}
.capitalize {
  text-transform: capitalize;
}
.text-white {
  --tw-text-opacity: 1;
  color: rgb(102 0 149 / var(--tw-text-opacity));
}
.shadow-md {
  --tw-shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
  --tw-shadow-colored: 0 4px 6px -1px var(--tw-shadow-color), 0 2px 4px -2px var(--tw-shadow-color);
  box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
}
.shadow-lg {
  --tw-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);
  --tw-shadow-colored: 0 10px 15px -3px var(--tw-shadow-color), 0 4px 6px -4px var(--tw-shadow-color);
  box-shadow: var(--tw-ring-offset-shadow, 0 0 #0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
}
.transition {
  transition-property: color, background-color, border-color, fill, stroke, opacity, box-shadow, transform, filter, -webkit-text-decoration-color, -webkit-backdrop-filter;
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, backdrop-filter;
  transition-property: color, background-color, border-color, text-decoration-color, fill, stroke, opacity, box-shadow, transform, filter, backdrop-filter, -webkit-text-decoration-color, -webkit-backdrop-filter;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
  transition-duration: 150ms;
}
.focus\:border-weather-secondary:focus {
  --tw-border-opacity: 1;
  border-color: rgb(0 78 1 / var(--tw-border-opacity));
}
.focus\:shadow-\[0px_1px_0_0_\#004E71\]:focus {
  --tw-shadow: 0px 1px 0 0 #000000;
  --tw-shadow-colored: 0px 1px 0 0 var(--tw-shadow-color);
  box-shadow: var(--tw-ring-offset-shadow, 0 0 #11ff0000), var(--tw-ring-shadow, 0 0 #0000), var(--tw-shadow);
}
.focus\:outline-none:focus {
  outline: 2px solid transparent;
  outline-offset: 2px;
}
@media (min-width: 640px) {

  .sm\:flex-row {
    flex-direction: row;
  }
}
</style>