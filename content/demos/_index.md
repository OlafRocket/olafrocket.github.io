---
title: Demos
---

Each demo is a SQL file in the
[examples folder]({{< repo "examples" "tree" >}}) of the repository. A demo
registers named Python functions with `py_replace_function()` and calls
them with `py_call()`.

{{< cards >}}
  {{< card link="ping" title="ping" subtitle="Measure the latency of another host" >}}
  {{< card link="slack-send" title="slack_send" subtitle="Send a Slack message from a trigger" >}}
  {{< card link="pagerduty-send" title="pagerduty_send" subtitle="Trigger a PagerDuty incident" >}}
{{< /cards >}}
