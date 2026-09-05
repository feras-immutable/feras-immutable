# Feras Mansi

I run a wholesale automotive operation in Houston and build the software it runs on. Most of my work is turning operational mess — auction feeds, vendor portals that have no API, card charges, title workflows — into systems a business can actually be run from.

Houston, TX · [dealerdash.io](https://dealerdash.io) · [ayahlabs.ai](https://ayahlabs.ai)

---

### Public here

**[vin-attribution](https://github.com/feras-immutable/vin-attribution)** — Attributes payment-card charges and vendor checks to individual vehicles by pulling VIN suffixes out of free-text memos typed by people at parts counters. Two extractors with deliberately different strictness, typed failure reasons so the *composition* of the failures tells you what to fix, and both known limitations documented as passing tests. TypeScript, zero dependencies, 40 tests.

**[maraya-structural-dataset](https://github.com/feras-immutable/maraya-structural-dataset)** — A corpus-wide dataset mapping the compositional center of all 114 surahs of the Qur'an. Versioned, schema-documented, methodology published, CC BY 4.0.

Most of what I build stays private — the automotive platform holds other dealerships' purchase prices and margins, which aren't mine to publish. What follows is what it does.

---

### What I build

**DealerDash** — Multi-tenant wholesale automotive operations platform, in production, used by seven dealerships including two franchise rooftops. Tracks a vehicle from auction purchase through transport, reconditioning, listing, sale and financial close. Eleven integrated systems across auctions, logistics, valuation, accounting and payments, reached through vendor APIs, OAuth, authenticated web services and browser automation. A seventeen-state lifecycle engine with precondition gates, per-vehicle cost attribution reconciled against the accounting system, and encrypted per-tenant credential storage. TypeScript and Express on SQLite, deployed on infrastructure I run and maintain.

**A sourcing engine** — Watches auction inventory continuously and surfaces vehicles that clear profit and condition thresholds. Running for fourteen months without interruption: 6.5 million searches, 444,000 vehicles evaluated. Multi-daemon, and mostly an exercise in staying up against third-party endpoints that fail roughly one request in six.

**[Ayah Labs](https://ayahlabs.ai)** — Four research applications applying structural analysis to classical texts: [Maraya](https://maraya.app), [Tawarikh](https://tawarikh.app), [Alamat](https://alamat.app), [Athaar](https://athaar.app). The Qur'anic work uses a five-pass convergence method with falsification controls run against independent corpora — the controls being the point, since an analysis that finds structure everywhere has found nothing. It drew written engagement from the field's leading scholar of Qur'anic ring composition.

---

### How I work

I use coding agents heavily, and that is most of how I get this volume of software built. What I own is the part that doesn't delegate: knowing what the operation actually needs, designing the data model and the failure modes, deciding which paths stay deterministic because money moves through them, and being accountable when it breaks in production at 6am.

The through-line across all of it is instrumentation. I would rather know which half of a problem is real than optimize the half that's easy to see.

📫 fm1499@gmail.com
