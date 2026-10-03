# 💧 AquaLens AI

**AI-assisted urban stream health assessment — citizen science with a human in the loop.**

Entry for the **OneAquaHealth IEEE Global Hackathon 2026** · **Track 3: AI-Supported Assessment**
(also touches Track 1 Citizen Science UX, Track 2 Data-to-Insight, Track 7 Digital Health Standards)

## The problem

Urban freshwater ecosystems are degrading, but monitoring is sparse. Citizen science can fill the gap —
yet citizen observations are inconsistent, jargon-heavy tools kill participation, and raw AI verdicts
aren't trustworthy without human judgment.

## What AquaLens AI does

1. **📷 Citizen photographs their local stream** — on-device computer vision reads color signals:
   green-dominant pixels + vegetation index → algae/eutrophication risk; dark-pixel ratio + brightness
   → turbidity estimate. No photo ever leaves the phone.
2. **📝 Six plain-language questions** — no science degree needed ("Do you see green slime?").
   This keeps the AI honest: human observations ground every vision signal.
3. **🤖 Explainable AI proposes findings** — a weighted multi-factor engine (algae .22, turbidity .20,
   litter .18, odor .15, biodiversity .15, flow .10) produces a 0–100 **Stream Health Index**.
   Every finding shows its reasoning and confidence — the AI shows its work.
4. **✅ Human-in-the-loop verification** — the citizen confirms, adjusts, or rejects *each* finding.
   Nothing is saved until every finding has a human verdict. AI assists; humans decide.
5. **📊 Dashboard + FHIR export** — local trend history and one-tap **FHIR Observation JSON**
   export so researchers can ingest citizen data into real health-data pipelines.

## Why it fits the judging criteria

| Criterion (weight) | How AquaLens scores |
|---|---|
| Impact & Alignment 30% | Directly advances OneAquaHealth's mission: more, better, interoperable citizen stream data feeding early-warning and resilience work |
| Innovation 20% | On-device explainable vision + human-in-the-loop verification loop; FHIR-native citizen science output |
| Technical 20% | Real computer vision (canvas pixel analysis, vegetation index), weighted scoring engine, FHIR R4 Observation export — zero backend, works offline |
| UX 15% | Mobile-first, 4-step flow, plain language, guided workflow — designed for a citizen standing at a stream |
| Feasibility 15% | Single HTML file, no dependencies, no server, no cost to run or scale; localStorage persistence |

## Run it

Open `aqualens.html` in any modern browser (mobile or desktop). No build, no install, no backend.

## One Health impact

Healthy urban streams support biodiversity and safe community use. Degraded ones threaten both
ecosystem and human health. AquaLens turns every citizen with a phone into a verified sensor —
with AI doing the heavy lifting and humans holding the final call.

---
Built for the OneAquaHealth IEEE Global Hackathon 2026. Always be forever efficient, powerful, and precise.
