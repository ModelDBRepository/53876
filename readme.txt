Readme for a model from the Quadroni and Knopfel 1994 paper:

Quadroni R, Knopfel T.
Compartmental models of type A and type B guinea pig medial vestibular neurons.
J Neurophysiol. 1994 Oct;72(4):1911-24.

    Institut fur Theoretische Physik, ETH-Honggerberg, Zurich, Switzerland.

Abstract:

1. We have developed compartmental models of guinea-pig medial
vestibular nuclei neurons (MVNns). The structure and the parameters of
the model cells were chosen to reproduce the responses of type A and
type B MVNns as described in electrophysiological recordings.
2. Dynamics of membrane potentials were modeled in 46 and 61 branched
electrical compartments for Type A and Type B MVNns,
respectively. Each compartment was allowed to contain up to nine
active ionic conductances: a fast inactivating sodium conductance,
gNa, a persistent sodium conductance, gNap, a low-voltage activated
calcium conductance, gCa(LVA), a high-voltage activated calcium
conductance, gCa(HVA), a fast-voltage activated potassium conductance,
gK(fast), a slowly relaxing voltage activated potassium conductance,
gK(slow), a fast transient potassium channel, gK(A), a slowly relaxing
mixed sodium-potassium conductance activating at hyperpolarized
membrane potentials, gH, and a calcium-activated potassium conductance
gK(AHP).  The kinetics of these conductances were derived from
voltage-clamp studies in a variety of preparations. Kinetic parameters
as well as distribution and density of ion channels were adjusted to
yield the reported electrophysiological behavior of medial vestibular
neurons.
3. Dynamics of intracellular free [Ca2]i were modeled by inclusion of
a Ca(2+)-pump and a Na(+)-Ca2+ exchanger for extrusion of
calcium. Diffusion of calcium between submembraneous sites and the
center of an electrical compartment was modeled by 25 and 6 shell-like
chemical compartments for the cell body and the proximal dendrites,
respectively. These compartments also contained binding sites for
calcium.
4. The dynamics of active conductances were the same in both models
except for gK(fast). This was necessary to achieve the different shape
of spikes and of spike afterhyperpolarization in type A and type B
MVNns. An intermediate depolarizing component of the spike
afterhyperpolarization of type B neurons in part depended on their
dendritic cable structure.
5. Variation of the low threshold calcium conductance, gCa(LVA), shows
that the ability to generate low-threshold spike bursts critically
depends on the density of this conductance. Sodium plateaus were
generated when increasing the density of gNap.
6. The type B model cell generated rhythmic bursts of spiking activity
under simulation of two distinct experimental conditions.(ABSTRACT
TRUNCATED AT 400 WORDS)

-----------------------------------------
How to run the model:

Autolaunch from ModelDB and select figures by pressing a button or
download and expand the archive.  Then on

mswin: double click on the mosinit.hoc file after compiling the mod
     files with mknrndll

unix: type "nrnivmodl" and enter and then "nrngui mosinit.hoc" in the
     expanded archive folder.

mac: after the archive is unziped drag and drop the newly created mvns
     folder onto the mknrndll icon. Then drag and drop the mosinit.hoc
     in the mvns folder onto the nrngui icon.

-----------------------------------------

Note that the jpg file in this collection that shows the steady state
version of figure 3.  This figure differs slightly from the demo
because the demo doesn't reach a steady state before the currents are
displayed.  To get the same currents merely increase the simulation
length (tstop) to greater than 1000 ms and press init and run button.

Note that in the ca_X.mod files the K_ are converted into K2f_'s from
the paper by multiplying 2*FARADAY them (twice for the charge on Ca).
This effectively turns the formula's for the j_X fluxes (particles
passing boundaries) into formula's for i_X currents (coulombs per
second).

For questions about the paper please contact Thomas Knopfel, for
questions about the model code, Tom Morse.

20070912 Updated with extra dummy current in ca_*.mod files to
synchronize calculation of conductances with the currents.  Thanks to
Stephen Larson for the bug report and Michael Hines for the fix.
