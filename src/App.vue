<template>
  <RouterView />
</template>

<script>
import { createMemoryHistory, createRouter } from "vue-router";

import HomePage from "./Pages/HomePage.vue";
import Profile from "./Pages/Profile.vue";
import Reg from './Pages/Reg.vue';
import Login from './Pages/Login.vue';

const routes = [
  { path: "/", component: HomePage },
  { path: "/profile", component: Profile },
  { path: "/reg", component: Reg },
  { path: "/login", component: Login },
];

export const router = createRouter({
  history: createMemoryHistory(),
  routes,
});

export default {
  name: "App",
  components: {}
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Raleway:ital,wght@0,100..900;1,100..900&display=swap");
@import "styles/colors.scss";

html,
body,
div,
span,
applet,
object,
iframe,
h1,
h2,
h3,
h4,
h5,
h6,
p,
blockquote,
pre,
a,
abbr,
acronym,
address,
big,
cite,
code,
del,
dfn,
em,
img,
ins,
kbd,
q,
s,
samp,
small,
strike,
strong,
sub,
sup,
tt,
var,
b,
u,
i,
center,
dl,
dt,
dd,
ol,
ul,
li,
fieldset,
form,
label,
legend,
table,
caption,
tbody,
tfoot,
thead,
tr,
th,
td,
article,
aside,
canvas,
details,
embed,
figure,
figcaption,
footer,
header,
hgroup,
menu,
nav,
output,
ruby,
section,
summary,
time,
mark,
audio,
video {
  margin: 0;
  padding: 0;
  border: 0;
  font-size: 100%;
  font: inherit;
  vertical-align: baseline;
}
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
menu,
nav,
section {
  display: block;
}
html {
  height: 100%;
}
body {
  line-height: 1;
}
ol,
ul {
  list-style: none;
}
blockquote,
q {
  quotes: none;
}
blockquote:before,
blockquote:after,
q:before,
q:after {
  content: "";
  content: none;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}

@media (prefers-reduced-motion: no-preference) {
  :root {
    scroll-behavior: smooth;
  }
}

body {
  background-color: #424769;
  font-family: "Raleway", sans-serif;
  font-optical-sizing: auto;
  font-weight: weight;
  font-style: normal;
}

Main,
.soon {
  margin-top: 200px;
  margin-left: auto;
  margin-right: auto;
}
</style>
