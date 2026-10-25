[[Primary Research Paper 2]]

# Moonshot: Public R&D and Growth: Detailed Notes

**Paper:** #Kantor & #Whalley, _American Economic Review_, Sept 2025, 115(9): 2891–2925 **Legend:** ⭐ = parts you marked "IMP" in your PDF

---

## 1. The Big Picture (Abstract in plain words)

- **Question:** Can government-funded R&D create long-term economic growth?
- **Setting:** The Cold War space race (1957 Sputnik → 1969 moon landing → later years), using NASA contractor spending.
- **Problem they solve:** NASA didn't pick contractors randomly. It picked firms/places that were already good, and those places might have grown anyway. So a simple comparison would be misleading. The authors build a clever way to get "windfall" R&D that is not driven by local growth trends.
- **Main findings:**
    1. NASA contractor R&D **did increase** manufacturing value added, employment and capital in space-related sectors.
    2. Migration (inventors moving) happened, but **not enough** to make local effects differ from national effects.
    3. Overall effect was **modest**: local fiscal multiplier ≈ 0.3 (during the race) and ≈ 0.4 (after).
    4. **No evidence of productivity (TFP) gains or technology spillovers** in the data they can measure.
- **JEL codes:** E22, H54, L60, N12, N42, N62, O47.

---

## 2. Introduction (pp. 2891–2897)

### 2.1 Motivation

- Growth theory (Solow 1957; Romer 1990; Aghion & Howitt 1992) says technology drives growth.
- Social returns to R&D may exceed private returns, so firms **underinvest** in innovation (Arrow 1962; Griliches 1992; Bloom et al. 2013).
- Can government R&D fill the gap? Governments in OECD countries spend over **$158 billion** on R&D (2020), yet the answer is unclear.

### 2.2 Why the space race? (Figure 1)

- Sputnik (1957) → geopolitical crisis → NASA created 1958 → race to the moon launched 1961.
- NASA got **over 0.7% of GDP** in the mid-1960s and employed **over 400,000 workers** at the peak.
- Figure 1 shows: Panel A, NASA spending (total and contractor) jumps after 1958, peaks mid-1960s (about $5,000 million in 1958 dollars), falls, then stays roughly $2,000–3,000 million. Panel B, NASA patents rise sharply after the late 1960s, while total patents and total government patents rise slowly.

### 2.3 Why manufacturing?

- Reaching the moon needed not just ideas but **real products**: spacecraft, satellites, thrusters, navigation and communications equipment, computer hardware and software, launch infrastructure. Manufacturing captures these indirect effects well.

### 2.4 ⭐ The key research design idea ("technology harvesting")

- NASA had to win quickly, so it gave money to firms **already specialized** in the technological building blocks of space. It harvested existing promising technology rather than picking randomly.
- **Problem:** If NASA picked places already poised to grow, NASA spending and growth would be correlated without NASA causing anything.
- **Two-step fix:**
    1. Use the CIA's declassified National Intelligence Estimates on **Soviet space technology** (post-Sputnik) to define what technologies the space mission "demanded."
    2. Search for those technologies in **US patents before 1958** to see which industries in which counties were already specialized in them.
- A county-industry has **"high space capability"** if its pre-1958 patents match the post-1958 Soviet space tech demand.
- **Why Soviet, not NASA's choices?** Soviet choices reflected Soviet mission needs and Soviet strengths. With almost no US-Soviet trade or knowledge sharing, they were unrelated to where the US happened to be strong. This isolates variation in NASA R&D that's "virtually independent of location-specific unobservables."
- **Design in one line:** compare changes in outcomes between space industries and other industries, before vs. after the space race, in county-industries with different pre-1958 space capability. This is a **triple difference**.

### 2.5 ⭐ Data built

- A new panel of **large urban counties, 1947–1992**.
- Digitized the amount NASA contractors received for each industry-county.
- Matched to **census of manufactures** data (value added, employment, labor income) at county × two-digit industry level.
- Also used **government ownership/funding of patents** from Fleming et al. (2019).

