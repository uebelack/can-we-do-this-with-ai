---
colorSchema: light
favicon: https://uebelacker.dev/favicon.ico
fonts:
  sans: ['Fira Code', 'Caveat']
  serif: Roboto Slab
  mono: Fira Code
  weights: '300,400,600,700'
---

# Können wir das mit KI machen?

## Was sich in Unternehmen mit LLMs automatisieren lässt – und was nicht

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
    <div class="social-post-avatar">MM</div>
    <div>
      <div class="social-post-name">Max Mustermann</div>
      <div class="social-post-meta">Digital Transformation Evangelist | Keynote Speaker</div>
      <div class="social-post-meta">2 Std. · 🌐</div>
    </div>
  </div>
  <div class="social-post-body">
    <p>🔄 <b>Business Automation war gestern – jetzt übernehmen KI-Agenten.</b></p>
    <p>Starre Workflows, teure RPA-Bots: vorbei. KI-Agenten führen Prozesse nicht nur aus – sie denken und handeln eigenständig.</p>
    <p>✅ Kein Workflow-Design mehr – Agenten lernen durch Beobachtung<br/>✅ Flexibel statt starr – sie passen sich in Echtzeit an<br/>✅ Keine Silos – sie arbeiten über alle Abteilungen hinweg</p>
    <p>Wer heute noch auf klassische Automatisierung setzt, wird morgen überholt. 🚀💡</p>
    <p class="social-post-tags">#AI #Automation #KIAgenten #FutureOfWork</p>
  </div>
  <div class="social-post-reactions">👍💡❤️ 428 · 96 Kommentare · 51 Reposts</div>
</div>

---

# Ein Bankkonto eröffnen

```mermaid {scale: 0.72}
flowchart LR
  S(("&nbsp;Start&nbsp;")) --> A[Antrag ausfüllen]
  A --> ID[Identität prüfen]
  ID --> VO{Unterlagen<br/>vollständig?}
  VO -->|nein| NA[Unterlagen<br/>nachfordern]
  NA --> ID
  VO -->|ja| BO{Bonität ok?}
  BO -->|nein| AB[Ablehnen]
  BO -->|ja| KE[Konto eröffnen]
  KE --> WB[Willkommensbrief]
  WB --> EN((("&nbsp;Ende&nbsp;")))
  AB --> EN
  classDef human fill:#fde68a;
  classDef system fill:#bfdbfe;
  class A,ID,NA,AB human;
  class KE,WB system;
```

<div class="legend">
  <span><i class="swatch-human"></i>Mensch</span>
  <span><i class="swatch-system"></i>System</span>
  <span class="hand-note">… und jeder Pfeil dazwischen: von Hand modelliert.</span>
</div>

---

# Wer bin ich?

- **David Übelacker**
- Software Architect @ nag informatik ag in Basel
- 20+ Jahre Erfahrung in der Web- und Mobile-App-Entwicklung

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

# Was ist ein LLM?

Ein Large Language Model (LLM) ist eine Art von künstlicher Intelligenz, die darauf ausgelegt ist, menschenähnlichen Text zu verstehen, vorherzusagen und zu generieren.

<div class="pt-20">

```mermaid {scale: 1.3}
flowchart LR
  start(( )) --> prompt("🙋<br/>Prompt")
  prompt --> llm("🧠<br/>LLM")
  llm --> result("📊<br/>Return result")
  result --> done(( ))
```

</div>

---

# Was ist ein KI-Agent?

Ein KI-Agent ist ein System, das ein Ziel bekommt und mithilfe eines Large Language Models (LLM) und Tools selbst entscheidet, welche Schritte nötig sind – und so lange iteriert, bis es erreicht ist.

<div class="pt-8">

```mermaid {scale: 0.95}
flowchart LR
  start(( )) --> goal("🙋<br/>Define Goal")
  goal --> llm("🧠<br/>LLM")
  llm --> check{"Goal<br/>achieved?"}:::gateway
  check -- no --> tools("🤖<br/>Tools")
  tools --> llm
  check -- yes --> result("📊<br/>Return result")
  result --> done(( ))
  classDef gateway font-size:19px;
```

</div>

---

# Was ist RAG?

RAG (Retrieval-Augmented Generation) ist eine KI-Technik, mit der sich die Ausgabe eines LLM durch gezielte Informationen optimieren lässt, ohne das zugrunde liegende Modell selbst anzupassen.

<div class="pt-8">

```mermaid {scale: 0.86}
flowchart LR
  start(( )) --> question("🙋<br/>Question")
  question --> search("🔍<br/>Similarity<br/>search")
  db[("🗄️<br/>Vector DB")] --> search
  search --> prompt("💬<br/>Prompt<br/>+ Context")
  prompt --> llm("🧠<br/>LLM")
  llm --> result("📊<br/>Return result")
  result --> done(( ))
```

</div>

---
layout: fact
---

# Vielen Dank!

<br/>

<div class="center">
<img src="./images/qr_repo.svg" style="width: 300px"/>
</div>

https://github.com/uebelack/can-we-do-this-with-ai
