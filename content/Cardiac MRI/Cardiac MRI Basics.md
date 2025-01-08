---
tags:
  - cMRI
---

- Cardiac MRI are usually done on 1.5 Tesla (30,000 times the Earth's magnetic field)
- ⚠️ Safety issue: the magnet 🧲  is always on
- In the presence of a strong magnetic field (typically 0.5 – 3.0 Tesla (T) for clinical applications) atoms ⚛︎ in the body (typically hydrogen) are stimulated to emit radio waves 🔊. These radio waves 🔊 are detected by an antenna  (more specifically, the **radiofrequency coils**) placed around, or over, the body part of interest allowing an image of the body to be reconstructed.
	- Extra magnetic fields (using **gradient coils**) are used to constantly change the magnetic field to allow images of the body to be reconstructed.
- The *typical* magnetic field strengths used in clinical MRI scanners are:
	- 1.5 Tesla
	- 3 Tesla
- **Excitation**: The RF pulse (radiowave) causes a proton to be excited → flips from low- to high-energy state
- **Relaxation**
	- **T1 Recovery**
		- the natural tendency is to from high-energy state back to a low-energy state
		- there is a predictable rate of regrowth/relaxation. 
		- In the figure below, you are going from the high-energy state in the transverse plane ($M_{xy}$) where the flip angle is 90˚ (100% transverse magnetization and 0% longitudinal magnetization) and there is "regrowth" towards the low-energy state where the flip angle is 0˚ in the longitudinal axis ($M_z$) and the protons are aligned upright in the direction of the *main* magnetic field.
		- When this rate of regrowth is mapped over time, the **T1 time constant** is the amount of time it takes to regain **63%** of the intrinsic (full) magnetization ($M_0$)
		- ![[Cardiac MRI Basics-20250108102331506.webp|489]]
		- 📝 T1 time is <u>tissue-specific</u>, i.e. different tissues have different T1 times
			- Fat has short T1 times, i.e. hydrogen protons that are within fat will have very fast T1 recovery
				- ~200-250 ms
			- Water has very *slow* T1 recovery times
				- ~2,000 ms (10-fold greater T1 relaxation time compared to fat❗)
			- ![[Cardiac MRI Basics-20250108103655546.webp]]
				- [Figure source](https://radiologykey.com/principles-of-magnetic-resonance-imaging-physics/)
	- **T2 Decay** (aka spin-spin relaxation)
		- When the RF excitation pulse is applied, the protons are all spinning in-phase. Immediately after this pulse is applied, they begin to **dephase** at a rate proportional to the amount of the magnetic field. → eventually, protons will return to their out-of-phase initial pre-RF excitation state, as measured by the **T2 relaxation time**. ([Source](https://radiologykey.com/principles-of-magnetic-resonance-imaging-physics/))
		- The rate of **dephasing** is different for each tissue, resulting in further tissue contrast.
		- ![[Cardiac MRI Basics-20250108104223135.webp]]
			- 📝 this "dephasing" is occurring in the $xy$-plane
		- T2 decay time is the amount of time it takes to drop your magnetization to **37%** of what it was after you first applied a 90˚ RF pulse
		- ![[Cardiac MRI Basics-20250108104012826.webp]]
- The **Larmor equation** is a mathematical formula that describes the **precession frequency** of nuclei in a substance placed in a static magnetic field
	- $\omega = \gamma \cdot B$
	- used to calculate the frequency of an RF signal that causes a change in the nucleus spin energy level. 
	- $\gamma$: the gyromagnetic ratio is different for each nucleus of different atoms. 
	- $B$: the stronger the magnetic field ($B$), the higher the precessional frequency ($\omega$).
	- At 1.5T, the protons are spinning around 64 MHz
	- At 3T, protons are spinning around at 128 MHz
	- ![[Cardiac MRI Basics-20250108101631669.webp|513]]


> [!NOTE] Earth's 🌎 magnetic field 🧲
> The Earth's magnetic field, which is typically around 25-65 microtesla (µT). Therefore, 1 Tesla is about 30,000 times the earth's magnetic field.


# MRI Machine

![[Cardiac MRI Basics-20250108094646703.webp|501]]

- Layers of the MRI scanner coils (listed from outer-to-inner)
	- **Main magnet coils** ($B_0$)
		- defines the strength of the *constant* magnetic field ($B_0$), which is typically measured in Tesla units.
	- **Gradient coils** ($G$)
		- Series of coils within main magnet
			- 3 sets: $x$, $y$, and $z$ directions
				- The $z$-axis is parallel to $B_0$
			- ![[Cardiac MRI Basics-20250108095958658.webp|415]]
		- Make slight alterations to the local magnetic field in a graded fashion
		- Units are measured in milliTesla/meter (mT/m)
		- Can be turned on/off
		- Allow for spatial localization given the coordinate axis reference system afforded by the $x$, $y$, and $z$ axes. ∴, allows you to register all of your images b/c you are in a *fixed* coordinate system.
		- Safety issues:
			- Loud noise
				- make the familiar banging sounds of an MRI scan
			- Peripheral nerve stimulation - temporary
	- **Radiofrequency coils** ($B_1$)
		- Innermost layer of coils
		- There are 2 sets of RF coils: 
			- *transmitter* coils
				- <u>send</u> in a RF pulse → excitation of protons
				- *generally* located within the MRI scanner itself
			- *receiver* coils
				- <u>receive</u> radiowaves → signal is processed to generate your image
				- typically flexible coils places around the patient; best quality if they are as close as possible to the area you're trying to image
			- ![[Cardiac MRI Basics-20250108100739017.webp|384]]
		- Turn on/off
		- Help generate MRI image
		- Safety issues:
			- Burns
			- Device malfunction

# Terminology

| Term                                           | Meaning                                                                                                                                                                                                                                                                                                                                                                          |
| ---------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| T1 [ms]                                        | Time constant representing the recovery of *longitudinal* magnetization (spin-lattice relaxation)                                                                                                                                                                                                                                                                                |
| Native T1                                      | T1 in the absence of an exogenous contrast agent                                                                                                                                                                                                                                                                                                                                 |
| T2 [ms]                                        | Time constant representing the decay of *transverse* magnetization (spin-spin relaxation)                                                                                                                                                                                                                                                                                        |
| T2* [ms]                                       | Time constant representing the decay of *transverse* magnetization in the presence of local field inhomogeneities                                                                                                                                                                                                                                                                |
| ECV [%]                                        | Extracellular volume fraction, calculated by  <br>$ECV = \frac{\frac{1}{T1_{\text{myo}_\text{post-Gad}}} - \frac{1}{T1_{\text{myo}_\text{native}}}}{\frac{1}{T1_{\text{blood}_\text{post-Gad}}} - \frac{1}{T1_{\text{blood}_\text{native}}}} \times (100 - \text{Hct})$<br>where myo = myocardium; blood = intracavitary blood pool; Hct = cellular volume fraction of blood [%] |
| Synthetic ECV [%]                              | ECV where hematocrit is not measured by laboratory blood sampling but derived from blood T1                                                                                                                                                                                                                                                                                      |
| [[MRI Mapping Techniques\|Parametric mapping]] | A process where a secondary image is generated in which each pixel represents a specific magnetic tissue property (T1, T2, or T2*) or a derivative such as ECV) derived from the spatially corresponding voxel of a set of co-registered magnetic resonance source images                                                                                                        |