### 2.6 Background facts

- NASA spending was concentrated in a few sectors (Figure 2A) that grew faster than others in output, employment, capital and TFP over 1958–1992 (Figure 2B). But this might not be causal, hence the design above.

### 2.7 Five main results

1. **First stage:** The space race caused NASA contracting (spending and patents) to expand more in industry-counties already specialized in space building blocks before Sputnik.
2. **Growth:** The space race caused manufacturing **value added, employment and capital** to grow more in those same pairs.
    - Worry: NASA just followed manufacturing trends. They show **no differential pre-trends** before the race, so NASA wasn't following local private trends. Results hold with controls for industry trends, military contracting and skill.
3. ⭐ **Fiscal multiplier:** Space race spending was large, so local effects could come just from the fiscal multiplier, even without tech spillovers. They estimate about **0.3 during the race** and **0.4 after**.
    - Ramey (2019, p. 103) says typical government spending multipliers are **0.6–0.8, perhaps up to 1**.
    - Military spending triggered by wars or foreign policy: **0.3–1.2** (Batini et al. 2014).
    - **Conclusion:** NASA contractor R&D had a _relatively small_ output effect compared to normal government spending or even defense spending.
4. ⭐ **Productivity spillovers:** They do **not** detect local technological spillovers.
    - Caveat: estimates are probably **lower bounds** because they don't capture NASA spending at universities or NASA's own research centers, international diffusion, or effects outside manufacturing.
5. ⭐ **Migration:** Local estimates would overstate national effects if workers moved in from elsewhere.
    - Using inventor-level patent panel data (Akcigit et al. 2022), they find inventors in space industries **did migrate** toward space-capable places, robust to normal county-to-county migration patterns and state tax policy.
    - **But** other positive spillovers (demand, technology) can offset this. Using a spatial framework based on Donaldson & Hornbeck (2016), they find that in the medium and long term, overall market effects were small enough **not to amplify or attenuate** the local effects. So **local and national fiscal multipliers were largely the same.**

### 2.8 ⭐ Contributions to literature (p. 2896)

1. **Innovation economics / public R&D:** Prior work gives causal estimates of public R&D on knowledge production (Azoulay et al. 2019; Myers & Lanahan 2022; Gross & Sampat 2023) and productivity (Moretti, Steinwender & Van Reenen 2025). Closest paper: Schweiger, Stepanov & Zacchia (2022), where Soviet science cities are more productive today. **This paper adds causal estimates of public R&D on long-term economic growth.**
2. **Industrial policy:** Temporary management transfers (Giorcelli 2019), trade protection (Juhász 2018), university funding (Kantor & Whalley; Hausman; Andrews) can have long-term effects. Criscuolo et al. (2019) found short-run effects on small firms' employment, but not long-term. South Korea's 1970s industrial policy had persistent effects (Lane; Choi & Levchenko). **This paper gives evidence on the spatial and temporal lags of public R&D that directly engaged private firms.**
3. **Government spending multipliers:** Complements Ramey (2021) on short vs. long-run effects of infrastructure, and Antolin-Diaz & Surico on public spending. Contributes to whether **local multipliers reflect national multipliers** (Nakamura & Steinsson 2014; Chodorow-Reich 2019; Ramey 2019). Inventors did migrate toward persistent fiscal shocks, but **not enough to create a wedge** between local and national multipliers.

### 2.9 The "Sputnik moment" debate

- **Pro-moonshot view:** Mazzucato (2021) says NASA was good at coordinating research and the geopolitical mission motivated scientists. Gruber & Johnson (2019) call for a new "Sputnik moment." Footnote 4: Biden's Cancer Moonshot (2022), Obama's (2016), and Nixon's 1971 National Cancer Act speech all invoke the moon landing.
- **Skeptical view:** Surveys of space scientists shortly after (Robbins, Kelley & Elliott 1972) say NASA's role was mostly _incremental_. Fogel (1966) doubted that commercially useful tech would come from mission-oriented R&D.
- **This paper's verdict:** Moonshot R&D had **first-order effects in space sectors**, but magnitude is at the **low end** of typical multipliers, so its role in **broad-based productivity growth was rather limited.**
- Nelson (1959) is the intellectual root of the "moonshot" idea in economics. Footnote 6: business R&D is shifting away from basic research (Arora et al. 2021), so public funding for basic research may matter more.

