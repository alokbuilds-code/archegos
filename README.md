# ARCHÉGOS: THE INVISIBLE POSITION
### An Institutional Financial Investigation & Forensic Digital Dossier

```
[CLASSIFICATION: PUBLIC RECORD / AUTHORITATIVE ARCHIVE]
[SUBJECT: ARCHEGOS CAPITAL MANAGEMENT LP / SUNG KOOK HWANG]
[JURISDICTION: U.S. DISTRICT COURT — SDNY (22-CR-240)]
[INSTRUMENTATION: BILATERAL TOTAL RETURN SWAPS (TRS) / OVER-THE-COUNTER DERIVATIVES]
```

---

## 1. Executive Description

ARCHÉGOS: THE INVISIBLE POSITION is an institutional-grade, investigative computational dossier designed to forensic-engineer the catastrophic March 2021 disintegration of Archegos Capital Management LP, the private single-family office orchestrated by former Tiger Asia principal Sung Kook (Bill) Hwang. Operating beyond the statutory oversight thresholds of the U.S. Securities and Exchange Commission via Dodd-Frank family-office carve-outs under Rule 202(a)(11)(G)-1, the fund exploited bilateral Total Return Swaps (TRS) across an interconnected syndicate of global tier-one prime brokers—including Credit Suisse, Nomura Holdings, Morgan Stanley, Goldman Sachs, and UBS Group AG. Through these non-cleared over-the-counter contracts, Archegos engineered massive synthetic economic exposure toward a hyper-concentrated basket of equities (principally ViacomCBS, Discovery, Inc., Baidu, and Vipshop) without assuming formal legal title or triggering mandatory beneficial ownership reporting on SEC Schedule 13D or Form 13F.

By leveraging an equity cushion of approximately $36 billion at ratios fluctuating between 5:1 and 8:1, the fund sustained notional gross market positions eclipsing $100 billion. Crucially, counterparties operated under severe structural opacity; each lending desk hedged swap liabilities through physical share purchases on open exchanges while remaining entirely ignorant that rival institutions were financing identical underlying positions. When ViacomCBS issued a secondary equity offering on March 22, 2021, inducing an initial 9% price retrenchment, the resulting mark-to-market depreciation breached initial collateral thresholds. As variation margin calls went unanswered, the structural defect of bilateral OTC leverage manifested: a prisoner’s dilemma where early liquidators (Goldman Sachs and Morgan Stanley) salvaged capital through immediate multi-billion-dollar block sales, while delayed counterparties (Credit Suisse and Nomura) sustained devastating unsecured shortfalls totaling $5.5 billion and $2.85 billion respectively.

This research archive synthesizes the authoritative Wikipedia factual baseline, public federal indictments from the Southern District of New York (22-CR-240), Senate Banking Committee inquiries, and regulatory penalty decrees into a cohesive, unembellished digital apparatus. Pairing mathematical risk simulations with historical document inspection, the platform models how regulatory blind spots and fragmented dealer networks convert concealed balance-sheet concentration into systemic financial contagion.

---

## 2. Mathematical Risk & Derivative Formulation

The technical mechanics of the collapse rest upon the asymmetry of the bilateral Total Return Swap (TRS) payoff structure and non-linear capital depletion under multiplier leverage.

### 2.1 The Bilateral Total Return Swap Payoff
For a notional position of $N$ shares in underlying equity $S$ executed at initial trade price $S_0$ and evaluated at timestamp $t$:

$$\Pi_{\text{Archegos}}(t) = N \cdot \left( S_t - S_0 \right) + N \cdot D_{[0, t]} - \int_0^t \left( \text{USD-SOFR} + \kappa_b \right) \cdot \Phi_{\text{borrowed}} \, d\tau$$

Where:
* $S_t - S_0$ represents mark-to-market capital appreciation or depreciation.
* $D_{[0, t]}$ represents aggregate dividend payouts distributed by the underlying issuer.
* $\text{USD-SOFR} + \kappa_b$ represents the prime broker financing spread applied to the borrowed capital balance $\Phi_{\text{borrowed}} = \text{Gross Exposure} - \text{Equity Cushion}$.

### 2.2 Equity Cushion Destruction & Critical Depletion Threshold
Given fund net capital $E_0$, leverage multiplier $L = \frac{G_0}{E_0}$ (where $G_0$ is total gross market exposure), the instantaneous net fund equity $E(t)$ following an underlying price movement $\Delta P = \frac{S_t - S_0}{S_0}$ is:

$$E(t) = E_0 + G_0 \cdot \Delta P = E_0 \cdot \left( 1 + L \cdot \Delta P \right)$$

The critical market retracement $\Delta P_{\text{crit}}$ that triggers a total terminal wipeout of fund equity ($E(t) \le 0$) is defined strictly by the inverse of the leverage factor:

$$\Delta P_{\text{crit}} = -\frac{1}{L}$$

