# On the Integration of Business Process Simulation and Predictive Process Monitoring

This repository contains the supplementary material for the paper  
**"On the Integration of Business Process Simulation and Predictive Process Monitoring"**, accepted at **EDOC 2026**.

## Literature Review

The screening form used in our systematic literature review is available here:  
https://github.com/robert-l-b/slr_BPS_x_PPM/tree/main/Screening%20Forms

## Classification of Included Papers

Our systematic literature review identified **32 papers** that integrate BPS and PPM. Below, we classify them along the three research questions.

### RQ1: What tasks are addressed by integrating BPS and PPM?

Among the 32 papers, 23 address process simulation, four focus on predicting future process performance, and five address prescriptive tasks.

| Task Classification | Count | Papers |
|---|---|---|
| **As-is simulation** | 14 | Pandey et al. (2012), Bergmann et al. (2014), Fauzan et al. (2019), Camargo et al. (2019), Mesabbah et al. (2020), Rashid et al. (2022), de Leoni et al. (2023), Meneghello et al. (2023), Lopez-Pintado et al. (2024), Kirchdorfer et al. (2025), Vinci et al. (2025, online), Vinci et al. (2025, reliable), Graziosi et al. (2025), Özdemir et al. (2026) |
| **What-if simulation -- concrete application** | 5 | He et al. (2014), Tangkawarow et al. (2018), Elbattah et al. (2018), Chang et al. (2018), El Kassimi et al. (2024) |
| **What-if simulation -- no specific task** | 4 | Pourbafrani et al. (2022), Camargo et al. (2023), Oyamada et al. (2024), Buliga et al. (2025) |
| **Predict performance** | 4 | Rieke et al. (2010), Solomon et al. (2011), Ruschel et al. (2020), Chinnathai et al. (2023) |
| **Prescribe action** | 5 | Weinzierl et al. (2020), Padella et al. (2024), Meneghello et al. (2024), De Moor et al. (2025, ProCause), De Moor et al. (2025, SimBank) |

### RQ2: How are BPS and PPM integrated?

We distinguish between asymmetric and symmetric integration patterns. In asymmetric patterns, one technique acts as the client and leverages the other as a supporting component. When BPS is the client, predictive models may provide input (P1), be embedded within the simulation workflow (P2), or be applied to simulation outputs (P3). When PPM is the client, simulation may generate input (P4), be integrated within the predictive pipeline (P5), or be applied to prediction outcomes (P6). Pattern P7 captures symmetric integration.

| Integration Pattern | Count | Papers |
|---|---|---|
| **P1** -- PPM provides input to BPS | 8 | Tangkawarow et al. (2018), He et al. (2014), Elbattah et al. (2018), Chang et al. (2018), Fauzan et al. (2019), Pourbafrani et al. (2022), Camargo et al. (2023), Kirchdorfer et al. (2025) |
| **P2** -- PPM embedded within BPS workflow | 13 | Bergmann et al. (2014), Camargo et al. (2019), Mesabbah et al. (2020), Rashid et al. (2022), de Leoni et al. (2023), Meneghello et al. (2023), El Kassimi et al. (2024), Lopez-Pintado et al. (2024), Oyamada et al. (2024), Buliga et al. (2025), Vinci et al. (2025, online), Vinci et al. (2025, reliable), Graziosi et al. (2025) |
| **P3** -- PPM applied to BPS outputs | 1 | Özdemir et al. (2026) |
| **P4** -- BPS generates input for PPM | 4 | Ruschel et al. (2020), Chinnathai et al. (2023), Padella et al. (2024), Meneghello et al. (2024) |
| **P5** -- BPS integrated within predictive pipeline | 2 | Rieke et al. (2010), Weinzierl et al. (2020) |
| **P6** -- BPS applied to prediction outcomes | 2 | De Moor et al. (2025, ProCause), De Moor et al. (2025, SimBank) |
| **P7** -- Symmetric integration | 2 | Solomon et al. (2011), Pandey et al. (2012) |

### RQ3: What synergies emerge from integrating BPS and PPM?

