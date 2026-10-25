## Notes: R&D Spillovers and the Geography of Innovation and Production
[[Primary Research Paper 1]]
**Authors:** #DavidBAudretsch & #MaryannPFeldman  
**Journal:** The American Economic Review, Vol. 86, No. 3 (June 1996), pp. 630–640

---

### 1. Main Objective / Research Questions

The paper’s core purpose is to examine two linked things:

- To what extent does **industrial activity cluster spatially** (geographically)?
- To link this **geographic concentration to the existence of knowledge externalities (spillovers)**.

Key underlying research questions:

- Does innovative activity cluster geographically more in some industries than others?
- Is this clustering simply because **production itself** is geographically concentrated (i.e., innovation just follows factories)?
- Or does clustering happen **because of knowledge spillovers** — i.e., because being close to the source of new knowledge (R&D labs, skilled workers, university research) matters, independent of where production is located?

The central hypothesis: **Innovative activity will cluster more in industries where new economic knowledge (knowledge spillovers) plays a bigger role — even after controlling for where production is located.**

This directly builds on and tests an assumption used but never tested in earlier studies (Jaffe 1989; Acs et al. 1992, 1994; Feldman 1994a) — that knowledge spillovers cause geographic clustering of innovation. No one before this paper had actually tested this “propensity to cluster” claim.

---

### 2. Research Design

**On the basis of enquiry:**  
Empirical, quantitative research — uses real data and statistical/econometric modeling (not theoretical/conceptual only, though it builds on theory from Marshall, Krugman, Arrow).

**On the basis of objective:**  
Descriptive + Explanatory (causal) research:

- Descriptive part: mapping/measuring where innovation and production are located (Figure 1, Tables 1 & 2).
- Explanatory part: testing WHY certain industries cluster more than others using regression models (Tables 5 & 6).

**On the basis of applicability:**  
Applied economic research — meant to inform economic geography, industrial policy, and regional innovation policy (they specifically mention that “state” is used as the unit because it’s the most relevant level for policy-making).

**Unit of Observation:** The **state** (crude proxy for the “true” economic market, but chosen because it matches available data and is the policy-relevant unit). Authors acknowledge (citing Krugman) that “states aren’t really the right geographical units” since they don’t match actual economic market boundaries.

---

### 3. Data Sources (in detail)

|Data / Variable|Source|Year Data Collected|Description|
|---|---|---|---|
|Innovation counts|U.S. Small Business Administration’s Innovation Data Base (SBIDB)|Compiled/data year: **1982**|8,074 commercial innovations recorded in the US; compiled by a private firm, **The Futures Group**, which also did quality control. Sourced from new product announcements in over 100 technology, engineering, and trade journals covering every industry.|
|Innovation-by-state/location detail|Edwards and Gordon (1984) — “Characterization of Innovations Introduced on the U.S. Market in 1982”|1982/1984|Distinguishes location of the _innovating establishment_ vs. location of the larger parent company (headquarters).|
|Usable manufacturing innovation data|Same SBIDB|1982|Total manufacturing innovations = 4,476; of these, 276 excluded (foreign-developed or missing location info) → final usable sample = **4,200** manufacturing innovations with location info.|
|Production/value-added data (Gini of production)|U.S. Department of Commerce, Bureau of the Census — **1982 Economic Census**|1982|Industry value-added by state, normalized by state’s share of total manufacturing value-added.|
|Natural resources share|Input-output data from **U.S. International Trade Commission databank**|**1976**|Share of total industry inputs purchased from mining and agriculture.|
|Scale (establishment size)|U.S. Department of Commerce, Bureau of the Census|**1982**|Mean size of largest establishments accounting for half of industry value-of-shipments, divided by industry value of shipments.|
|Transportation costs|Commodity Transport Survey of the U.S. Census of Transportation, via Weiss (1991)|**1967**|Radius of mean distance shipped.|
|Industry R&D/Sales|Line of Business Survey, **U.S. Federal Trade Commission**|**1977**|R&D expenditure divided by sales.|
|Skilled labor share|U.S. Department of Commerce, Bureau of the Census|**1970**|Share of industry employment made up of professional/kindred workers, managers, administrators, craftspeople.|
|University research|Yale Survey of Industrial Managers (Levin et al., 1987) + National Science Foundation (NSF) Survey of Science Resources|1987 (survey)|Expenditure on university research relevant to specific industries, mapped using a **relevance survey (Likert scale 1–7)** of what academic disciplines matter to which industries. Departments rated above a relevance score of 5 were considered relevant.|

