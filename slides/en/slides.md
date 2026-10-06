---
colorSchema: light
favicon: https://uebelacker.dev/favicon.ico
fonts:
  sans: ['Fira Code', 'Caveat']
  serif: Roboto Slab
  mono: Fira Code
  weights: '300,400,600,700'
---

# Can We Do This with AI?

## What Enterprises Can Automate with LLMs, and What They Can't

<img src="./images/comic.png" class="cover-comic" />

<div class="draft-badge">DRAFT</div>

<div class="absolute bottom-10">
  <span class="font-700">
    David Übelacker
  </span>
</div>

---
layout: center
---

<div class="social-post">
  <div class="social-post-head">
    <div class="social-post-avatar">JD</div>
    <div>
      <div class="social-post-name">Jane Doe</div>
      <div class="social-post-meta">Digital Transformation Evangelist | Keynote Speaker</div>
      <div class="social-post-meta">2h · 🌐</div>
    </div>
  </div>
  <div class="social-post-body">
    <p>🔄 <b>Business automation is yesterday's news – AI agents are taking over.</b></p>
    <p>Rigid workflows, expensive RPA bots: over. AI agents don't just execute processes – they think and act on their own.</p>
    <p>✅ No more workflow design – agents learn by watching<br/>✅ Flexible instead of rigid – they adapt in real time<br/>✅ No more silos – they work across every department</p>
    <p>Anyone still betting on classic automation today will be left behind tomorrow. 🚀💡</p>
    <p class="social-post-tags">#AI #Automation #AIAgents #FutureOfWork</p>
  </div>
  <div class="social-post-reactions">👍💡❤️ 428 · 96 comments · 51 reposts</div>
</div>

---

# Opening a Bank Account

```mermaid {scale: 0.72}
flowchart LR
  S(("&nbsp;Start&nbsp;")) --> A[File application]
  A --> ID[Verify identity]
  ID --> CP{Documents<br/>complete?}
  CP -->|no| RE[Request missing<br/>documents]
  RE --> ID
  CP -->|yes| CR{Credit check ok?}
  CR -->|no| RJ[Reject]
  CR -->|yes| OP[Open account]
  OP --> WL[Welcome letter]
  WL --> EN((("&nbsp;End&nbsp;")))
  RJ --> EN
  classDef human fill:#fde68a;
  classDef system fill:#bfdbfe;
  class A,ID,RE,RJ human;
  class OP,WL system;
```

<div class="legend">
  <span><i class="swatch-human"></i>Human</span>
  <span><i class="swatch-system"></i>System</span>
  <span class="hand-note">… and every arrow between them: modelled by hand.</span>
</div>

---

# Who am I?

- **David Übelacker**
- Software Architect @ nag informatik ag in Basel
- 20+ years of experience in web and mobile app development

<div class="absolute bottom-10">
  <div class="flex items-end">
    <img src="./images/nag.svg" style="width: 20%; filter: invert(1);" />
    <div style="width:45%"></div>
    <div style="width: 30%; display: flex; flex-direction: column; align-items: center;">
      <img src="./images/qr.svg" style="width: 100%;"/>
      <div>uebelacker.dev</div>
    </div>
  </div>
</div>

---
layout: fact
---

# Thank you!

<br/>

<div class="center">
<img src="./images/qr_repo.svg" style="width: 300px"/>
</div>

https://github.com/uebelack/can-we-do-this-with-ai
