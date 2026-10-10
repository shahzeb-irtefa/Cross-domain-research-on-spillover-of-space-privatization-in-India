## 1. Main Objective / Research Questions

**Overall objective:** To estimate the _causal, long-term_ effect of public R&D on economic growth, using the Cold War space race (NASA's moonshot) as a natural experiment.

**Why it matters:** Theory says R&D drives growth, and social returns may exceed private returns, so firms underinvest. Governments spend huge sums on R&D (over $158 billion in OECD countries in 2020), yet there was "no credible empirical estimate" of what the moonshot contributed to growth. Policymakers also keep calling for a new "Sputnik moment."

**Specific research questions:**

1. Did the space race cause NASA contracting (spending and patents) to expand in places already specialized in space-relevant technology? (first stage)
2. Did NASA contractor R&D raise manufacturing **value added, employment and capital** locally, in the short and long term?
3. How large is the implied **local fiscal multiplier** compared with ordinary government spending?
4. Did it raise **productivity (TFP)**, meaning were there local technological spillovers?
5. Did **inventors migrate** toward space-capable places, and does that make local effects differ from national effects?
6. After accounting for migration, demand and technology spillovers across regions, do **local and national multipliers** differ?

---

## 2. Research Design

**The identification problem:** NASA did not pick contractors randomly. It "harvested" places and firms that were already technologically strong, which may have grown anyway. So a plain correlation between NASA money and growth is not causal.

**The solution: a triple-difference (DDD) design using Soviet technology demand**

- Define the technological "building blocks" of spaceflight from **Soviet** choices (CIA intelligence estimates), not NASA's. Soviet choices were unrelated to US strengths because there was little US-Soviet trade or knowledge sharing.
- Match these technologies to **pre-1958 US patents** to find which county-industries were already space-capable before Sputnik.
- Compare, **before vs. after** the space race, outcomes in **space industries vs. other industries**, in county-industries with **high vs. low** pre-1958 space capability.

**Three differences:**

|Difference|Treated|Control|
|---|---|---|
|Space capability|High (above median)|Low|
|Industry|Space industry (transportation, electronics)|Other industries|
|Time|Space race (1959–1972) and post-race (1973–1992)|Pre-1958|

**Why the design is credible:**

- The decision to go to the moon came **after** Sputnik (1957), so earlier specialization wasn't caused by NASA.
- Funding was concentrated in two sectors (89–90%), so the industry dimension is sharp.
- County, industry and year fixed effects absorb time-invariant traits; pre-1958 patents × year absorbs differential trends from initial innovation levels.
- **Table 1:** treatment and control groups were balanced in 1958.
- **Figure 5:** no pre-trends in 1947 and 1954.

**Extension for national effects:** Inventor migration model (Moretti & Wilson style) plus a spatial market-access framework (Donaldson & Hornbeck 2016) to separate local from national effects.

---

## 3. Data Sources (in detail)

### 3.1 Technology / space capability data

- **CIA declassified National Intelligence Estimates** of Soviet space capabilities (1946/47–1991), digitized from the CIA FOIA Reading Room. Main measure uses **post-1958** documents (more exclusively about space).
- **US patents, 1945–1958**, with full text, used to build text similarity. Locations come from:
    - **HistPat** (Petralia, Balland & Rigby 2016) for patents before 1975, assigning each patent to the most appropriate county.
    - **USPTO PatentsView** for post-1975, with exact inventor addresses.
    - A USPTO patent-technology-team crosswalk to FIPS counties (1969–2014). Multi-inventor patents are split proportionally.
- **Science Direct (SD) technology terms** used for the cosine-similarity scoring.

### 3.2 NASA activity data

- **NASA contractor spending:** hand-digitized from NASA historical databooks (Van Nimmen & Bruno 1976; Gawdiak 1994; Rumerman 2000, 2012). Gives company names, primary contract amounts, place of performance and headquarters for the **top 100 contractors, 1963–1992**. These top 100 are 87–92% of contractor spending. Measured in 1958 US$.
- **NASA patents:** patents owned or funded by NASA.
    - Pre-1976: **Fleming et al. (2019)**, scraped assignee and government-funding information from USPTO patent text.
    - Post-1976: reported directly by the USPTO.
    - A NASA Technical Reports Server (NTRS) list after 1972 was used to validate.
- **Aggregate NASA spending and employment:** Van Nimmen & Bruno (1976), Rumerman (2000), and Weinzierl (2018) for share of GDP.

### 3.3 Manufacturing outcome data

- **Census of Manufactures**, county × two-digit SIC industry (1972 definition).
    - Digitized: 1947, 1954, 1958, 1963, 1967, 1972.
    - Existing digital sources: 1977, 1982, 1987, 1992.
    - Variables: value added, employment, annual wages (labor income), plant and equipment additions (capital).
- **NBER-CES Manufacturing Industry Database** (Becker, Gray & Marvakov 2021) for industry-level growth in Figure 2.
- Stops at 1992 because 1997+ uses NAICS, and the study focuses on the Cold War.
- Three- and four-digit SIC are available but too many cells are masked.

### 3.4 Controls and additional data

- **Military:** army and navy patents (Fleming et al. 2019), a new military-patent measure built from a **military technology glossary**, county military/defense spending, and 1962 defense-funded research scientists.
- **Skill:** nonproduction worker share (industry-county-year), 1960 high school graduate % (population census), 1962 research scientists (National Register of Scientific and Technical Personnel), 1961 IBM mainframes installed.
- **Other:** transportation cost data, **state personal and corporate tax rates and R&D tax credits** (for the migration model).
- **Inventor panel:** individual inventor IDs built from patent data using **Akcigit et al. (2022)** disambiguation, 1945–1992.

### 3.5 Final sample

- **6,759 industry-county observations, 86 counties, 19 two-digit SIC industries, 1947–1992.**
- Only MSA counties with at least one pre-1958 patent; cell must report in 1958 and at least 8 censuses; ND, SD and WY dropped.
- Migration sample: **11,950** origin-destination-industry-year observations, top 50% of inventors.

---

## 4. Analytical / Statistical Methods

1. **Text analysis:** **Term-frequency cosine similarity** between each CIA document and each pre-1958 patent, aggregated to a county-industry **space capability score** (above median = "high").
2. **Triple-difference regression (Equation 1)** with county, industry and year fixed effects, pre-1958 patents × year, optional MSA × year FE. Standard errors **two-way clustered at MSA × industry**.
3. **Extensive-margin models** (linear probability: any NASA spending/patent = 1) and **PPML** (Poisson pseudo-maximum likelihood) for the intensive margin, which handles many zeros.
4. **TFP estimation:** production function Y = A·K^α·L^β estimated by OLS; log(A) is revenue-based TFP.
5. **Event-study (dynamic) version (Equation 2):** year-by-year coefficients with 1958 as base year, to test pre-trends.
6. **Fiscal multiplier calculation:** (β4 or β5 on value added × mean value added × output/value-added ratio) ÷ (β on spending × mean NASA spending).
7. **Migration model (Equation 3):** log odds of inventors moving from origin to destination, following Moretti & Wilson (2017), with origin, destination and pair fixed effects. Standard errors **three-way clustered** (origin county × year, destination county × year, county pair).
8. **Market-effects model (Equation 4):** adds "High Space Market" interactions, derived from an extension of Donaldson & Hornbeck's market-access trade model.
9. **Robustness tools:** alternative clustering and spatial errors, de Chaisemartin & D'Haultfoeuille heterogeneity-robust estimators, leave-one-state/industry-out, an **IV** using a funding dummy, national industry-level comparisons, alternative space-capability definitions, and a broader space-industry definition.

---

## 5. Key Independent (Explanatory) Variables

**Dependent (outcome) variables, for context:** NASA spending, NASA patents (first stage); log value added, log employment, log capital, log TFP (manufacturing); log out-migration ratio (inventors).

**Main explanatory variables (Equation 1):**

|Variable|Meaning|
|---|---|
|**High Space Capability (ij<1958)**|1 if the county-industry's pre-1958 patent similarity to Soviet space tech (CIA documents) is above median|
|**Space Race**|1 for 1959–1972 (census years 1963, 1967, 1972)|
|**Post-Space Race**|1 for 1973–1992 (census years 1977–1992)|
|**Space Industry**|1 for transportation or electronics (the sectors NASA demanded)|
|**Key interactions β4, β5**|HighSpace × SpaceRace × SpaceIndustry, and HighSpace × PostSpaceRace × SpaceIndustry (the treatment effects)|

**Controls / fixed effects:** county FE, industry FE, year FE, pre-1958 patents × year, MSA × year; army and navy patents; military spending; 1962 defense scientists × year; nonproduction worker share; 1960 high school graduates × year; 1962 research scientists × year; 1961 IBM mainframes × year.

**Migration model variables:** difference in log space score between destination and origin, interacted with space race, post-race and space industry; differences in personal tax, corporate tax and R&D credit rates.

**Market-effects model:** **High Space Market**, a binary variable for above-median space capability in a county-industry's market, with the same interactions.

---

## 6. Main Points of the Paper

- The space race is a rare, large and well-documented public R&D shock: NASA was over 0.7% of GDP in the mid-1960s, with 400,000+ workers; contractors were about 90% of its employment.
- NASA "harvested" existing capability, so the authors identify exogenous variation via **Soviet technology demand** matched to **pre-1958 US patents**.
- Spending was extremely concentrated: transportation and electronics took about 90%, and the top 10 contractors took nearly 70% (1965).
- Winning the race often meant **combining or speeding up existing technologies** rather than inventing new ones (Robbins et al. 1972).
- NASA R&D raised **output, jobs and capital** in space sectors, but **not productivity**.
- The local fiscal multiplier is small (**0.3 and 0.4**).
- **Inventors migrated** toward space locations, but spillovers elsewhere offset this, so **local ≈ national**.
- The "Sputnik moment" argument should be treated with caution.
- Mission-oriented, centralized R&D (like NASA) may not represent public R&D generally.

---

## 7. Findings

**First stage (Table 2)**

- High-capability space-industry cells got more NASA activity: extensive-margin effects about 0.07–0.08 for spending and 0.05–0.12 for patents.
- NASA spent about **$264 million more (race)** and **$240 million more (post-race)** in 1958 dollars. Patent effects were more than twice as large after the race as during it (patent attribution is noisy).

**Manufacturing (Table 3)**

- Value added: about **+0.35 to +0.38** log points, similar during and after the race.
- Employment: about **+0.42 to +0.45** during the race and **+0.34 to +0.36** after.
- Capital: **+0.25 to +0.31** during and **+0.50 to +0.56** after (larger later, consistent with lagged accumulation).
- **TFP: about zero (−0.04 to −0.02), insignificant.** So no productivity gain or tech spillover detected.
- Non-space cells (β2, β3): about zero, so no spillover to non-space industries.

**Validity checks**

- No pre-trends (1947, 1954) in Figure 5.
- Results stay the same after controlling for military activity and skill (Table 4), and across many robustness checks.

**Multipliers**

- **Local fiscal multiplier ≈ 0.3 (1958–1972) and ≈ 0.4 (post-1972).**
- Below Ramey's 0.6–0.8 general range; low end of the 0.3–1.2 military range.

**Migration (Table 5)**

- Space-industry inventors moved toward space-capable places: η3 ≈ 0.27–0.28 (race) and η4 ≈ 0.52–0.68 (post-race, larger, so migration takes time). Robust to tax controls and state × year FE.
- Non-space inventors had a _negative_ effect during the race, possibly competition for scarce lab resources.

**Market / national effects (Table 6)**

- Market-effect coefficients are near zero and imprecise, with local effects unchanged.
- Migration to space places offsets positive demand/tech spillovers, so **local and national multipliers are largely the same.**

**Bottom line:** Moonshot R&D had real, meaningful effects **in the space sector**, but modest in size, no larger than non-R&D government spending, and with limited evidence of broad productivity growth.

---

## 8. Drawbacks / Limitations

**Scope and generalizability**

- **Only NASA contractor spending** is studied. It excludes spending at **universities and NASA's own research centers**, which may be more basic-research-heavy and a bigger source of spillovers. The authors say the multiplier and spillover estimates are likely **lower bounds**.
- **Manufacturing only.** Effects in services, other sectors or via international diffusion are not captured.
- **Mission-oriented, centralized R&D** (Mowery, Nelson & Martin 2010) may not generalize to other public R&D.
- **State dependence:** the 1960s were a boom; effects might differ in slow-growth periods.
- Multiplier **ignores spillovers to other industries or places** and **how spending was financed** (taxes or debt).

**Measurement problems**

- **NASA patent attribution is noisy**, especially before government interest statements were required and because NASA could waive rights to contractors (pre-Bayh-Dole). Spending and patents are only weakly spatially correlated.
- **Military patents are undercounted** (army and navy were "license agencies"). Even the new glossary-based measure is imperfect.
- **TFP is revenue-based**, mixing quantity, quality and price, and doesn't address endogenous input choices.
- Patents only capture a part of innovation; patent inventor location and "modal industry" are approximations.
- **Two-digit SIC** industries are coarse (finer data have too many masked cells). Census data exist only in certain years (about every five years).
- The **space capability score** depends on text similarity choices and CIA documents (checked in robustness, but still a constructed measure).

**Identification caveats**

- Can't test **pre-trends in NASA spending** (NASA didn't exist before 1958).
- Relies on the assumption that Soviet technology demand is unrelated to US local growth trends and on a binary above-median cutoff.
- Table 1 shows **some baseline differences** (labor income, navy patents, total patents, skill), though the DDD differences are mostly balanced.
- Highly saturated models with **industry-county fixed effects weaken** the value added and employment effects (limited time dimension).
- National-level industry comparisons weaken the design (NASA-sector-specific shocks could bias estimates).
- **Sample restrictions** (urban MSA counties, balanced-ish panel requirements) may limit representativeness. Only 86 counties.
- Post-race effects confound continuing NASA spending with long-run technology effects, so distinguishing demand from spillovers relies on the pattern of coefficients over time.

**Migration and spatial analysis**

- **No individual panel data** exist for the period; migration is observed only for **patent inventors**, not for ordinary workers.
- Inventor migration estimates do not directly measure total labor reallocation.
- The spatial framework relies on a **theory-based market measure** and imprecisely estimated market effects, so "no wedge" may partly reflect low statistical power.
- Authors note the negative effect for non-space inventors is not fully explained.