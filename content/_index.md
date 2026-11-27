---
title: lang_python
layout: hextra-home
---

{{< hextra/hero-badge >}}
  <div class="hx:w-2 hx:h-2 hx:rounded-full hx:bg-primary-400"></div>
  <span>Experimental, open source</span>
{{< /hextra/hero-badge >}}

<div class="hx:mt-6 hx:mb-6">
{{< hextra/hero-headline >}}
  Python inside MariaDB
{{< /hextra/hero-headline >}}
</div>

<div class="hx:mb-12">
{{< hextra/hero-subtitle >}}
  A server plugin that runs CPython 3.14 and numpy&nbsp;<br class="hx:sm:block hx:hidden" />in the server process
{{< /hextra/hero-subtitle >}}
</div>

<div class="hx:mb-6">
{{< hextra/hero-button text="Get started" link="docs" >}}
</div>

<div class="hx:mt-6"></div>

{{< hextra/feature-grid >}}
  {{< hextra/feature-card
    title="Inline code"
    subtitle="py_eval and py_exec put Python inside a SQL expression, with no DDL."
  >}}
  {{< hextra/feature-card
    title="Named functions"
    subtitle="py_create_function stores Python functions in the server. py_call runs them once per row."
  >}}
  {{< hextra/feature-card
    title="Columnar aggregates"
    subtitle="py_agg passes a whole group of rows to Python as numpy arrays, also over window frames."
  >}}
  {{< hextra/feature-card
    title="Server access"
    subtitle="The built-in inhost module runs SQL from Python inside the hosting server."
  >}}
{{< /hextra/feature-grid >}}
