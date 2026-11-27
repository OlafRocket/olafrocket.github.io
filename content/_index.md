---
title: It's not Rocket Science Lab
layout: hextra-home
---

<div class="lab-hero">

<img class="lab-hero-logo" src="/images/logo.svg" alt="" width="72" height="72" />

<div class="hx:mt-6 hx:mb-6">
{{< hextra/hero-headline >}}
  It's not Rocket Science Lab
{{< /hextra/hero-headline >}}
</div>

<div class="hx:mb-12">
{{< hextra/hero-subtitle >}}
  Open source R&amp;D for software people actually use.
{{< /hextra/hero-subtitle >}}
</div>

<div class="hx:mb-6">
{{< hextra/hero-button text="Read the blog" link="blog" >}}
</div>

</div>

<hr class="lab-rule" />

<h2 class="lab-section">Projects</h2>

{{< hextra/feature-grid cols="2" >}}
  {{< hextra/feature-card
    title="MariaDB language plugins"
    icon="puzzle"
    class="lab-wide"
    subtitle=`<span class="lab-tag">prototype</span> The goal: a language plugin type for MariaDB. A server branch adds the plugin type, dollar-quoted bodies and CREATE FUNCTION / PROCEDURE ... LANGUAGE, so that a stored routine can be written in any language a plugin provides. lang_python and lang_js are the first two languages.`
    link="https://github.com/OlafRocket/server/tree/lang-ext"
    style="background: radial-gradient(ellipse at 50% 90%, rgba(190, 100, 30, 0.30), rgba(255, 255, 255, 0));"
  >}}
  {{< hextra/feature-card
    title="lang_python"
    icon="code"
    subtitle=`<span class="lab-tag">experimental</span> Python inside MariaDB: a server plugin that runs CPython 3.14 and numpy in the server process. Inline code, named functions, columnar aggregates.`
    link="docs"
    style="background: radial-gradient(ellipse at 50% 90%, rgba(150, 82, 38, 0.30), rgba(255, 255, 255, 0));"
  >}}
  {{< hextra/feature-card
    title="lang_js"
    icon="lightning-bolt"
    subtitle=`<span class="lab-tag">prototype</span> JavaScript stored routines for MariaDB. In preparation.`
    style="background: radial-gradient(ellipse at 50% 90%, rgba(96, 58, 34, 0.28), rgba(255, 255, 255, 0));"
  >}}
  {{< hextra/feature-card
    title="y-cpp"
    icon="share"
    subtitle=`<span class="lab-tag">library</span> A minimal port of the Yjs shared editing library to native C++.`
    link="https://github.com/OlafRocket/y-cpp"
    style="background: radial-gradient(ellipse at 50% 90%, rgba(200, 110, 40, 0.28), rgba(255, 255, 255, 0));"
  >}}
  {{< hextra/feature-card
    title="apv-rtp"
    icon="video-camera"
    subtitle=`<span class="lab-tag">prototype</span> RTP payload format for APV (Advanced Professional Video), as a C99 library: packetizer and depacketizer for the IETF draft.`
    link="https://github.com/OlafRocket/apv-rtp"
    style="background: radial-gradient(ellipse at 50% 90%, rgba(120, 96, 52, 0.28), rgba(255, 255, 255, 0));"
  >}}
{{< /hextra/feature-grid >}}