---

## 3. Historical Background (Section I)

### A. Origins of NASA

- Sputnik launched **Oct 4, 1957**. US intelligence knew a launch was coming, but the US's **Vanguard** failure on live TV (Dec 6, 1957) caused public fear.
- Eisenhower (1958 State of the Union): the Soviets were "waging total cold war" using every area of life.
- Eisenhower proposed **NASA in 1958**: civilian control of space, except weapons systems, military operations and defense (those went to ARPA, also created in 1958, per footnote 7).

### B. Growth and organization

- Eisenhower wanted the US to be _a_ leader, not _the_ leader, in space; he didn't commit to an all-out race.
- **Kennedy, May 25, 1961** (after Alan Shepard's flight) committed to landing a man on the moon and returning him safely **before the decade was out**. The US wasn't close to this capability, so it needed massive investment.
- **Budget:** about **$7 billion (2021$)** in 1961 (about 0.9% of federal spending) → peak about **$51 billion (2021$)** in 1966 (about **4.4%** of federal budget). (Nominal: $744M in 1961 and $5.933B in 1966.)
- After 1969 it declined but was still **1.92%** of federal spending in 1970, then 0.75–1% from 1975 on. For comparison, all nondefense federal R&D was only 1.5% of the federal budget in 2020.
- **Contracting out:** The 1958 Act let NASA contract with individuals, firms and agencies. First administrator **T. Keith Glennan** favored contracting out, partly from aversion to a bigger government payroll and partly to build a "national team" and invigorate the aerospace industry.
- **Employment:** In-house NASA staff grew 10,200 (1960) → 34,300 (1965). Contractor staff grew 30,500 (1960) → **peak 376,700 (1965)**. Private contractors were **90%** of NASA-related employment in 1965; universities only **1.7%**.
- By 1988, total NASA workforce was 52,224 (56% contractors).

### C. NASA contractors

- Winning the race meant building actual products. In the FY1967 input-output table, the **top five manufacturing sectors got about half of NASA spending**: aircraft & parts (SIC 372), electrical equipment (361–366), computers & office equipment (357), industrial inorganic chemicals (281), instruments (381–387).
- Few prime contractors: in 1965 the **top ten got nearly 70%** of contract spending. Examples: North American Aviation, Boeing, Grumman, Douglas, General Electric, McDonnell, IBM, RCA.
- **Geography was politically touchy** (most dollars went to a handful of states). NASA's answer: _competence of the contractor, not location_, decided awards. Reason: lives were at stake. Marshall Space Flight Center demanded contractors move from "mass production with acceptable errors" to "do it right the first time, with no error."

### D. Technology impacts

- Winning didn't mean inventing wholly new technology so much as **combining or speeding up existing technologies** (Robbins et al. 1972).
- Many NASA patents looked narrow (space capsule design, navigation/guidance, moon-landing apparatus).
- Still, breakthroughs in **cryogenics, integrated circuits, digital communications, computer simulation** could spill over.
- NASA claims over 2,000 **spinoffs** (e.g., MRI, remote sensing, gas analyzer, circuit connector).

---

## 4. Data Construction and Descriptive Statistics (Section II)

Three components: (i) CIA documents matched to pre-Sputnik US patents, (ii) NASA contractor spending and patents, (iii) census manufacturing data.

### A. Space technologies and space-capable places

- **Why not use NASA's own tech choices?** They reflect mission needs _and_ places where the US was already superior, which may have grown anyway. NASA may have just "harvested" potential.
- **So use Soviet choices** from digitized CIA national intelligence estimates of Soviet space capabilities (1947–1991). Main measure uses **post-1958 documents** (more exclusively about space).
- **How matching works:** Compute **term-frequency cosine similarity** (on a set of scientific terms) between each CIA document and each pre-1958 US patent. This captures tech similarity regardless of USPTO classification.
- **Figure 3** shows example patents similar to CIA documents (pop-up fins, missile guidance, orbital devices, satellites, space rendezvous).
- **Space capability score** = aggregate similarity across all pre-1958 patents in an industry-county cell.
- Footnote 14: Frequent terms in NASA patents include "aircraft," "antennae," "propellant." In CIA reports: "missiles," "satellites," "orbitals."

### B. NASA contractor spending and patents

- **Spending:** Digitized NASA's historical databooks: company names, contract amounts, place of performance and HQ for the **top 100 primary contractors, 1963–1992**. Top 100 firms = **87–92%** of contractor spending. **Transportation equipment and electronics ≈ 90%** of manufacturing contractor spending. Big metro examples: Los Angeles County, Nassau County NY, Hamilton County (Cincinnati) OH.
- **Patents:** Patents owned or funded by NASA. Pre-1976 from Fleming et al. (2019); post-1976 from USPTO. Locations from HistPat (pre-1975) and PatentsView (post-1975). Multi-location patents are split proportionally.
- **Measurement limitation:** Before **Bayh-Dole (1980)**, agencies had different patent policies. NASA's law gave the government all rights, but the administrator could **waive** rights to contractors. If contractors lobbied for waivers, NASA patents would be mismeasured. (Waivers became "essentially automatically granted" by early 1980s.) Footnote 28: checking against NASA's internal list suggests NASA mostly followed a "title policy," so measurement is reasonably good. **That's why they use both spending and patents.**
- **Military patents problem:** Army and Navy were "license agencies" (contractors got patents), so military innovation is undercounted. They build a new military-patent measure by searching patent text for terms from a military technology glossary.

### Figure 1 takeaways (text)

- Real NASA spending peaked **1965**, fell **>50%** by mid-1970s, rose steadily after but never matched peak.
- NASA patents were very low before 1958 (few early ones are from NACA, NASA's predecessor). Patents per year rose from **21 (1961) to 256 (1969)**; fluctuated **150–300** from 1967 onward.
- Contractor spending fell after the mid-1960s peak, but **patenting stayed elevated**.

### C. Manufacturing data

- Census of Manufactures at industry-county level: digitized **1947, 1954, 1958, 1963, 1967, 1972**; existing digital sources for **1977, 1982, 1987, 1992**.
- Variables: total value added, employment, wages, plant and equipment additions.
- Unit: **two-digit SIC industry (1972 definition)** × county. (Three- and four-digit data have too much masked/missing data.) Stops at 1992 because 1997+ uses NAICS and the focus is the Cold War.

### D. Additional data

- Skill (population census), research scientists (National Register of Scientific and Technical Personnel), **IBM mainframes** installed, defense spending, transportation costs.

### E. Sample selection

- Based on counties and industries in the census of manufactures. Excluded: counties with no 1945–1958 patents (can't compute score) and counties not in an MSA (standard errors clustered at MSA level).
- Cell must report in the **1958 census** and in **at least 8 censuses**; both value added and employment must be reported; at least one industry-county in the county must be space related; drop ND, SD, WY (only one reporting county).
- **Final sample: 6,759 industry-county observations, 86 counties, 19 two-digit SIC industries, 1947–1992.**
- **Figure 4:** map of space capability scores. Space-capable places are spread across the country, with a small cluster in the northeast.

### Table 1: balance in 1958

- Compares above vs. below median space capability (cols 2–3) and space vs. non-space industries (cols 5–6), with p-values for differences (cols 4, 7) and the difference-in-differences (col 8).
- **Takeaways:** Treated and control groups are quite similar. High-capability places had somewhat higher labor income, more navy patents and higher skill. Space vs. non-space industries differ only in labor income and total patents. In the "difference between differences" only **navy patents** are significantly different.
- Sample means: value added $72 million (1958$), employment 7,760, labor income $4,832, 735 industry-counties in 1958 (76 space industry, 659 non-space).
- **Conclusion:** triple-difference treatment and control groups were **balanced** in 1958.

---

## 5. Local Effects of Public R&D (Section III)

### A. Conceptual framework

- Space spending can raise local manufacturing output in two ways: (1) **local fiscal multiplier** (ordinary demand effect) or (2) **technological spillovers** raising productivity in the same industry or neighboring industries.
- Effects may build up **over time** or spread **across locations**.
- Neighbors could gain (demand for their goods, tech gains) or lose (**labor migrating** to space-active areas). The net size decides if the local multiplier equals the national effect.

### B. Empirical approach: the triple-difference model (Equation 1)

Y_ijt = β1 + β2 HighSpace×SpaceRace + β3 HighSpace×PostSpaceRace + **β4 HighSpace×SpaceRace×SpaceIndustry** + **β5 HighSpace×PostSpaceRace×SpaceIndustry** + (Pre-1958 Patents × year FE) + county FE + industry FE + year FE + error

- **i** = county, **j** = industry, **t** = year.
- **High Space Capability** = 1 if the similarity between pre-1958 patents and post-1958 CIA documents is **above median**.
- **Space Race** = 1 for 1959–1972; **Post-Space Race** = 1 for 1973–1992. (Census years used in tables: space race = 1963, 1967, 1972; post = 1977, 1982, 1987, 1992.)
- **Space Industry** = 1 for **transportation or electronics** (identified from NASA's actual demand).
- **Fixed effects** absorb time-invariant county/industry traits. **Pre-1958 patents × year** controls for trends from baseline innovation level. Some versions add **MSA × year FE**.
- **Standard errors:** two-way clustered at **MSA × industry**.
- **Coefficients of interest: β4 and β5.**
    - For NASA spending: expected positive (more NASA activity in specialized places after 1958), and larger during the race than after.
    - For manufacturing: positive if NASA spending caused growth. If it was **just a demand shock** (fiscal multiplier), effects should **fall** after NASA scaled down. If it was a **technology shock with slow spillovers**, effects should **grow over time**.
- **Key assumption:** Industry-counties that specialized in space-relevant research before 1958 did not get more NASA activity until after the race began. Plausible since the decision to go to the moon came after Sputnik, and funding was highly targeted at two sectors (transportation + electronics = **89%** of contractor funding).
- Can't check pre-trends for NASA spending (NASA didn't exist), but they check pre-trends in manufacturing later.
- Footnote 26: the triple difference captures NASA's decision logic: sectors were chosen by mission demands (transportation and electronics were _required_), and within them, suppliers with space-capable tech were selected.

### C. Results: NASA spending and patents (Table 2) (this is the "first stage")

- **Panel A (extensive margin; any NASA spending = 1):** β4 ≈ 0.07 and β5 ≈ 0.08 for spending; for patents 0.05 (race) and 0.12 (post), all precise. Non-triple interactions ≈ 0.
- **Panel B (PPML, intensive margin):** Preferred estimate (column 1): NASA spent **$264 million more during** and **$240 million more after** the race (1958$) in industry-counties with strong prior space-related research. These magnitudes feed the multiplier calculation.
- **Patents:** Positive and precise in Panel A, but **post-race effects are more than double** the race-period effects. PPML on patents shows no significant intensive-margin effect.
- **Interpretation:** Contractor spending effects fall after the race, but patenting effects stay or grow, suggesting it **takes time for contractor activity to turn into innovations** (consistent with Robbins et al. 1972). Caveat: patent attribution to NASA is measured with error, especially when **government interest statements weren't required** (footnote 28).
- Footnote 27: annual dynamic series for NASA patents shows no pre-trends. Footnote 21: patent-level space score strongly predicts NASA ownership/funding of a patent; NASA spending and NASA patenting are spatially correlated, though less than expected due to measurement problems.

### D. Results: Manufacturing (Table 3)

|Outcome|β4 (space race)|β5 (post-race)|
|---|---|---|
|log(value added)|0.35 (0.06) / 0.38|0.38 (0.08) / 0.36|
|log(employment)|0.42 / 0.45|0.36 / 0.34|
|log(capital)|0.31 (0.13) / 0.25 (0.15)|0.56 / 0.50 (larger post-race)|
|log(TFP)|−0.04 / −0.03|−0.02 / −0.02 (not significant)|

(Pairs of numbers = without / with MSA × year FE. The double-interaction rows, β2 and β3, are close to zero in all columns.)

- **Value added (cols 1–2):** Grew faster in space sectors in places with pre-Sputnik capability. Point estimates **similar during and after** the race. This fits demand stimulus continuing along with post-race contractor spending. **Not strong evidence of larger long-term gains from knowledge accumulated.**
- **Employment (cols 3–4):** Similar pattern; effects larger and more precise during the race.
- **Capital (cols 5–6):** Post-race effects **larger**, consistent with capital building up with a lag.
- **Productivity (cols 7–8):** Since value added, employment and capital effects are similar in size, little productivity effect is suggested. TFP is estimated from a production function Y = A·K^α·L^β by OLS (revenue-based TFP). Effects are **near zero and even slightly negative**. Caveats: revenue-based, doesn't handle endogenous input choices. Conclusion: **little evidence of positive productivity effect or tech spillovers.** (Footnote 29: revenue changes mix quantity, quality, and quality-adjusted price, which can't be separated.)

### E. Prior trends (Figure 5, Equation 2)

- Dynamic version of the model with **1958 as base year**, plotting year-by-year coefficients with 95% confidence intervals.
- **1947 and 1954 coefficients ≈ 0 and not significant**: no evidence of pre-trends. Supports the design.
- Figure 5 shows value added, employment and capital jump positive from 1963 on and stay positive; TFP stays near zero throughout.
- Footnote 30: the main-effect coefficients (High Space Capability × Year alone) are also near zero, supporting the idea of using NASA-revealed demand to define the space industry.

### F. Military activity and skills (Table 4)

- Worry: Cold War military research and skill growth might correlate with NASA activity.
- **Panel A (military controls):** Army and Navy patents (from Fleming et al.), then **military spending** (county) and **1962 defense-funded scientists × year**. Results barely change. Footnote 31: military and NASA patents are weakly spatially correlated, so this isn't surprising. Footnote on Bayh-Dole: military patents are undercounted because defense funders were "license agencies."
- **Panel B (skill controls):** Nonproduction worker share (industry-county-year, but mixes occupation and education), **1960 high school graduate % × year**, then **1962 research scientists × year** (upper-tail skill; Squicciarini & Voigtländer 2015) and **1961 IBM mainframes × year** (advanced IT). Results stay largely unchanged.
- **Conclusion:** Manufacturing results are highly robust to local military activity and human capital.

### G. ⭐ Multipliers

- Formulas:
    - **Space Race Output Effect** = β4(VA) × mean value added × output/value-added ratio (the ratio is used because total output isn't available before 1967).
    - **Space Race Spending Effect** = β4(Spending) × mean NASA spending (from Table 2, Panel B, col 1).
    - **Local multiplier** = Output Effect ÷ Spending Effect (same for the post-race period).
    - They exclude β2 and β3 since spillovers to non-space industries are estimated to be zero.
- **Results:** **0.3 during the race (1958–1972)** and **0.4 after (post-1972)**.
- **Comparison:** Below Ramey's general government spending multipliers of **0.6–0.8**; in the **low range** of military multipliers (**0.3–1.2**).
- **Interpretation:** Small relative to other spending, and **does not rise over time**, so little local technological spillover. Mission-oriented NASA R&D "failed to produce robust spillovers to the broader economy."
- **Caveats:**
    1. Doesn't account for effects on other industries/locations or **how spending was financed**.
    2. **State dependence:** the 1960s were a boom, so effects may have been larger in the slower late 1970s–80s.
    3. Excludes NASA spending at **universities and NASA research centers**, which may be more basic-research-intensive. If spillovers came from there, the aggregate effect is understated. So treat estimates as a **lower bound**.
- Footnote 32: Ramey (2021) shows long-term multipliers are larger when public investment has larger productivity effects and the economy is below optimal public investment; public R&D may fit those conditions.

### H. Robustness checks (supplemental appendix)

- Results robust to **county- and industry-specific time trends**. A highly saturated model with **industry-county FE** weakens value added and employment effects (limited time dimension) but not capital (Table A8).
- **Broader space industry definition** (add printing & publishing, and instruments): same conclusions (Table A9). These are the top four space-capable industries, but only transportation and electronics were heavily demanded by NASA.
- **Clustering** at other levels and spatial correlation (A10); heterogeneous-effects estimators (de Chaisemartin & D'Haultfoeuille, A11); dropping one state or industry at a time (Figures A3–A6); productivity in growth rates (A12).
- **IV:** Dummy for receiving funding in year t as endogenous variable gives precise estimates of **4.96–6.10** on contractor spending for all outcomes except productivity (A13).
- **National industry totals** (include non-local effects but weaker design): space industries were **larger but not more productive** after Sputnik (A14).
- **Spillovers to non-space industries:** Non-space-only sample shows little effect of pre-1958 space capability after the race began (A15). Little evidence of spillovers to colocated non-space neighbors.
- **Alternative capability measure:** compare post-Sputnik NASA patents with **US** space technology locally before Sputnik; similar estimates and no pre-trends (A16, Figure A7).
- **Text-processing variations**, treatment assignment rules, which CIA documents used (A17); military technology glossary similarity (A18). Results hold.

---

## 6. Spatial Spillovers of Public R&D (Section IV)

- **Why this matters:** The local estimates may not equal the national effects. If a place-based spending boost just pulls labor from elsewhere, the local effect **overstates** the national one. If there are demand or tech spillovers across areas, the local effect **understates** it.
- Footnote 34: Ramey (2019) and Chodorow-Reich (2019) discuss how migration can make local ≠ national multipliers, but most evidence is about **less persistent shocks**. NASA was a persistent shock, so migration is more likely here.
- Footnote 35 example: Houston's Manned Spacecraft Center (renamed Johnson Space Center, 1973) hired almost all technical and clerical workers locally, but only **10% of the 6,000 scientists, engineers and administrators** came from the Houston area. Within five years, **over 125 tech firms** (GE, Honeywell, IBM, North American Aviation, Lockheed, Raytheon, TI, TRW) opened Houston offices.

### A. ⭐ Inventor migration

- **Challenge:** No individual panel data for the 1940s–60s (footnote 37). Solution: a **disambiguated panel of patent inventors** (Akcigit et al. 2022 procedures), unique IDs for US inventors, 1945–1992.
- **Approach follows Moretti & Wilson (2017)** with three differences:
    1. County-to-county flows **within an industry** at county × industry × patent **application year** level.
    2. Includes time-invariant **space technology scores** interacted with space-era and space-industry dummies.
    3. Larger sample: inventors in the **top 50%** of producers, which allows industry variation.
- Footnote 38: they chose Moretti-Wilson over Akcigit et al. due to computational burden at the county level. Footnote 39: application year is used (closer to the time of innovation); each inventor's industry is their modal industry.
- **Equation 3:** log odds ratio of moving from origin _o_ to destination _d_ in industry _j_ = η1–η4 on (log space score at destination − log space score at origin) interacted with space race, post-race, and space industry dummies, **plus** controls for differences in personal income tax rates, corporate tax rates and R&D tax credits, plus FE for origin, destination, origin-destination pair (distance, travel costs), application year, industry, and pre-1958 patents (origin and destination) × year.
- **η3 and η4** are the coefficients of interest; expected **positive** if NASA spending pulled inventors toward space-capable places.
- Standard errors: three-way clustered by origin county × year, destination county × year, and county pair.
- **Table 5 results (all three columns similar):**
    - η3 (space race × space industry): **0.27–0.28** (significant).
    - η4 (post-race × space industry): **0.68 → 0.62 → 0.52** (larger after the race, suggesting migration takes time).
    - Col 2 adds tax controls; col 3 adds origin-state and destination-state × year FE. Results hardly change. 11,950 observations.
- **Conclusion:** Space race spending in space industries led inventors to **migrate toward opportunity**, consistent with the employment effects in Table 3 and historical accounts.
- **Side finding:** The main (non-triple) space capability coefficient is **negative and significant during the race** (about −0.13 to −0.15). Non-space inventors may have faced **competition for scarce lab resources/opportunities**. Left for future research.

### B. Including market effects

- Question: How do migration, demand and technology spillovers combine to shape the **national return**?
- They extend Donaldson & Hornbeck's (2016) county-to-county trade model (Supplemental Appendix Section 4; footnote 41: focus on public R&D, holding transport infrastructure fixed and adding market-level consumption externalities).
- **Equation 4** adds **High Space Market** terms (county-industry has above-median space-score-based market measure) with the same interactions. **β8 and β9** capture market-level effects of space activity **elsewhere**.
- **Table 6 results:**
    - Local effects barely change (e.g., value added β4 ≈ 0.32–0.38, β5 ≈ 0.42–0.49), still precise.
    - Market effects (β6–β9) are **close to zero**, imprecise, with signs depending on outcome and specification.
- **Interpretation:** No net market effects is consistent with **worker mobility to space county-industries offsetting** positive demand/technology spillovers. So the **local impact is a reasonable proxy for NASA's impact on the broader economy.** National ≈ local multiplier.

---

## 7. Conclusion (Section V and p. 2922)

- The moon landing (1969) was a milestone for US technological leadership, yet there had been **no credible empirical estimate** of its economic contribution.
- Using new data and a novel identification strategy based on geopolitical tensions, they find **economically meaningful, stable, precisely estimated** effects on long-term manufacturing growth in the **space sector**.
- But the effects are **fairly modest** and **no larger than other non-R&D government expenditures**.
- **Cautions on generalizing:**
    - Mowery, Nelson & Martin (2010): mission-oriented R&D is unusually focused and centralized. Non-mission-oriented public R&D might have different returns.
    - Contractor-spending focus gives a tight design and covers most NASA spending but may **miss spillovers** from NASA centers and universities (more basic science).
- **Policy lesson:** Growth depends on many factors (public and private R&D, human and physical capital, infrastructure, culture, geography, institutions, luck). The space race shows **limits of public R&D in generating growth**. The US government now invests a tiny fraction in non-military R&D compared to the Cold War peak. For those calling for a new "Sputnik Moment," the paper offers **cautionary lessons**.

---

## 8. Quick Revision Sheet

**Key numbers**

- NASA: 0.7% of GDP (mid-1960s); 400,000+ workers; budget share 0.9% (1961) → 4.4% (1966)
- Contractor employment peak: 376,700 (1965); contractors = 90% of NASA employment
- Top 10 contractors ≈ 70% of spending (1965); top 100 = 87–92%
- Transportation + electronics ≈ 89–90% of contractor spending
- Sample: 6,759 obs; 86 counties; 19 industries; 1947–1992
- NASA spent $264M (race) and $240M (post) more in high-capability space-industry cells
- Value added effects ≈ 0.35–0.38 log points; TFP ≈ 0
- **Multiplier: 0.3 (race), 0.4 (post)**; Ramey: 0.6–0.8; military: 0.3–1.2
- Migration: η3 ≈ 0.27; η4 ≈ 0.5–0.7

**Key terms**

- **Triple difference:** high vs. low space capability × space vs. non-space industry × before vs. during/after the race
- **Space capability score:** textual similarity between pre-1958 US patents and CIA descriptions of Soviet space tech
- **Technology harvesting:** NASA picked already-capable firms (the endogeneity problem)
- **Local vs. national multiplier:** differ if there is migration (overstates national) or cross-area spillovers (understates national)
- **PPML:** Poisson pseudo-maximum likelihood (handles zeros and intensive-margin spending)
- **Bayh-Dole Act (1980):** uniform patent policy; before it, agencies differed (NASA = title with waivers; Army/Navy = license)