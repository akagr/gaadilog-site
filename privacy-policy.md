---
layout: default
title: Privacy Policy
permalink: /privacy-policy/
description: GaadiLog collects nothing by default. Optional anonymous analytics, off out of the box, off-switchable any time. Everything you log lives only on your device.
---

<header class="policy-head">
  <h1 class="policy-head__title">A short, <em>honest</em> privacy policy.</h1>
  <dl class="policy-meta">
    <dt>Effective</dt><dd>TBD on v1.2 release · previously 05 May 2026</dd>
    <dt>App</dt><dd>GaadiLog · <span style="color:var(--ink-soft)">me.akashagrawal.gaadilog</span></dd>
    <dt>By</dt><dd>Akash Agrawal</dd>
    <dt>Contact</dt><dd><a href="mailto:akagr@outlook.com">akagr@outlook.com</a></dd>
  </dl>
</header>

<div class="prose" markdown="0">

<p>This is a plain-English description of how GaadiLog handles your data. By default GaadiLog still collects nothing — the section below describes that default, and the one after describes the optional anonymous analytics you can switch on in Settings if you'd like to help spot bugs and rough edges.</p>

<h2>What we collect — by default</h2>

<div class="declaration">
  <p class="declaration__word">Nothing.</p>
  <p class="declaration__sub">Not a byte. Not a guess. Not a hash.</p>
</div>

<p>GaadiLog stores everything you log — vehicles, fuel-ups, services, documents, reminders, photos — <strong>only on your device.</strong> There is no server. There is no account system. No sign-up, no login, no cloud sync, no backup to our infrastructure, and no way for us to read what you log even if we wanted to.</p>

<h2>What changes if you turn analytics on</h2>

<p>Settings → Privacy has a toggle, <strong>off out of the box</strong>, labeled <em>"Share anonymous usage data."</em> Turning it on sends a small stream of anonymous events to our analytics provider, <a href="https://posthog.com">PostHog</a>, so we can see which features get used and catch errors before they hit users at scale.</p>

<table class="ledger-table">
  <thead>
    <tr>
      <th>Sent when on</th>
      <th>What that means</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Event names</td>
      <td>The action you took — e.g. <code>vehicle_added</code>, <code>fuel_logged</code>, <code>export_run</code>. Never the contents — just that the action happened.</td>
    </tr>
    <tr>
      <td>Anonymous device ID</td>
      <td>A random UUID generated on this device on first launch and stored locally. Not tied to your name, email, phone, or any account. We cannot reverse it to identify you.</td>
    </tr>
    <tr>
      <td>App &amp; device metadata</td>
      <td>App version, OS version, device model, locale, timezone. Used to know whether a bug is iOS-only, India-only, or specific to one build.</td>
    </tr>
    <tr>
      <td>Crash stack traces</td>
      <td>If GaadiLog throws an unexpected error, the stack trace is captured so we can fix it. The trace is code line references — it does not contain anything you have logged.</td>
    </tr>
  </tbody>
</table>

<p><strong>What is never sent, even with analytics on:</strong></p>

<ul>
  <li>Your name, email, or phone number (we do not have these anyway).</li>
  <li>Vehicle plate numbers, makes, models, or any vehicle identifier.</li>
  <li>Fuel, service, or expense values.</li>
  <li>Photos — invoices, document scans, or vehicle pictures.</li>
  <li>Your location.</li>
  <li>Any free-text you have typed into the app.</li>
</ul>

<p>You can flip the toggle off at any time. Once off, no further events leave the device. Events already sent before you turned it off remain in PostHog and decay per the retention policy below.</p>

<h2>Permissions, and why</h2>

<table class="ledger-table">
  <thead>
    <tr>
      <th>Permission</th>
      <th>Why we ask · what we do with it</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Camera<small>iOS &amp; Android</small></td>
      <td>To photograph your vehicle, service invoices, and document scans (RC, insurance, PUC) directly from inside the app. The image is saved into the app's private storage on your device. It is not uploaded anywhere.</td>
    </tr>
    <tr>
      <td>Photo library<small>iOS &amp; Android</small></td>
      <td>To attach photos you already have (existing invoice scans, document images) to a service or document record. The image is copied into the app's private storage. The original in your library is unchanged.</td>
    </tr>
    <tr>
      <td>Notifications<small>iOS &amp; Android</small></td>
      <td>To remind you when a document is about to expire, or when a service interval is due. All reminder scheduling happens on your device via the operating system's local-notification system. No push servers are involved.</td>
    </tr>
    <tr>
      <td>Receive boot completed<small>Android only</small></td>
      <td>To re-arm your scheduled reminders after you reboot your phone. The app does no other background work.</td>
    </tr>
  </tbody>
</table>

<h2>What we share</h2>

<p>If analytics is off — the default — nothing. There is no advertising SDK, no tracking pixel, and no other third-party telemetry in the app.</p>

<p>If analytics is on, the anonymous events described above are sent to <a href="https://posthog.com">PostHog</a>, our analytics provider, acting as a contractual sub-processor. PostHog's own privacy policy is at <a href="https://posthog.com/privacy">posthog.com/privacy</a>. They do not get a license to resell, repackage, or share your usage data — we use their platform only to read it ourselves.</p>

<p>The app's only other network use is downloading the Material 3 system fonts via Flutter's standard rendering, and only if your device has not cached them already.</p>

<h2>Where your data lives</h2>

<p>Everything you log lives in GaadiLog's private storage on your device, in a SQLite database file:</p>

<p><strong>iOS:</strong> in the app's container directory, accessible only to GaadiLog itself and to iOS system tools.<br>
<strong>Android:</strong> in the app's internal storage directory, accessible only to GaadiLog itself.</p>

<p>If you delete the app, this data is deleted along with it. There is no remote copy.</p>

<p>If you have turned analytics on, the anonymous events described earlier also live in PostHog's <strong>[TBD: EU / US]</strong> cloud infrastructure, retained for 12 months and then discarded. Uninstalling the app does not retroactively delete events already sent — but no new events will be sent.</p>

<h2>Export</h2>

<p>You can export your data at any time as CSV (per vehicle, or for all vehicles) and as PDF (a per-vehicle service-history report). The OS share sheet then hands the file to whichever app you choose. Once it leaves GaadiLog's share sheet, the receiving app's privacy policy applies — not ours.</p>

<h2>Children</h2>

<p>GaadiLog has no age gate because it does not collect personal information from anyone. The Indian-market context means most users will be adults registering vehicles, but there is nothing in the app that identifies, tracks, or profiles users of any age.</p>

<h2>Changes to this policy</h2>

<p>If the policy changes — as it did in v1.2, when the optional analytics toggle was added — the new version appears at the same URL with an updated effective date. Material changes (anything that affects what data leaves your device) also surface in-app the next time you open it, which is how you would have found out about the v1.2 update.</p>

<h2>Contact</h2>

<p>Questions, concerns, or notice of any kind: <a href="mailto:akagr@outlook.com">akagr@outlook.com</a>.</p>

</div>
