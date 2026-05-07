# Journal Profiles

<!--
These profiles calibrate the domain-referee and methods-referee when reviewing
for a specific journal. Each profile describes the journal's review culture
in plain language — the LLM adapts its priorities accordingly.

Used by: domain-referee.md, methods-referee.md (via /review --peer [journal])
-->

## How This Works

When `/review --peer [journal]` is invoked:

1. **Editor reads the paper** → desk review (reject or send to referees)
2. **Editor selects referees** → draws dispositions and pet peeves from the journal's **Referee pool**
3. **Profile found below** → referees calibrate using the full profile
4. **Profile NOT found** → referees use the journal name + .claude/references/domain-profile.md to adapt (still better than generic)
5. **No journal specified** → generic top-field referee behavior

### Referee Pool Field

Each journal profile includes a **Referee pool** that weights which dispositions the editor draws from. The two referees always get DIFFERENT dispositions. Dispositions: STRUCTURAL, CREDIBILITY, MEASUREMENT, POLICY, THEORY, SKEPTIC (see editor.md for definitions).

### Table Format Convention

**Default:** All journals use standard economics table conventions — significance stars (`*` p<0.10, `**` p<0.05, `***` p<0.01), standard errors in parentheses, booktabs formatting. This default applies unless a journal profile below includes a **Table format** override.