| Synergy | Description | Count | Papers |
|---|---|---|---|
| **S1** | Simulation is used to generate synthetic data to train and validate predictive models | 5 | Pandey et al. (2012), Camargo et al. (2019), Chinnathai et al. (2023), Meneghello et al. (2024), De Moor et al. (2025, SimBank) |
| **S2** | PPM flags risky cases at runtime, and simulation runs micro-what-ifs for prescriptive support | 3 | Rieke et al. (2010), He et al. (2014), Weinzierl et al. (2020) |
| **S3** | PPM-based drift detection feeds back to update simulation parameters | 2 | Rashid et al. (2022), Vinci et al. (2025, online) |
| **S4** | PPM is used to determine parameters of the simulation model | 20 | Solomon et al. (2011), Bergmann et al. (2014), Tangkawarow et al. (2018), Elbattah et al. (2018), Chang et al. (2018), Fauzan et al. (2019), Mesabbah et al. (2020), Pourbafrani et al. (2022), Rashid et al. (2022), Camargo et al. (2023), de Leoni et al. (2023), Meneghello et al. (2023), El Kassimi et al. (2024), Lopez-Pintado et al. (2024), Oyamada et al. (2024), Kirchdorfer et al. (2025), Vinci et al. (2025, online), Vinci et al. (2025, reliable), Graziosi et al. (2025), Buliga et al. (2025) |
| **S5** | Simulation is used to assess the impact or usefulness of prediction or forecasting accuracy | 6 | He et al. (2014), Weinzierl et al. (2020), Ruschel et al. (2020), Padella et al. (2024), De Moor et al. (2025, ProCause), De Moor et al. (2025, SimBank) |
| **S6** | PPM is used to evaluate BPS models | 1 | Özdemir et al. (2026) |

**Co-occurrence of Synergies and Integration Patterns:**

| Synergy | P1 | P2 | P3 | P4 | P5 | P6 | P7 | Sum |
|---|---|---|---|---|---|---|---|---|
| S1 |  | 1 |  | 2 |  | 1 | 1 | **5** |
| S2 | 1 |  |  |  | 2 |  |  | **3** |
| S3 |  | 2 |  |  |  |  |  | **2** |
| S4 | 7 | 12 |  |  |  |  | 1 | **20** |
| S5 | 1 |  |  | 2 | 1 | 2 |  | **6** |
| S6 |  |  | 1 |  |  |  |  | **1** |

---

## Process Perspectives in Predictive Simulation Models

Predictive models are most often used to parameterize or refine simulation models, predicting the future behavior of running instances, and generating event data across different process perspectives. The table below provides an overview of the process perspectives for which predictive (generative) models are used to estimate simulation parameters.

| Paper | Control-flow | Temporal Dynamics | Resource Perspective | Data Attributes | Others |
|-------|---|---|---|---|---|
| de Leoni et al. (2023) | x |  |  |  |  |
| El Kassimi et al. (2024) | x |  |  |  |  |
| Camargo et al. (2023) |  | x |  |  |  |
| Meneghello et al. (2023) |  | x |  |  |  |
| Rashid et al. (2022) |  | x |  |  |  |
| Fauzan et al. (2019) |  | x |  |  |  |
| Tangkawarow et al. (2018) |  | x |  |  |  |
| Meneghello et al. (2024) |  |  | x |  |  |
| Lopez-Pintado et al. (2024) |  |  |  | x |  |
| Pourbafrani et al. (2022) |  |  |  |  | x |
| Elbattah et al. (2018) |  |  |  |  | x |
| Oyamada et al. (2024) | x | x |  |  |  |
| Vinci et al. (2025, online) | x | x |  |  |  |
| Ruschel et al. (2020) | x | x |  |  |  |
| Solomon et al. (2011) | x | x |  |  |  |
| Mesabbah et al. (2020) | x | x |  |  |  |
| Bergmann et al. (2014) | x |  | x |  |  |
| Kirchdorfer et al. (2025) |  | x | x |  |  |
| Graziosi et al. (2025) | x | x | x |  |  |
| Vinci et al. (2025, reliable) | x | x | x |  |  |
| Buliga et al. (2025) | x | x | x | x |  |
| **Number of Papers** | **11** | **14** | **6** | **2** | **2** |