* At $L = 5.0\times$, a market retracement of **$-20.0\%$** reduces the net equity cushion to zero.
* At $L = 7.0\times$, a market retracement of **$-14.28\%$** induces insolvency.
* When ViacomCBS plunged **$-27.0\%$** on Friday, March 26, 2021, Archegos entered immediate default, converting lending banks into unsecured general creditors bearing an aggregate shortfall exceeding **$\$10 \text{ Billion}$**.

---

## 3. Repository Architecture & Directory Blueprint

```
archegos-dossier/
│
├── index.html                 # Complete 16-chapter forensic layout & document modal DOM
├── style.css                  # Institutional typography, color tokens, and layout styles
├── script.js                  # Quantitative simulation engine, canvas network & state machine
└── README.md                  # Comprehensive forensic specification and documentation
```

### Component Architecture Matrix
* **Runtime Engine**: Zero build-tooling dependencies. 100% vanilla ES6+ module-free architecture ensuring persistent archival durability.
* **Canvas Simulation**: Native HTML5 `<canvas>` rendering 2D force-directed nodes and bilateral swap connections without directional arrow artifacts.
* **Document Inspection Room**: Modal interface providing typography scaling, dynamic zoom factors ($0.75\times$ to $1.5\times$), and multi-page pagination over primary court and regulatory dockets.
* **Precision Typography**:
  * Serif Headlines: *Cormorant Garamond* (300/400/500/600 italic & regular).
  * Analytic Body: *Inter* (300/400/500/600).
  * Quantitative Data & Records: *JetBrains Mono* with OpenType tabular figures (`tnum`).

---

## 4. Primary Counterparty Quantitative Loss Tally

Loss figures are documented strictly in accordance with official bank regulatory filings, earnings statements, and public inquiry records:

| Institution | Loss (USD) | Peak Notional | Liquidation Timing | Primary Structural Consequence |
| :--- | :--- | :--- | :--- | :--- |
| **Credit Suisse** | **$5,500,000,000** | >$20.0B | Delayed (Mar 29–30) | Dismissal of CRCO & Investment Bank Head; $2B convertible notes; $387M regulatory penalty; 2023 emergency UBS merger. |
| **Nomura Holdings** | **$2,850,000,000** | Est. $10.0B+ | Delayed (Mar 29–30) | Largest operational loss in corporate history; complete restructuring of U.S. prime services. |
| **Morgan Stanley** | **$911,000,000** | Est. $8.0B+ | Fast (Mar 26–27) | $644M loss sustained in initial block sales; $267M incurred during residual risk derisking. |
| **UBS Group AG** | **$774,000,000** | Est. $5.0B+ | Staggered (Apr 2021) | Material pre-tax charge disclosed in Q1 2021 financial results. |
| **Mitsubishi UFJ (MUFG)** | **$300,000,000** | Undisclosed | Delayed (Mar 30) | EMEA securities division write-down directly tied to margin defaults. |
| **Goldman Sachs** | **$0.00 (Negligible)** | Est. $10.0B+ | Immediate (Mar 26 AM) | Executed preemptive block sales at market open on Friday; transferred loss downstream. |
| **Deutsche Bank** | **$0.00 (Negligible)** | $4,000,000,000 | Immediate (Mar 26 AM) | Liquidated $4B position rapidly without sustaining net balance-sheet impairment. |

---

## 5. Primary Legal & Evidentiary Citations

1. **U.S. District Court (SDNY)**: *United States of America v. Sung Kook Hwang & Patrick Halligan*, Docket No. `22-CR-240 (AKH)`.
   - Charge: Racketeering conspiracy (18 U.S.C. § 1962(d)), securities fraud, wire fraud.
   - Outcome: Convicted on 10 counts (July 2024); Sentenced to 18 years in federal prison (Nov 21, 2024).
2. **U.S. Senate Committee on Banking, Housing, and Urban Affairs**: Formal inquiry letters issued by Chairman Sherrod Brown to Credit Suisse, Nomura, Goldman Sachs, and Morgan Stanley (April 5, 2021).
3. **Credit Suisse Group AG**: Ad-hoc Trading Update pursuant to Article 53 LR (March 29, 2021) & Final Paul Weiss Special Committee Report (July 2021).
4. **Board of Governors of the Federal Reserve System & Bank of England (PRA)**: Joint Cease and Desist Order and $387.5 Million civil money penalty against Credit Suisse (July 24, 2023).

---

## 6. Local Deployment & Execution

The dossier is entirely self-contained. To run locally without web servers or compilers:

```bash
# Clone or navigate to the directory
cd "path/to/archegos-dossier"

# Option A: Direct browser launch
start index.html       # Windows
open index.html        # macOS
xdg-open index.html    # Linux

# Option B: Minimal static local server (preserves strict CORS headers for fonts)
npx serve .
# or
python -m http.server 8080
```

---

## 7. Archival Colophon

* **Content Authority**: Wikipedia (*Archegos Capital Management*) and its 37 corroborating investigative references.
* **Design Philosophy**: High-finance institutional research × Editorial cinema.
* **Strict Visual Governance**: Complete absence of arrow characters (`→`, `➜`, directional glyphs). All relationships structured via typographic hierarchy, status pills, and geometric connectors.
