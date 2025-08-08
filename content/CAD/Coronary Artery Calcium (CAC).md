---
tags:
  - CAD
  - imaging
aliases:
  - Agatson
---
- Uses **non-contrast CT** with a fixed threshold of 130 Hounsfield units (HUs) for calcium detection
- With modern scanners and protocols, the radiation dose required for acquisition of a CT calcium score is approximately 1 mSV.
- Weighting
	- A weight of 1 is given for attenuation of 130 to 199
	- 2 for 200 to 299
	- 3 for 300 to 399
	- 4 for attenuation ≥400
	- The weighting factor is multiplied by the area of each lesion, with the sum of values for all lesions used to determine the total Agatston score

> [!warning] If patient with [[Familial Hyperlipidemia]], don't even bother with CAC
> 

# CAC Scan Acquisition

- Slice thickness: 3mm
- Prospectively triggered scan
- Target exposure depends on heart rate (40-75%)
	- Diastasis is at ~75% of R-R interval (used when HR is nice and slow)
	- Isovolumic relaxation is at ~40% of R-R interval (used when HR is high)
		- The 🫀 can't move (at least on the Left) because the [[Aortic Valve|AV]] and [[Mitral Valve|MV]] are closed during IVR
- Tube potential is fixed at 120 kV, tube current variable
- Non-contrast study

# Advantages of obtaining a CAC scan prior to [[Coronary Computed Tomography Angiography (CCTA)|CCTA]]

- Minimizes Scan range
- Provides estimate of plaque burden - useful for prognosis
- ~~Establishes pre-test probability for obstructive CAD~~ (not actually true)
- CAC >600 should make you pause as it can ↓ [[Sensitivity|sensitivity]] and [[Specificity|specificity]] in looking for obstructive CAD
	- 🤔 Is this still the case in the era of photon-counting CT, I wonder
- 📄 Arbab-Zadeh A, Miller JM, Rochitte CE, Dewey M, Niinuma H, Gottlieb I, Paul N, Clouse ME, Shapiro EP, Hoe J, Lardo AC, Bush DE, de Roos A, Cox C, Brinker J, Lima JA. Diagnostic accuracy of computed tomography coronary angiography according to pre-test probability of coronary artery disease and severity of coronary arterial calcification. The CORE-64 (Coronary Artery Evaluation Using 64-Row Multidetector Computed Tomography Angiography) International Multicenter Study. J Am Coll Cardiol. 2012 Jan 24;59(4):379-87. doi: 10.1016/j.jacc.2011.06.079. PMID: 22261160; PMCID: PMC3348589.
# Percentile Scoring

- [cac-tools.com](https://www.cac-tools.com/) can be used for patients 30-45 years old
- [MESA 10-Year CHD Risk with Coronary Artery Calcification](https://internal.mesa-nhlbi.org/about/procedures/tools/mesa-score-risk-calculator) works for 45-85 years of age

## Coronary Age Calculation

- TODO
# LDL Goals

| CAC Score                  | Recommendation                    | LDL Goal                                                         |
| -------------------------- | --------------------------------- | ---------------------------------------------------------------- |
| 0                          | Consider *no* statin              | -                                                                |
| 1-99                       | Favors statin (esp if age >55 yo) | <100                                                             |
| 100+ (or ≥75th percentile) | Statin                            | <70 (add [[Ezetimibe]] if needed)                                |
| 1000+                      | Statin                            | <70 (add [[Ezetimibe]] + [[PCSK9 Inhibitors\|PCSK9i]] if needed) |

![[Coronary Artery Calcium _CAC_-1744895073637.webp|531x908]]
Figure source: [^acc22]

National Lipid Association CAC-based management [^nla]
![[Coronary Artery Calcium _CAC_-1744895219335.webp]]
# Power of Zero (CAC of 0)

- If CAC 0, no need for statin *unless* [[Diabetes]], smoker
- What does a zero coronary artery calcium score tell us?
	- <u>Intermediate Risk</u> w/ dyspnea or classic angina
		- 16% incidence inducible ischemia on [[Positron Emission Tomography (PET)|PET]]
	- <u>High Risk</u> Symptomatic Patients in ED w/ ACS
		- 70% prevalence of obstructive [[Coronary Artery Disease (CAD)|CAD]] by [[Coronary Computed Tomography Angiography (CCTA)|CCTA]]
- 🌟 Negative CAC is helpful in **Low** and **Intermediate** Risk population (but not high-risk populations)

## Warranty of CAC = 0?

- Blaha recommends 3-5 years [^dzaye20]
	- ![[Coronary Artery Calcium _CAC_-1744894912396.webp]]


[^dzaye20]: Dzaye O, Dardari ZA, Cainzos-Achirica M, et al. Warranty Period of a Calcium Score of Zero. JACC: Cardiovascular Imaging. 2021;14(5):990-1002. doi:10.1016/j.jcmg.2020.06.048
[^acc22]: Lloyd-Jones DM, Morris PB, Ballantyne CM, et al. 2022 ACC Expert Consensus Decision Pathway on the Role of Nonstatin Therapies for LDL-Cholesterol Lowering in the Management of Atherosclerotic Cardiovascular Disease Risk. Journal of the American College of Cardiology. 2022;80(14):1366-1418. doi:10.1016/j.jacc.2022.07.006
[^nla]: Orringer, Carl E., et al. "The National Lipid Association scientific statement on coronary artery calcium scoring to guide preventive strategies for ASCVD risk reduction." _Journal of clinical lipidology_ 15.1 (2021): 33-60.