**Exception — AEA journals** (AER, AEJ:Applied, AEJ:Policy, AER:Insights): No significance stars. Report standard errors in parentheses; use exact p-values or confidence intervals for key results. See the [AEA Style Guide](https://www.aeaweb.org/journals/aeri/style-guide) and content-standards.md for implementation details.

---

## Sociology

**World Sociology**

### American Sociological Review (ASR)
**Focus:** General sociology; stratification, organizations, culture, politics, race, gender, economic sociology, social psychology, methods
**Bar:** Extremely high. Requires a major theoretical and/or empirical contribution with broad disciplinary relevance.
**Domain referee adjusts:** Contribution to central sociological debates; generalizability beyond the specific case; theoretical innovation.
**Methods referee adjusts:** Very high rigor expectations. Strong causal identification, robustness checks, advanced quantitative methods or exceptionally rigorous qualitative designs.
**Typical concerns:** “What is the general sociological contribution?”; “Why should non-specialists care?”; “Is the causal claim justified?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (very high), MEASUREMENT (high), POLICY (medium), THEORY (very high), SKEPTIC (very high)
**Table format:** Clean professional tables; significance stars accepted.

### American Journal of Sociology (AJS)
**Focus:** General sociology with strong emphasis on theory, historical sociology, organizations, networks, culture, inequality
**Bar:** Extremely high. Prefers ambitious papers with long-term theoretical importance.
**Domain referee adjusts:** Depth of conceptual argument; connection to classical and contemporary sociological theory.
**Methods referee adjusts:** Rigorous but more methodologically pluralist than ASR; accepts historical and qualitative work if exceptionally deep.
**Typical concerns:** “Is the theory sufficiently developed?”; “Does the empirical material support the broader claims?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (high), MEASUREMENT (medium), POLICY (low), THEORY (very high), SKEPTIC (high)

### Annual Review of Sociology
**Focus:** Synthetic review articles across all sociological fields
**Bar:** Invitation-driven or highly selective proposals; requires authoritative synthesis of a literature
**Domain referee adjusts:** Coverage of literature; clarity of synthesis; identification of future research agendas
**Methods referee adjusts:** Less about original identification; more about accurate interpretation of evidence and literatures
**Typical concerns:** “Is the review comprehensive?”; “Does it fairly represent competing perspectives?”
**Referee pool:** STRUCTURAL (medium), CREDIBILITY (medium), MEASUREMENT (medium), POLICY (medium), THEORY (high), SKEPTIC (medium)

### Social Forces
**Focus:** General sociology with emphasis on empirical social science, inequality, demography, education, family, labor, stratification
**Bar:** Very high. Strong empirical contribution with clear sociological importance.
**Domain referee adjusts:** Relevance to ongoing empirical debates; contribution to cumulative knowledge.
**Methods referee adjusts:** Strong expectations for identification, modeling, robustness, and transparency.
**Typical concerns:** “Is the contribution incremental?”; “Are alternative explanations addressed?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (high), MEASUREMENT (high), POLICY (medium), THEORY (medium), SKEPTIC (high)

### European Sociological Review (ESR)
**Focus:** Comparative and international sociology; inequality, migration, education, welfare states, labor markets
**Bar:** Very high. Strong comparative contribution and methodological rigor.
**Domain referee adjusts:** Comparative leverage; contribution to European and global sociological debates.
**Methods referee adjusts:** High quantitative standards; replication logic and robustness expected.
**Typical concerns:** “Is the comparison theoretically meaningful?”; “Are institutional differences adequately modeled?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (high), MEASUREMENT (high), POLICY (medium), THEORY (medium), SKEPTIC (high)

**Latin American Sociology**

### Revista Mexicana de Sociología (RMS)
**Focus:** General sociology; inequality, labor, politics, social movements, culture, Latin American development
**Bar:** High regional prestige; strong theoretical grounding and empirical relevance required.
**Domain referee adjusts:** Relevance to Latin American debates; dialogue with regional intellectual traditions.
**Methods referee adjusts:** Moderate-to-high rigor; accepts qualitative, historical, and quantitative work.
**Typical concerns:** “Does the paper sufficiently engage Latin American scholarship?”; “Is the empirical evidence adequate?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (medium), MEASUREMENT (medium), POLICY (high), THEORY (high), SKEPTIC (medium)

### Dados
**Focus:** Political sociology, inequality, labor, state, democracy, development
**Bar:** Very high for Latin America; internationally visible.
**Domain referee adjusts:** Contribution to comparative and Brazilian/Latin American sociology.
**Methods referee adjusts:** Strong methodological expectations; quantitative sophistication increasingly valued.
**Typical concerns:** “Is the design rigorous enough for international standards?”; “Does it travel beyond Brazil?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (high), MEASUREMENT (high), POLICY (high), THEORY (medium), SKEPTIC (high)

### Sociedade e Estado
**Focus:** Social theory, labor, state, inequality, political sociology, contemporary capitalism
**Bar:** High. Strong conceptual framing expected.
**Domain referee adjusts:** Engagement with critical theory and contemporary sociological debates.
**Methods referee adjusts:** Pluralist; accepts qualitative and theoretical work with less emphasis on causal identification.
**Typical concerns:** “Is the theoretical framing coherent?”; “Does the empirical material sustain the interpretation?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (medium), MEASUREMENT (low), POLICY (medium), THEORY (very high), SKEPTIC (medium)

### Revista Latinoamericana de Estudios del Trabajo (RELET)
**Focus:** Sociology of work, labor markets, precarization, unions, informality, labor process
**Bar:** High within labor sociology; strong regional relevance required.
**Domain referee adjusts:** Contribution to Latin American labor debates; engagement with critical labor theory.
**Methods referee adjusts:** Mixed-methods friendly; empirical grounding required even in theoretical pieces.
**Typical concerns:** “Does the paper sufficiently situate the case in regional labor transformations?”; “Is the concept of labor/class adequately specified?”
**Referee pool:** STRUCTURAL (very high), CREDIBILITY (medium), MEASUREMENT (medium), POLICY (high), THEORY (high), SKEPTIC (medium)

### Caderno CRH
**Focus:** Labor, inequality, urban sociology, development, critical theory
**Bar:** High. Values theoretically informed empirical work.
**Domain referee adjusts:** Dialogue with dependency theory, critical sociology, and Brazilian social thought.
**Methods referee adjusts:** Moderate rigor expectations; qualitative and interpretive methods common.
**Typical concerns:** “Is the argument sufficiently grounded?”; “Does the paper contribute beyond description?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (medium), MEASUREMENT (low), POLICY (high), THEORY (high), SKEPTIC (medium)

**Argentinean Sociology

### Desarrollo Económico
**Focus:** Development, inequality, labor markets, political economy, class structure, economic sociology
**Bar:** One of the most prestigious Argentine social science journals; strong empirical and theoretical contribution required.
**Domain referee adjusts:** Contribution to debates on development and inequality in Argentina/Latin America.
**Methods referee adjusts:** Moderate-to-high methodological standards; quantitative rigor valued.
**Typical concerns:** “Is the contribution original?”; “Does the analysis sufficiently engage regional debates?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (high), MEASUREMENT (medium), POLICY (high), THEORY (high), SKEPTIC (high)

### Estudios del Trabajo
**Focus:** Sociology of work, labor markets, unions, employment, labor process, inequality
**Bar:** High within labor studies in Argentina.
**Domain referee adjusts:** Relevance to Argentine labor debates; engagement with labor sociology traditions.
**Methods referee adjusts:** Mixed methods accepted; empirical consistency expected.
**Typical concerns:** “Is the labor concept clearly operationalized?”; “Does the evidence support the interpretation?”
**Referee pool:** STRUCTURAL (very high), CREDIBILITY (medium), MEASUREMENT (medium), POLICY (high), THEORY (high), SKEPTIC (medium)

### Trabajo y Sociedad
**Focus:** Labor sociology, social structure, territory, inequality, labor precarity
**Bar:** Moderate-to-high. Strong empirical relevance valued.
**Domain referee adjusts:** Connection to labor transformations and Argentine social structure.
**Methods referee adjusts:** Flexible methodological standards; qualitative work common.
**Typical concerns:** “Is the argument sufficiently connected to broader debates?”; “Does the evidence go beyond description?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (medium), MEASUREMENT (low), POLICY (high), THEORY (medium), SKEPTIC (medium)

### Entramados y Perspectivas
**Focus:** Critical sociology, political sociology, labor, culture, inequality
**Bar:** High theoretical expectations within critical sociology traditions.
**Domain referee adjusts:** Depth of conceptual and political analysis.
**Methods referee adjusts:** Lower emphasis on formal causal identification; interpretive coherence matters more.
**Typical concerns:** “Is the theoretical framework internally coherent?”; “Does the empirical material substantiate the claims?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (medium), MEASUREMENT (low), POLICY (medium), THEORY (very high), SKEPTIC (medium)

### Revista Argentina de Sociología
**Focus:** General sociology; social theory, inequality, politics, education, labor
**Bar:** High national prestige; broad disciplinary relevance expected.
**Domain referee adjusts:** Contribution to Argentine sociological debates and traditions.
**Methods referee adjusts:** Methodological pluralism; rigor expectations depend on approach.
**Typical concerns:** “Is the contribution sufficiently sociological?”; “Does the paper engage relevant Argentine literature?”
**Referee pool:** STRUCTURAL (high), CREDIBILITY (medium), MEASUREMENT (medium), POLICY (medium), THEORY (high), SKEPTIC (medium)

---

## Add Your Own Journal

Copy this template and add it above this section:

```markdown
### [Journal Name] ([Abbreviation])
**Focus:** [fields and topics covered]
**Bar:** [what it takes to publish here]
**Domain referee adjusts:** [what matters most to domain reviewers at this journal]
**Methods referee adjusts:** [rigor expectations, preferred methods, required checks]
**Typical concerns:** [common referee questions at this journal]
**Referee pool:** [disposition] (high/medium/low) for each: STRUCTURAL, CREDIBILITY, MEASUREMENT, POLICY, THEORY, SKEPTIC
**Table format:** [optional — only include if journal deviates from default (stars OK). E.g., "No significance stars (AEA style)."]
```
