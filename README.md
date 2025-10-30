# Startup Scale Potential Evaluation Model

**[Live Demo](https://lunarlunar.github.io/ScaleEval/index.html)**

---

## Abstract

This project provides an interactive, quantitative evaluation model designed to offer a structured framework for entrepreneurs, investors, and market analysts to assess the long-term scale potential of a startup. The core thesis of this model is that the ultimate scale of a successful startup is the product of **Product-Market Fit (PMF)** and **Resource Leverage**, multiplied by the ratio of **Team Competency** to **Systemic Risk**.

By employing a mathematical formula with exponential weights, this tool translates qualitative concepts into quantitative metrics. It is calibrated and validated against real-world case studies, such as the success of Notion and the failure of WeWork, to help users identify high-growth potential ventures and high-risk projects.

---

## Theoretical Foundation

The model is rooted in several widely accepted venture capital theories and business strategy principles:

1.  **Product-Market Fit (PMF) as the Core Engine:**
    Coined by Marc Andreessen, founder of Netscape, "Product-Market Fit" is considered the single most important factor for a startup's success (Andreessen, 2007). This model treats PMF as an exponential amplifier (α weight > 1) because a product that genuinely solves a market pain point has super-linear growth potential, driving organic traffic, word-of-mouth, and high user retention.

2.  **The Team as a Risk Buffer and Execution Amplifier:**
    An exceptional team is not merely an executor of plans but a "risk buffer" in a chaotic market. When faced with unpredictable challenges, the team's resilience, experience, and trust capital are the only elements that can navigate a company through crises (Horowitz, 2014). Therefore, Team Competency (β weight) plays the dual role of amplifying execution outcomes while mitigating risks.

3.  **The Double-Edged Sword of Resource Leverage:**
    Resources like capital and networks are growth accelerators, but their effectiveness is not infinite. This model references the economic concept of "diminishing marginal returns," setting the initial value for Resource Leverage (γ weight) to linear growth (γ ≈ 1.0). The case of WeWork serves as a stark warning that over-reliance on external capital leverage while ignoring fundamental business model flaws can lead to catastrophic failure.

4.  **The Exponential Penalty of Risk:**
    Startups often fail not from a lack of effort, but from uncontrolled risks. Nassim Taleb's "Black Swan Theory" reminds us that low-probability, high-impact events are the norm, not the exception (Taleb, 2007). This model intentionally positions Risk as a denominator with a strong exponential penalty (δ weight > 1.5), because a single fatal structural risk, governance failure, or funding chain collapse is enough to nullify all efforts.

---

## Interface Overview

The dashboard is divided into several key sections to guide your evaluation process:

### 1. Weight Index Settings
![Weight Index Settings](images/pic_Weight%20Index%20Settings.png)
This section is for calibrating the model's sensitivity. Here you can set the exponential weights (α, β, γ, δ) that determine the influence of each core factor on the final score. For convenience, you can load presets tailored for different industries, such as SaaS, Deep Tech, or Hardware, to start with a relevant baseline.

### 2. Startup Factor Scoring
![Startup Factor Scoring](images/pic_Startup%20Factor%20Scoring.png)
This is the primary input area where you score the startup on a scale of 1 to 10 across the four key dimensions: Product-Market Fit, Leverage, Team, and Risk. Each dimension is broken down into several sub-factors. Hovering over each sub-factor provides a detailed explanation of the scoring criteria to ensure a consistent evaluation.

### 3. Case Scoring Logic Explanation
![Case Scoring Logic Explanation](images/pic_Case%20Scoring%20Logic%20Explanation.png)
To provide context and a reference point, this table offers a transparent look at how iconic companies like Notion and WeWork are scored within this model. You can load these cases to see how different profiles result in varying scores, which helps in calibrating your own evaluations.

---

## The Core Model

**Formula: Scale Potential ≈ (PMF<sup>α</sup> × Leverage<sup>γ</sup>) × (Team<sup>β</sup> / Risk<sup>δ</sup>)**

-   **PMF (Product-Market Fit):** Measures the degree to which a product satisfies strong market demand.
    -   `P1: Pain Point Depth` - How severe is the problem you are solving?
    -   `P2: Product Differentiation` - What is your fundamental advantage over competitors?
    -   `P3: Iteration Quality` - How quickly and effectively does the team improve the product?

-   **Leverage (Timing & Resource Leverage):** Measures the efficiency of converting resources into scale.
    -   `L1: Timing Correctness` - Is now the perfect time for this venture?
    -   `L2: Network Capital` - How many influential people can you access?
    -   `L3: Hard Resources` - The scale of capital you can deploy.
    -   `L4: Soft Resources` - Intangible assets like brand, patents, and community.

-   **Team (Team Competency):** Measures the overall capability of the team.
    -   `T1: Execution Ability` - The ability to turn ideas into reality.
    -   `T2: Core Complementarity` - Do team members' skills and traits complement each other?
    -   `T3: Vision & Experience` - Is the team's vision ambitious and backed by relevant experience?
    -   `T4: Trust Capital` - How strong are the internal and external trust relationships?

-   **Risk (Competition & Risk Factor):** Measures potential fatal threats, both internal and external.
    -   `R1: Competition Intensity` - Is the market a red ocean or a blue ocean?
    -   `R2: External & Structural Risk` - Do you face regulatory hurdles or structural flaws in your business model?
    -   `R3: Governance & Funding Chain Risk` - Are there internal issues that could lead to failure?

### Exponential Weights (α, β, γ, δ)

-   **α (PMF Weight):** The core amplifier, typically the highest weight.
-   **β (Team Weight):** The execution and buffer amplifier, a high weight.
-   **γ (Leverage Weight):** The resource multiplier, usually linear or slightly above.
-   **δ (Risk Weight):** The strong penalty term, should be the highest negative weight to filter out high-risk ventures.

---

## How to Use

1.  **Open `index.html`:** Launch the file in your web browser.
2.  **Set Weights:** Based on the industry you are evaluating (e.g., General SaaS, Hardware), click the buttons at the top to load recommended weights or adjust α, β, γ, and δ manually.
3.  **Score the Factors:** In the four main sections (PMF, Leverage, Team, Risk), rate each sub-factor on a scale of 1-10. Hover over the titles for detailed scoring guidelines.
4.  **View the Results:** The "Final Scale" at the top will update in real-time, and the "Smart Explanation" below will dynamically generate a qualitative analysis based on your scores.
5.  **Reference Cases:** Use the "Load This Case" buttons to auto-fill the scores for Notion or WeWork to understand how the model evaluates these contrasting companies.

---

## Case Studies

| Company | Factor | Score (1-10) | Scoring Logic Explanation |
| :--- | :--- | :--- | :--- |
| **Notion** | PMF (High) | Pain(9), Diff(9), Iteration(9) | **Core:** Solved the deep pain of integration chaos; high customization is a strong differentiation. Fast and high-quality iteration. |
| | Team (High) | Exec(9), Comp(8), Vision(9), Trust(9) | **Buffer:** Founders could pivot and rewrite code, showing superb execution. High trust among core members was key to surviving crises. |
| | Leverage (Mid-Low) | Timing(8), Network(5), Hard(4), Soft(9) | **Efficiency:** Very low early hard resources (funding), but extremely high soft resources (community, IP value), leading to high resource efficiency. |
| | Risk (Low) | Comp(5), Struct(3), Gov(2) | **Controllable:** Despite facing giant competitors, SaaS has low structural risk, and internal management is extremely lean. |
| **WeWork** | PMF (Mid) | Pain(7), Diff(6), Iteration(4) | **Inflated:** Flexible office demand exists, but the model is essentially subleasing with low barriers. Iteration focused on expansion, not product optimization. |
| | Team (Very Low) | Exec(5), Comp(4), Vision(7), Trust(3) | **Flawed:** High vision, but core issues in corporate governance and extremely low execution efficiency (Trust Capital only 3 pts). |
| | Leverage (Very High) | Timing(8), Network(9), Hard(9), Soft(5) | **Leverage:** The founder's network and SoftBank's funding (hard resources) were extremely high, but resource efficiency was poor. |
| | Risk (Very High) | Comp(8), Struct(8), Gov(9) | **Out of Control:** Fierce competition, **structural risks (long-term lease debt)**, and **governance risks (CEO's self-interest, funding chain)** were off the charts. |

---

## References

-   Andreessen, M. (2007). *The Pmarca Guide to Startups, part 4: The only thing that matters*. PMarchive.
-   Blank, S. (2013). *The Four Steps to the Epiphany: Successful Strategies for Products that Win*. K&S Ranch.
-   Horowitz, B. (2014). *The Hard Thing About Hard Things: Building a Business When There Are No Easy Answers*. HarperBusiness.
-   Ries, E. (2011). *The Lean Startup: How Today's Entrepreneurs Use Continuous Innovation to Create Radically Successful Businesses*. Crown Business.
-   Thiel, P. (2014). *Zero to One: Notes on Startups, or How to Build the Future*. Crown Business.
-   Taleb, N. N. (2007). *The Black Swan: The Impact of the Highly Improbable*. Random House.
-   Graham, P. (2012). *Startup = Growth*. PaulGraham.com.

