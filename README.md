<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/header-dark.png">
  <img src="assets/header-light.png" width="100%" alt="Husam El Tahir (حسام الطاهر). Chemical engineer by training, now running strategic programs in the UAE. Builds small AI tools in English and Arabic in his spare time.">
</picture>

<br>

I'm not a software engineer. I build with AI coding tools, and the part I bring is everything around the code: picking a problem worth solving, writing down the rules before anything gets built, and testing until it holds up. It's the same job I've done for over a decade on factory floors, SAP rollouts and data centre builds, just smaller and faster.

Half of what's below works in Arabic as well as English. In the Gulf, that isn't a nice extra.

## How a project goes

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/build-dark.png">
  <img src="assets/build-light.png" width="100%" alt="Five steps in a line: 1 find one real problem, 2 write the rules first, 3 build the smallest useful version, 4 test it on real cases, 5 measure then decide. A dashed loop runs from step 5 back to step 3, labelled fix, then test again.">
</picture>

## Things I've built

### A voice agent that answers in English and Arabic

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/voice-dark.png">
  <img src="assets/voice-light.png" width="100%" alt="Test scorecard from 5 November 2026: 25 of 28 tests passed. English 12 of 14, Modern Standard Arabic 7 of 7, Gulf dialect Arabic 6 of 7.">
</picture>

- Answers questions about moving from the UK to the UAE using only one website's own guides, and runs a live salary comparison when someone asks how much better off they'd be.
- The whole agent is defined in a few config files, so every change can be reviewed, rolled back and tested again.
- 28 written tests, half of them in Arabic, that I can re-run after any change. Some are in Gulf dialect, because that's how people actually talk here.

**[Code and full test results](https://github.com/husameltahir/bilingual-voice-agent)** · built on ElevenLabs · November 2026

<details>
<summary>How it fits together</summary>
<br>

```mermaid
flowchart LR
  Q["Caller asks a question<br/>by voice or text"] --> A["Agent<br/>English or Arabic"]
  A --> K["31 relocation guides<br/>the only source it may use"]
  A --> T["Salary calculator<br/>called live"]
  K --> R["Answer in the<br/>caller's language"]
  T --> R
  S["28 written tests"] -. "re-run after each change" .-> A
```

</details>

### Mudeef, a house-manual concierge for holiday homes

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/mudeef-dark.png">
  <img src="assets/mudeef-light.png" width="100%" alt="Two phone screens of the Mudeef demo in Arabic. Left: a guest asks whether parking is free, and the assistant says it has passed the question to the host. Right: a guest asks for the check-out time, and the assistant answers from the house manual.">
</picture>

*Mudeef (مضيف) is Arabic for host.*

- A host uploads the house manual once. Guests open a link or scan a QR code and ask anything, in English, Arabic, Russian or Hindi.
- It answers only from the manual. If the answer isn't there, it says so and passes the question to the host.
- Refunds, complaints and anything about money are handed to the host. Emergency words are caught before the AI sees the message, and the reply is always the same fixed text with 999, 998 and 997.

**[Try the demo](https://mudeef-concierge-uae.lovable.app/demo)** · a made-up flat in Abu Dhabi, any of the four languages

### A relocation platform for people moving from the UK to the UAE

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/reloc-dark.png">
  <img src="assets/reloc-light.png" width="100%" alt="Three screens from the relocation platform: a UK to UAE salary and cost-of-living comparator, a household move plan, and a decision report showing a verdict and the money left each month.">
</picture>

- Works out whether a UAE offer leaves a household better off once rent, school fees and the move itself are paid for, then plans the move step by step.
- More than 20 tools and 31 guides. Figures on the site carry a dated source, and anything without one gets removed.
- My longest build: started in April 2026, more than 200 small releases since. Live in open beta; I'm happy to share the link.

**[Case study](https://github.com/husameltahir/relocation-platform-case-study)**

### Smaller builds

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/small-dark.png">
  <img src="assets/small-light.png" width="100%" alt="Three smaller projects. Ahlan Score, tested but not launched. Deck Forensics, an early prototype. Risk Radar, with a live demo.">
</picture>

- **Ahlan Score.** With the owner's consent, it sends test enquiries by WhatsApp, Instagram, web form, phone and email, then scores how fast and how well the business replies, including whether it answers in Arabic. The result is a short bilingual report. Built and tested on sample data; no live audits yet.
- **Deck Forensics.** Drop in a PowerPoint deck and it lists every font, colour and figure. It runs in your browser, so the file never leaves your computer. Next on the list: totals that don't add up, and figures that disagree between slides.
- **Risk Radar.** Turns a week of program updates from chat threads, stand-ups and vendor emails into a risk list, with an owner and a source for every item. [Live demo](https://husameltahir.github.io/risk-radar/) · [code](https://github.com/husameltahir/risk-radar)

## Background

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/career-dark.png">
  <img src="assets/career-light.png" width="100%" alt="Career line: 2013 GE, Lean operations, cycle times cut by up to 67%. 2019 Reckitt, global SAP processes across 15 live regions. 2022 Google, new data centres, time to market down 20%. 2025 Abu Dhabi, strategic programs and partnerships. Below it, a second line of side projects from April 2026 to November 2026.">
</picture>

The side projects use the same habits as the day job: agree what good looks like before starting, make it repeatable, then measure it.

## Get in touch

[LinkedIn](https://www.linkedin.com/in/husam-eltahir/) is the best way to reach me. I'm always happy to compare notes with people putting AI in front of real customers, especially in Arabic.

<sub>The screens above come from working demos with made-up data. Last updated November 2026.</sub>