**Sample size for regression analysis:** 163 four-digit SIC (Standard Industrial Classification) manufacturing industries — the number of industries for which comparable data across all these different measures could be compiled.

**Note on mismatched years:** Data comes from different years (1967, 1970, 1976, 1977, 1982, 1987) — all pooled together as if representing a stable snapshot of industry characteristics. This is a limitation.

---

### 4. Analytical / Statistical Method

#### Step 1: Measuring Geographic Concentration — Gini Coefficients

- Following **Krugman (1991b)**, they calculate **Gini coefficients** to measure how geographically concentrated (a) production and (b) innovation are, for each industry.
- **Gini of Production:** Based on industry value-added by state, normalized by that state’s share of total manufacturing value-added. A coefficient of 0 = no extra concentration beyond overall manufacturing distribution; closer to 1 = more concentrated.
- **Gini of Innovation:** Same logic, but based on count of innovations by state and industry.
- Cases where state/industry data were suppressed were excluded.

#### Step 2: Regression Models

- **OLS (Ordinary Least Squares) regressions** — Table 5. Six equations:
    - Equations (1)-(3): Gini of Production as dependent variable.
    - Equations (4)-(6): Gini of Innovation as dependent variable.
- **3SLS (Three-Stage Least Squares) regressions** — Table 6, used because Gini of Production and Gini of Innovation are **endogenous to each other** (each affects the other — simultaneity problem).
    - They also tested **2SLS (Two-Stage Least Squares)** first; because standard errors differed (indicating **cross-equation correlation**), they settled on 3SLS as the more appropriate method.
    - Instruments used: all exogenous variables on the right-hand side of the model’s equations.

#### Key Independent (Explanatory) Variables Used:

1. **Natural resources** — industries dependent on natural resource inputs are expected to be more geographically concentrated (near the resource).
2. **Scale** — capital-intensive industries with big minimum efficient scale (MES) expected to be more concentrated.
3. **Transportation costs** — inversely related to mean distance shipped; higher transport cost → lower geographic concentration of production.
4. **Industry R&D/Sales** — proxy for how R&D-intensive (and thus how spillover-prone) an industry is.
5. **Skilled labor** — proxy for human capital as a channel of knowledge transmission.
6. **University research** — proxy for the “pool” of relevant basic science knowledge available to an industry.
7. **Gini of Innovation / Gini of Production** — used as cross-variables to test whether one drives the other.

#### Correlation Matrix (Table 4)

- Checked pairwise correlations between all variables (Gini of production, Gini of innovation, natural resources, scale, transportation costs, R&D/sales, skilled labor, university research) before regression, to understand relationships and check for multicollinearity concerns (note: University research and Gini of production have a very high correlation of 0.8730).

---

### 5. Main Points of the Paper

- Innovation and technological change depend heavily on **new economic knowledge**, and this knowledge **“spills over”** — i.e., firms and universities investing in R&D create knowledge that benefits third parties too (building on Jaffe 1989, Acs et al., Feldman).
- As **Marshall (1920)** and **Krugman (1991b)** argued, there may be **geographic limits** to how far information/knowledge flows — especially **tacit knowledge**. Cost of transmitting _information_ may not depend on distance, but cost of transmitting _knowledge_ likely rises with distance. So **proximity matters**.
- Before this paper, no one had tested whether innovative activity actually has a tendency to **cluster spatially**, even though many theoretical models assumed it.
- To explain why innovation clusters in some industries more than others, you must FIRST control for whether **production itself** is concentrated in that industry — otherwise you can’t tell if clustering of innovation is due to knowledge spillovers or just because factories happen to be clustered there.
- Because knowledge externalities can’t be measured directly, the authors use **R&D intensity (R&D/Sales)** as a proxy — following **Arrow (1962)**’s argument that spillovers matter more in R&D-intensive industries.
- **Skilled labor** is treated as another channel/mechanism through which knowledge transmits (skilled/educated workers carry and diffuse tacit knowledge).
- **University research** relevant to an industry is another proxy for the availability of new economic knowledge.
- Other (non-knowledge) factors that shape geographic concentration of _production_ specifically: natural resource dependency, transportation costs, and scale economies/capital intensity.
- Figure 1 shows innovations are heavily concentrated on the **coasts**, especially **California and New England**; almost no innovation registered in states like **North Dakota, South Dakota, Montana, Wyoming**; traditional manufacturing belt states (Ohio, Illinois, Michigan, Pennsylvania) are **not particularly innovative** despite having lots of manufacturing.
- Table 1 shows specific industries have extremely high spatial concentration of innovation — e.g., **Computers**: 41.7% of all US innovations in California alone, another ~10% in Massachusetts (over half in just 2 states). **Pharmaceuticals**: ~40% in New Jersey, 14% in New York (over half in NJ-NY area).
- Table 2 shows manufacturing sectors with highest **production** concentration: primary metals, transportation equipment, textiles, food & beverages, leather, chemicals. Sectors with highest **innovation clustering**: transportation equipment, instruments, electronics. These lists don’t fully overlap — proving production concentration alone doesn’t explain innovation concentration.

