# Evaluating differences in overdose between medications
*Causal epidemiology considerations and solutions for studies evaluating impact of Rx drugs in preventing overdose*

We want to draw legitimate conclusions about what causes overdoses. We use data sources from electronic health records, insurance claims, vital statistics, and elsewhere to answer fundamental questions about the safety of new medications. But we know that these data sources are imperfect, and that not everything is documented in them with certainty.

*So how do we know whether what we are seeing is real?*

[Detailed study overview](https://www.opioiddata.org/studies/counfounding-opioid-safety-studies/) at OpioidData.org

## Scope of the Problem

The following methodological issues are being explored by our team. We will update results throughout the project in the table below.

|Issue|Description|Status & Resources|
|---|---|---|
| **Cohort effect**  | The median age of overdose deaths has increased by 10 years over the last decade. There may be a birth-cohort effect as has been observed with other drugs. This may influence age-adjustment in statistical models. | *Under consideration* <BR> [Initial findings](https://doi.org/10.1016/j.drugalcdep.2014.10.005)|
| **Chanelling**  | We are evaluating and comparing methods for confounding by “indication”: the expected likelihood that patients receiving ADF opioids have different risk profiles for experiencing overdose than patients prescribed traditional opioids.  | *Under consideration*  |
| **Early adopter prescribers**  | Uptake of new technology occurs first in "early adopters." We hypothesized that early prescribers of new medicines could likewise be identified, possibly influencing interpretation of early post-market assessments.  | **In Progress**<br>[Abstract](https://opioiddatalab.github.io/PharmacistPrescriberSurveys/earlyAdopters/ICPEabstractEarlyPrescribers_submitted.html)  |
| **Death vs. disenrollment**  | Research using insurance claims data allow for a comprehensive nationwide assessment of opioid prescribing patterns and downstream effects. However without linkage to death data, disenrollment from the database is treated as a censoring event, as patients are lost to follow-up. Our preliminary analyses show that 27.6% of individuals who “disenroll” from the Medicare Supplemental plan have a death date within 30 days of disenrollment.  | **In progress**<br>[Study details](https://www.opioiddata.org/studies/predicting-out-of-hospital-death/)<br>[Preliminary analysis](https://opioiddatalab.github.io/overdose/YoungJC_ICPE_poster2019_OOH_deaths.pdf)  |
| **Last dose causality**  | In a recent analysis where the drugs involved in overdose death were not known, scientists assumed that the last dispensed opioid was the one involved in death. | *Planning* <br> [FDA analysis, page 572](https://www.fda.gov/media/141914/download)|
| **Comparator choice**  | What is the best comparator for an ADF? Is it other medicines with the same active ingredient? Or, would it be better to consider a patient pool of similar patients as the comparator?  | *Under consideration*  |
| **Heroin**  | Over the last decade, heroin-fentanyl overdose deaths increased as Rx overdose deaths decreased. COVID caused further changes. | *Under consideration*  |
| **Utilization adjustment**  | There are hidden assumptions of linearity between the amount dispensed and negative outcomes. However, for low volume products this assumption may not hold. | *Under consideration*<br> [Preliminary analysis](https://doi.org/10.1002/pds.4736)|
| **Stockpiling**  | Leftover opioid analgesic tablets from previous dispensings are ignored in exposure time calculations, excluding what could have been additional “at risk” exposure time. At the same time, “stockpiled” leftover drug and frequent changes in opioid analgesic regimens create challenges in accurately allocating exposure time, and thus correctly attributing overdose outcomes to a particular dispensed opioid analgesic.  | *Under consideration*<br>[Possible analytic approach](https://doi.org/10.1002/pds.5026)  |
| **Dose/MME**  | In support of safer opioid prescribing, 90 daily milligrams of morphine equivalents (MME) are considered a putative risk threshold in clinical guidelines and state laws. But, previously hidden calculation variations may inadvertently have unintended consequences. In order to assess this underappreciated concern, we identified variations in daily MME definitions from published literature and digital clinical tools.  | **In progress**<br> + [Justification](https://github.com/opioiddatalab/MMEequations/blob/master/docs/MME_initial_explorations.ipynb) + [Meta analysis](https://github.com/opioiddatalab/MMEequations/blob/master/MME_meta_analysis.ipynb)  |
| **Switching between opioids**  | Nearly all ADF-recipients also received non-ADFs. Can cross-over design-thinking be used to extricate the effect of the ADF? Or do we need to consider ADF use in the context of other prescribed medicines?  | *Under consideration*  |
| **Patient characteristics**  | How best to adjust for patient-level characteristics, like age, sex, and co-morbidities?  | *Under consideration*  |
| **Time-varying confounding**  | Since an individual’s risk for misuse of opioids likely changes over time, advanced statistical models may help quantify the importance of time-dependent adjustment.  | **In progress**<br>[Study details](https://www.opioiddata.org/studies/counfounding-opioid-safety-studies/)<br>[DAG](https://github.com/opioiddatalab/DAG/tree/master/docs)  |
 | **Days supply** |In most states, pharmacists calculate by hand the “days’ supply”. There is discretion at the pharmacist level and we would like to find out how consistent and accurate interpretations of doctors’ instructions are.  | *On COVID hold*<br>[Study details](https://www.opioiddata.org/studies/days-supply-validation/)|

