---
layout: default
title: Privacy Policy
permalink: /privacy-policy/
description: GaadiLog collects nothing. No accounts, no cloud, no tracking SDKs. Everything you log lives only on your device.
---

<header class="policy-head">
  <h1 class="policy-head__title">A short, <em>honest</em> privacy policy.</h1>
  <dl class="policy-meta">
    <dt>Effective</dt><dd>05 May 2026</dd>
    <dt>App</dt><dd>GaadiLog · <span style="color:var(--ink-soft)">me.akashagrawal.gaadilog</span></dd>
    <dt>By</dt><dd>Akash Agrawal</dd>
    <dt>Contact</dt><dd><a href="mailto:akagr@outlook.com">akagr@outlook.com</a></dd>
  </dl>
</header>

<div class="prose" markdown="0">

<p>This is a plain-English description of how GaadiLog handles your data. There is no legalese boilerplate because there is no data collection to describe in legalese.</p>

<h2>What we collect</h2>

<div class="declaration">
  <p class="declaration__word">Nothing.</p>
  <p class="declaration__sub">Not a byte. Not a guess. Not a hash.</p>
</div>

<p>GaadiLog stores everything you log — vehicles, fuel-ups, services, documents, reminders, photos — <strong>only on your device.</strong> There is no server. There is no account system. No sign-up, no login, no cloud sync, no backup to our infrastructure, and no way for us to read what you log even if we wanted to.</p>

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

<p>Nothing. There is no third-party analytics SDK, no crash-reporting SDK, no advertising SDK, no tracking pixel, and no telemetry of any kind in the app. The app's only network use is downloading the Material 3 system fonts via Flutter's standard rendering — and only if your device hasn't cached them already.</p>

<h2>Where your data lives</h2>

<p>In GaadiLog's private storage on your device, in a SQLite database file:</p>

<p><strong>iOS:</strong> in the app's container directory, accessible only to GaadiLog itself and to iOS system tools.<br>
<strong>Android:</strong> in the app's internal storage directory, accessible only to GaadiLog itself.</p>

<p>If you delete the app, this data is deleted along with it. There is no remote copy.</p>

<h2>Export</h2>

<p>You can export your data at any time as CSV (per vehicle, or for all vehicles) and as PDF (a per-vehicle service-history report). The OS share sheet then hands the file to whichever app you choose. Once it leaves GaadiLog's share sheet, the receiving app's privacy policy applies — not ours.</p>

<h2>Children</h2>

<p>GaadiLog has no age gate because it does not collect personal information from anyone. The Indian-market context means most users will be adults registering vehicles, but there is nothing in the app that identifies, tracks, or profiles users of any age.</p>

<h2>Changes to this policy</h2>

<p>If the policy changes — for example, when a future version adds an opt-in cloud sync — the new version will appear at the same URL with an updated effective date. Material changes (anything that affects what data leaves your device) will also surface in-app the next time you open it.</p>

<h2>Contact</h2>

<p>Questions, concerns, or notice of any kind: <a href="mailto:akagr@outlook.com">akagr@outlook.com</a>.</p>

</div>
