---
title: Double Trap
---

# {{ page.title }}

## Ion trap with tunable ion height

We designed and implemented a novel surface-electrode Paul trap that produces an RF-null along
the axis perpendicular to the trap surface. This architecture enables control of the ion height,
between 50 &mu;m and 300 &mu;m above the surface, using only DC electrodes, creating a platform for
precision electric-field noise detection, trapping of vertical ion strings without excess micromotion,
and potential applications for scalable quantum computers with surface ion traps.

<figure>
	<img src="/research/quantum-electronics/SingleTrap.jpeg" alt="Trap layout and potentials" height="200" />
	<figcaption>
		Fig. 1. (a) False-color microscope image of the microfabricated four-rf-electrode trap.
		Static voltages are applied to electrodes labeled dc, and rf electrodes are labeled rf+-
		according to the signal phase. (b) Top-down view of xy-plane rf pseudopotentials at a
		height of z = 175 &mu;m, with electrode geometry shown for reference.
		(c) Side view of rf potentials.
	</figcaption>
</figure>

<figure>
	<img src="/research/quantum-electronics/potential_lines.gif" alt="Potential during ion shuttling" height="350" />
	<figcaption>
		Fig. 2. Simulated shuttling of the ion perpendicular to the trap surface.
	</figcaption>
</figure>

## Electric-field noise vs. ion height

With the capability of shuttling the ion up and down, we can perform measurements of the
electric-field noise (see [SQIP](/research/quantum-computing/)).
We find the distance dependence of the noise to scale as d<sup>-2.6</sup> in our trap and a frequency dependence
which is consistent with 1/f noise. With significant evidence that we are not limited by technical
noise sources, our distance scaling data is consistent with a noise correlation length of about 100
&mu;m at the trap surface.

<figure>
	<img src="/research/quantum-electronics/DistanceScaling.png" alt="Heating rate vs. distance" height="300" />
	<figcaption>
		Fig. 3. Planar (blue) and normal (red) heating rates as a function of ion-surface distance for a
		fixed secular frequency of 1 MHz. Power-law fits are overlayed for reference.
	</figcaption>
</figure>

## Quantum information transfer through a classical conductor

An oscillating trapped ion induces oscillating image charges in the trap electrodes. If this current
is sent to the electrodes of a second trap, it influences the motion of an ion in the second trap.
The expected time for a complete exchange of the ion motions is 1 ms for a trap with a characteristic
size of 50 &mu;m. This inter-trap coupling may be used for scalable quantum computing, cooling ion
species that are not directly accessible to laser cooling, non-invasive study of superconductors,
and realization of hybrid systems by coupling an ion-trap quantum computer to a solid-state quantum computer,
e.g. a system of Josephson junctions.

<figure>
	<img src="/research/quantum-electronics/DoubleTrap.png" alt="Double trap" height="300" />
	<figcaption>
		Fig. 4. Schematic of coupling trap. The two trapping regions are located above the centers of the red squares,
		which are connected via an electrically floating wire. Out-of-phase RF is applied to the green electrodes,
		and DC is applied to the blue electrodes.
	</figcaption>
</figure>

This project is supported by AFOSR project "Prototype solid state quantum interface for trapped ions".
