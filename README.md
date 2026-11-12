<!--
  SHARED FILE — two agent sessions maintain this README.
  One looks after the Ground app, the other after Winds Aloft & Weather.
  Both commit as the same author, so the log cannot tell you who wrote what.

  PROTOCOL
  1. git pull --rebase  immediately before every push. Never force-push.
  2. Edit ONLY inside your own blocks. Blocks are delimited by HTML comments
     whose names carry the app: "ground:card", "ground:prose", "winds:card",
     "winds:prose", each with a :start and an :end. Each app owns two.
  3. Everything outside those blocks is shared. Change it only when it is
     genuinely about your app, and never reformat the other block.
  4. If a push is rejected, read the other side's commit before rebasing.
-->

# Nikos Pavlopoulos

Software developer — Java and Spring Boot by training, most recently TypeScript on
Cloudflare Workers. Backed by 10+ years of analytical and customer-facing work in
multinational environments.

📄 [Resume](https://resume.nikospavlopoulos.com) · 📩 Contact me via the email in my profile info

---

## Skydive Athens — production software for a dropzone

I am a licensed USPA skydiver and a certified skydiving coach, and I work ground
crew at a dropzone in Boeotia, Greece. I built both of these on my own initiative,
pro bono, to fix problems I kept running into there. Both are live, and both are
used on operating days.

<table width="100%">
<tr>
<td width="50%" valign="top" align="center">
<!-- ground:card:start -->

### Ground — fuel and flight log

<img src="images/ground-today.png" width="380" alt="The Today screen: three loads with takeoff, landing, duration and fuel, and the day's totals beneath">

**[▶ Try the demo](https://ground-demo.skydive-athens.com)**<br>
**[Case study and runnable code](https://github.com/nikospavlopoulos/sd-ground-demo)**

<!-- ground:card:end -->
</td>
<td width="50%" valign="top" align="center">
<!-- winds:card:start -->

### Winds Aloft &amp; Weather

<img src="images/winds-aloft.png" width="380" alt="The Winds screen: the wind every 1,000 ft above the field, each step with a drift arrow, direction, speed and temperature">

**[▶ Open the app](https://winds.skydive-athens.com)**<br>
**[Case study and runnable code](https://github.com/nikospavlopoulos/sd-winds-demo)**

<!-- winds:card:end -->
</td>
</tr>
</table>

<!-- ground:prose:start -->

**Ground** records every load the jump aircraft flies and every litre of fuel that
goes into it, replacing a phone note that was retyped from scratch every day and
whose totals were mental arithmetic between loads. The client is authoritative, so
a tap registers the moment it happens and survives a dropout while the crew move
around the zone. Totals are derived on read and never stored.

`TypeScript` `Preact` `Hono` `Cloudflare Workers` `D1 / SQLite` `Vitest` `Playwright`

<!-- ground:prose:end -->

<!-- winds:prose:start -->

**Winds Aloft & Weather** gives the wind every 1,000 ft from the surface to
15,000 ft **above the field** — the way an altimeter reads it, not above sea
level — with a drift arrow pointing where the wind will carry you. Five days,
scrubbed hour by hour with no further requests, plus surface weather from three
forecast models and cloud by height from two.

`TypeScript` `Preact` `Hono` `Cloudflare Workers` `Open-Meteo` `Vitest` `Playwright`

<!-- winds:prose:end -->

---

## Earlier work

- **[Skydiving Logbook REST API](https://github.com/nikospavlopoulos/skydivinglogbook-spring-rest)**
  [![Tests](https://github.com/nikospavlopoulos/skydivinglogbook-spring-rest/actions/workflows/test-workflow.yml/badge.svg)](https://github.com/nikospavlopoulos/skydivinglogbook-spring-rest/actions/workflows/test-workflow.yml)
  — log and manage skydiving jumps, with role-based access. Java, Spring Boot,
  Spring Data JPA, JWT via custom Spring Security filters, MySQL and H2,
  multi-stage Docker, CI running JUnit and integration tests at 95% coverage.
  [Video demo](https://youtu.be/ddpZyq2-30Q?si=0WPRMsWgoW6kFFLE).
- **[Skydiving Logbook — Thymeleaf](https://github.com/nikospavlopoulos/skydivinglogbook-spring-thymeleaf)**
  — my first full-stack project, and the REST API's predecessor.
- **[Airplane Crash Analysis](https://github.com/nikospavlopoulos/plane_crashes_R)**
  — long-term trends in airplane crashes and fatalities, cleaned, analysed and
  visualised in R.
- **[ProudSalesPro](https://github.com/nikospavlopoulos/proudsalespro)**
  — self-hosted WordPress blog on professional sales, 2012–2022. Ranked on
  Google's first page for two Greek search terms between 2014 and 2020.
- **[Traditional vs Agile](https://gist.github.com/nikospavlopoulos/f60bc9ad46a3d53a1b9818184592c50e)**
  — a 45-minute class presentation from a project-management programme at New
  York College, Athens.

---

#### Also

A fanatic Ubuntu and Firefox user. I like jumping out of perfectly good
airplanes, rock climbing, Lindy Hop, and Toastmasters — and there is a
[Scratch skydive project](https://scratch.mit.edu/projects/1140480389) too.