---

### 6. Findings

- **Natural resource dependency** → significantly **increases** geographic concentration of production (positive, significant coefficient).
- **Scale economies** → industries with greater scale economies are actually **less**, not more, geographically concentrated in production (negative, significant coefficient) — contrary to what Shelburne & Bednarzik (1993) argued; authors suggest this might be because their measure only captures the US market while many industries are global.
- **Industry R&D intensity** → positive and statistically significant effect on **both** Gini of production and Gini of innovation. R&D-intensive industries cluster more, in both production and innovation.
- **Skilled labor** → positive and statistically significant effect on both Gini of production and Gini of innovation — supports the idea that human capital is a channel for spillovers.
- **University research** → positive, statistically significant effect specifically on Gini of innovation.
- When Gini of Innovation is added as an explanatory variable for Gini of Production (equation 2), its coefficient is **not statistically significant** — geographic clustering of innovation does NOT explain clustering of production.
- **Most important finding:** Even **after controlling for the geographic concentration of production**, industries with more R&D intensity, more skilled labor, and more relevant university research **still show a significantly higher tendency for innovation to cluster spatially**.
- This means: **the tendency of innovative activity to cluster geographically is driven more by knowledge spillovers themselves, and not merely because production/factories happen to be clustered there.**
- Results were **consistent across both OLS and 3SLS estimation methods** — strengthening confidence in the findings.
- Industries where knowledge plays a bigger role (high R&D, skilled labor, university research relevance) tend to have **both** greater production concentration AND greater innovation concentration — but the innovation clustering effect holds independently of the production clustering effect.

---

### 7. Drawbacks / Limitations of the Paper

- **Unit of observation (the state) is a crude/imperfect proxy** for the real economic market — the authors themselves admit, citing Krugman (1991b), that “states aren’t really the right geographical units” because state boundaries don’t match actual economic market boundaries. Ideal data would be at city or county level, but wasn’t available at the time.
- **Data years are mismatched/inconsistent** — variables are drawn from very different years: transportation cost data from 1967, natural resources data from 1976, R&D/sales from 1977, skilled labor from 1970, innovation and production data from 1982, university research survey from 1987. This creates a temporal inconsistency — treating industry “structural” characteristics as if stable over 10-20 years, which may not always hold.
- **R&D/Sales ratio is an imperfect (indirect) proxy for knowledge spillovers** — knowledge externalities cannot be directly measured, so the paper relies on an assumption (from Arrow 1962) that R&D intensity reflects spillover potential; this is a conceptual leap, not a direct/verified measurement.
- **Scale variable’s counterintuitive result** — the authors themselves note their measure “limits the size of the market to the United States,” which may understate true scale economies for industries that are global, potentially biasing this coefficient.
- **Sample size limited to 163 four-digit SIC industries** — only industries where ALL variables had comparable, non-suppressed data could be included; this could exclude many industries and introduce selection bias.
- **Simultaneity / endogeneity concerns** between Gini of Production and Gini of Innovation had to be addressed with 3SLS — this indicates that separating cause and effect between production location and innovation location is statistically tricky, and results may still not fully resolve the direction of causality.
- **University research variable has very high correlation (0.87) with Gini of Production** (seen in the correlation matrix) — this raises a **multicollinearity concern** that could affect the reliability/precision of coefficient estimates involving these two variables.
- **The SBIDB innovation database itself has limitations** — it draws from technology/trade journal “new product announcements,” which may not capture all innovations (especially non-commercialized, informal, or unpublicized innovations), and 276 manufacturing innovations had to be dropped due to missing/foreign location data.
- **Innovation counts don’t measure quality/value of innovation** — the database counts innovations but doesn’t weight them by economic significance, so a minor product tweak counts the same as a major breakthrough.
- **No control for firm size distribution within industries** across states, which could also influence clustering independent of knowledge spillovers.