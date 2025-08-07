# How transparent is graphene? A surface science perspective on remote epitaxy

Zachary LaDuca, $^{1}$  Anshu Sirohi, $^{1}$  Quinn Campbell, $^{2}$  and Jason K. Kawasaki $^{1}$ ,  $^{*}$ $^{1}$ Materials Science and Engineering, University of Wisconsin- Madison, Madison, WI 53706, United States of America $^{2}$ Sandia National Laboratories, Albuquerque, NM 87123, United States of America(Dated: July 31, 2025)

Remote epitaxy is the synthesis of a single crystalline film on a graphene- covered substrate, where the film adopts epitaxial registry to the substrate as if the graphene is transparent. Despite many exciting applications for flexible electronics, strain engineering, and heterogeneous integration, an understanding of the fundamental synthesis mechanisms remains elusive. Here we offer a perspective on the synthesis mechanisms, focusing on the foundational assumption of graphene transparency. We highlight challenges for quantifying the strength of the remote substrate potential that permeates through graphene, and propose Fourier and beating analysis as a bias- free method for decomposing the lattice potential contributions from the substrate, from graphene, and from surface reconstructions, each at different frequencies. We highlight the importance of graphene- induced reconstructions on epitaxial templating, drawing comparison to moire epitaxy. Finally, we highlight the role of the remote potential in tuning surface diffusion and adatom kinetics on graphene. Tuning the surface diffusion length is crucial in navigating the competition between remote epitaxy and defect- seeded mechanisms like pinhole epitaxy.

# I. INTRODUCTION

Remote epitaxy [1] is a transformative approach for synthesizing single crystalline membranes and lattice mismatched heterostructures, for application in flexible electronics [2], discovery of new properties via strain engineering [3- 7], lattice mismatched heteroepitaxy with reduced dislocation densities [8- 10], and integration of dissimilar materials [11]. In this approach, thin films are grown on a graphene- covered single crystalline substrate. Under the right conditions, a single crystalline film can be produced which has epitaxial registry to the substrate rather than to graphene. Several reviews have focused on applications [12- 14], the processing steps required for making, transferring, and performing epitaxy on top of graphene- covered surfaces [14- 16], and comparison with different types of epitaxial growth modes [17, 18].

However, the synthesis mechanisms of remote epitaxy remain elusive. The foundational assumption of remote epitaxy is that graphene is transparent and weakly interacting. That is, graphene allows the lattice potential of the substrate to pass through while contributing a relatively weak lattice potential of its own, and the graphene does not distort the underlying substrate atomic positions or vice versa. This degree of transparency is difficult to quantify due to challenges in preparing clean graphene/substrate interfaces [19- 23]. The strength of the remote potential is typically inferred via post film growth observables like epitaxial alignment of the substrate or ability to exfoliate a membrane [1, 24] or its apparent wetting transparency [25, 26], but has not been directly measured [27- 29]. Additionally, there are many examples where graphene induces strong distortions in an underlying substrate. One example is "buffer" graphene that forms on Si- terminated SiC (0001) [30]. This buffer graphene is highly buckled due to partial covalent bonding to the SiC substrate, which results in dangling bonds out- of- plane and a long- range reconstruction in- plane with  $(6\sqrt{3}\times 6\sqrt{3})R30^{\circ}$  periodicity. Buffer graphene also has a semiconducting gap [31], suggesting less free carrier screening of the remote potential through buffer graphene than through pristine semimetallic graphene. These factors suggest that graphene- induced surface reconstructions are important to the mechanisms of remote epitaxy, beyond the simplest limit of graphene transparency.

Here we highlight some of the outstanding questions regarding graphene transparency, and their impacts on thermodynamics and kinetics of remote epitaxy:

Section II: How strong is the remote lattice potential? What is the nature of the remote bonding interaction and what kind of potential is the correct descriptor? How can we analyze complicated potentials that convolve the substrate lattice with the graphene lattice?

Section III: How does graphene interact with an underlying substrate? What are the impacts of changes in graphene bonding, local atomic registry between graphene and substrate, and surface reconstructions, on epitaxial growth on these surfaces?

Section IV: How does the remote potential modify adatom kinetics on graphene? How does kinetics control remote epitaxy versus defect- seeded mechanisms?

# II. HOW STRONG IS THE REMOTE LATTICE POTENTIAL?

We first address the strength of the remote lattice potential permeation of the substrate. For simplicity we ignore reconstructions here, and revisit the reconstruc

![](https://cdn-mineru.openxlab.org.cn/result/2025-08-07/d6c606d7-b5fc-4ba1-8c91-63b6ed66274b/d53adfe16efd9f669e1ec5489030ff307e0f18fe3a22378e4e1f0a616d31ec35.jpg)  
FIG. 1. Challenges for interpreting electrostatic potential maps of graphene/substrate heterostructures. (a,b) Crystal structures of graphene/Si (001) and graphene/GaN (0001), with fixed in-plane positions and allowed out-of-plane relaxation. (c,d) Electrostatic potential maps. The potential fluctuations of the graphene itself have been subtracted away. Atom position labels 1, 2, 3 and crystallographic axes are added for clarity. Note that (d) is sheared from the hexagonal symmetry of GaN (0001). (e,f) Line cuts of the electrostatic potentials. (g) Summary of extracted  $\Delta \phi$  for different graphene covered substrates. (h) Periodic profiles of the selected regions from (e) and (f). For graphene/Si it is the region  $x = 0$  to  $x = 0.5$  in (e). For graphene/GaN it is the region  $x \approx 0.8$  to  $x \approx 0.1$  (atom 3 to atom 1) in (d). Adapted from Kong et. al., "Polarity governs atomic interaction through two-dimensional materials," Nature Materials 17, 999-1004 (2018) Springer Nature [24]. Reproduced with permission from Springer Nature.

tions in Section III. Quantifying this potential is challenging since the nature of the film- graphene- substrate interaction remains unclear. In conventional epitaxy and van der Waals (vdW) epitaxy, where the characteristic spacing between film and substrate is  $2 - 3 \mathrm{\AA}$ , the primary interactions are covalent bonding and vdW interactions (fluctuating dipoles) between atoms. But for remote epitaxy, where film and substrate are separated by  $\sim 6 \mathrm{\AA}$  due to insertion of graphene, the nature of this interaction is unclear. One might expect it is some combination of covalent and vdW bonding interaction plus longer range electrostatics (if the adatoms are ionized, e.g. by charge transfer to or from graphene, as often occurs for alkali metals in graphite intercalation compounds [32]). Note, however, that electrostatics are less relevant for neutral adatoms. Another possibility is an extended molecular orbital that includes states from the substrate that hybridize with graphene [33].

To date, the field has relied on several proxies for the remote lattice potential. In the pioneering work on remote epitaxy, Kim et. al. [1] computed the charge density as a function of distance for GaAs slabs that are separated by a vacuum gap, using density functional theory (DFT). They found that for slabs separated by up to 9  $\mathrm{\AA}$ , there is a finite charge density in the middle of the vacuum gap. This calculation provided the first theoretical suggestion that the lattice potential of the substrate may extend significantly beyond the  $2 - 3 \mathrm{\AA}$  typical equilibrium spacing between atoms. It should be noted, however, that within the DFT surface science community, the emergence of charge within the vacuum region is considered a sign that the vacuum region is not large enough to create a truly "isolated" surface. While the calculations in question are trying to demonstrate that interaction between a substrate and film can take place across larger vacuum distances, this ignores the periodic nature of the structure. I.e., the DFT calculation represents an infinite GaAs material with repeating vacuum

regions in the middle. It is not clear from these calculations that this charge density interaction through the vacuum would persist if the film and substrate were truly isolated. Furthermore, the periodic nature of these calculations implies both the film and substrate are of the same size, which at best describes a minority of homoepitaxial cases. The finite slab size would need to be tested for convergence to ensure that both ends of the slab could behave independently to truly mimic a substrate and film with the ability to differ.

More importantly, many calculations of the remote potential (and its proxies) do not include free carrier screening from graphene, which is expected to be significant since graphene is a semimetal. As an order of magnitude estimate, the Thomas- Fermi screening length for a free electron gas with density  $n_{3D} = 10^{20} \mathrm{cm}^{- 3}$  is  $\lambda_{TF} = 1.7$ $\mathrm{\AA}$ . Assuming an effective graphene thickness of  $\Delta z = 3 \mathrm{\AA}$ , this suggests that the field transmission through monolayer graphene is  $exp(- \Delta z / \lambda_{TF}) = 17\%$  and the transmission through bilayer graphene is  $exp(- 2\Delta z / \lambda_{TF}) = 3\%$  [34]. Any estimate of the remote potential permeation through graphene would need to include screening.

The current standard is to use the electrostatic potential as a proxy for the remote interaction potential (Fig. 1). Generally the electrostatic potential is computed using DFT slabs. Some calculations include the graphene and then subtract it away during post processing [24, 35], while others ignore graphene entirely [9]. A common simplification is to ignore lateral reconstructions and fix the atoms to the bulk- like  $(x,y)$  positions, since reconstructions would require much larger supercells. These calculations often allow for out- of- plane  $z$  relaxations.

The electrostatic potential analysis was first introduced by Kong et. al. [24], who concluded that the magnitude of lateral electrostatic potential fluctuations scales directly with the degree of bond polarity in the underlying substrate (Fig. 1(g)). Note that in these electrostatic potential maps (Fig. 1(c,d)), the lattice potential of graphene has already been subtracted away [24], making it difficult to compare the relative magnitude of the remote potential strength versus the graphene potential strength. This is important because, as we will discuss later, if the remote substrate potential and graphene potential are of similar magnitude, then epitaxy to graphene can compete with remote epitaxy to the substrate. The bond polarity prediction was supported by experiments showing that for substrates with more polar bonding, single crystalline epitaxy was observed on a greater number of graphene layers. This provided a major guidance for the field: bond polarity controls remote epitaxy.

There are two major challenges for interpreting how the electrostatic potential guides epitaxy. First, although electrostatic (Coulomb) interactions describe the electronic workfunction and band alignments, it is less clear that electrostatics would control the pairwise attractive and repulsive interactions between atoms. The use of this potential assumes that the film adatoms are ionized. It is an open question these species are indeed ionized (and to what degree?), or whether other types of interactions, e.g. van der Waals interactions or covalent hybridization, may be more relevant to epitaxy and bonding. Kong et. al. introduced an empirical scale factor  $\gamma$  that describes the assumed degree of ionization. Then the modified electrostatic potential fluctuation is

$$
\Delta \phi = \gamma (\phi_{max} - \phi_{min}). \tag{1}
$$

The challenge with this scale factor is that the particular values of  $\gamma$  are not constrained by measurement or theory. Ref. [24] used values of  $\gamma = 1$  for Si, GaAs, and GaN, and a value of  $\gamma = 2$  for LiF. However, because the electronegativity and ionization energies vary signification for Si, GaAs, and GaN, it is unclear that  $\gamma$  should equal 1 for the adatoms in all three materials. Further experiments and theory are required to constrain  $\gamma$  and enable comparisons of  $\Delta \phi$  across different materials, with potentially different bonding character.

A second challenge is that the raw potential maps contain more than one periodicity: the substrate lattice, the graphene lattice, and a longer- range supercell periodicity from relaxation, such that

$$
\phi_{total} = \phi_{sub} + \phi_{gr} + \phi_{supercell}. \tag{2}
$$

To distinguish  $\phi_{sub}$  of the remote substrate, Ref. [24] used the following subtraction and cropping procedure: First, they subtract the short period potential for isolated graphene  $(\phi_{gr})$ , resulting in the maps of Fig. 1(c,d). Next they crop the longer range fluctuation of the relaxed supercell  $(\phi_{supercell})$ : for the profile above graphene/GaN (0001) (Fig. 1(d,f)), they focus on the line cut from atom 3 to atom 1, crop away the rest of the supercell, then subtract a linear background. The energy difference along the path from atom 3 to atom 1 is then used as  $\phi_{sub}$  for the substrate, and this selected profile is periodically repeated in the line cut shown in Fig. 1(h).

The challenge with the background and cropping procedure is that it is difficult to determine which region of the line cut is most representative of  $\phi_{sub}$ . Could it instead be defined as the region from atom 1 to atom 2, which has similar magnitude but opposite sign? Or could it be defined by the flat region from atom 2 to atom 3? Or should one consider the entire length of the supercell? The choice of region changes the answer from  $\Delta \phi_{sub} \approx 40$  meV (atom 3 to 1 or atom 1 to 2), to 80 meV (full range), to just a few meV (atom 2 to 3). Moreover, the immediate subtraction of  $\phi_{gr}$  makes it difficult to assess the relative magnitude of the remote potential fluctuation from the graphene potential fluctuation. For remote epitaxy to dominate, presumably  $\Delta \phi_{sub}$  would need to be much larger than  $\Delta \phi_{gr}$ .

Calculations by Dai et. al. [5] suggest that the graphene and remote substrate potentials have similar magnitude, resulting in complicated interference patterns (Fig. 2). The electrostatic potentials above the bare Ge (001) and (110) surfaces match the lattice periodicity of Ge in those orientations (Fig. 2(a,b)). The potential

![](https://cdn-mineru.openxlab.org.cn/result/2025-08-07/d6c606d7-b5fc-4ba1-8c91-63b6ed66274b/abb4668a83ca532f15c813f8def47ce2a1baea6927b4deb4ea26c8826fb9476d.jpg)  
FIG. 2. Electrostatic potential calculations highlighting the interference from the graphene and substrate potentials. Lattice vectors are added for clarity. Adapted from Dai et. al. "Highly heterogeneous epitaxy of hexoelectric BaTiO $_{3 - \delta}$  membrane on Ge," Nature Commun., 13, 2990 (2022), Springer Nature [5], under Creative Commons CC BY license.

maps above graphene/Ge (001) and graphene/Ge (110) reveal more complicated patterns where the underlying periodicity square lattice periodicity of Ge (001) and rectangular lattice of Ge (110) are still observed, but convolved with the hexagonal graphene lattice (Fig. 2(c,d)). These interference patterns suggest that the electrostatic potential fluctuations from Ge and graphene have similar magnitudes.

A recent analytical model by Kawasaki and Campbell further suggests that once free carrier screening from graphene is included, the remote substrate potential and the graphene potential have similar magnitude [34] (Fig. 3), and thus interference with graphene cannot be ignored. This model starts from a Morse pair interaction potential (rather than electrostatics), which includes covalent and van der Waals interactions between film and substrate, plus a van der Waals spacer layer modeled by a Lennard- Jones potential. The inclusion of free carrier screening for typical graphene carrier densities significantly attenuates the remote potential, such that for a typical graphene densities of order  $10^{12} \mathrm{~cm}^{- 2}$ , the screened potential is of order  $10 \mathrm{meV}$ , similar to graphene. The advantages of this approach are that the

![](https://cdn-mineru.openxlab.org.cn/result/2025-08-07/d6c606d7-b5fc-4ba1-8c91-63b6ed66274b/0b08128acb18be50457af2b7e6bfa5e15e6bea94731923c8de131c004e9aac7d.jpg)  
FIG. 3. Screened Morse model for the remote potential above graphene/GaAs (001). Blue curve is the potential through an insulating hBN spacer, in which there is no screening. Red curves are the screened potential through graphene for different graphene carrier densities. Dotted black curve is the Lennard-Jones potential of graphene. Solid black curve is the Morse potential for a bare GaAs substrate. Adapted from Kawasaki and Campbell, "An analytical model for the remote epitaxial potential," arXiv:2507.09913 (2025) [34].

Morse potential describes a pairwise bonding interaction, rather than the purely electrostatic interaction computed by DFT, and is defined by simple, interpretable parameters that are well benchmarked by experiments and theory.

How can one analyze these interference patterns to isolated the contributions from graphene and the substrate, in a bias- free way? We propose beating and Fourier analysis. Fig. 4(a- c) shows the essentials of this analysis, using a 1D model for the graphene and substrate lattices as sine waves with frequency  $Q_{gr}$  and  $Q_{sub}$ . The sum of these wave produces an interference pattern with beat frequency  $(Q_{sub} - Q_{gr}) / 2$  (dotted line). In reciprocal space, the Fourier transform displays peaks at  $Q_{gr}$  and  $Q_{sub}$ , allowing a bias- free analysis of the relative strengths of the graphene versus substrate potentials. Notably, the beat frequency does not appear in the Fourier analysis because it is not an independent frequency, it merely arises from interference between the two waves. These complementary real space and reciprocal space techniques may help to more rigorously define the different contributions to the potential fluctuation  $\Delta \phi$ .

# III. TO WHAT EXTENT DOES GRAPHENE INTERACT WITH A SUBSTRATE OR WITH A FILM?

Beyond the simple- out- of plane relaxation models of Figs. 1 and 2, in many clean systems, strong graphene/substrate interactions induce reconstructions

![](https://cdn-mineru.openxlab.org.cn/result/2025-08-07/d6c606d7-b5fc-4ba1-8c91-63b6ed66274b/d19439a79adc6ce8a410fce61354335599f3aa205c02a1b4e46d698abe65d83c.jpg)  
FIG. 4. Graphene induced surface reconstructions. (a-d) Schematic lattice potential  $\phi (x)$  above crystalline surfaces and their Fourier transform  $\hat{\phi} (Q)$ . (e) STM image of the  $(6\sqrt{3} \times 6\sqrt{3})$ $R30^{\circ}$  reconstruction of buffer-layer graphene/SiC(0001). From Hiebel et. al., Phys. Rev. B 80, 235429 (2009) [36] with permission from the American Physical Society. (f) STM image of the "6  $\times$  2" reconstruction of graphene/Ge(110). From Campbell et. al. Phys. Rev. Materials 2, 044004 (2018) [37] with permission from the American Physical Society. (g) STM image of the graphene/Ir (111) with  $(10 \times 10)_{gr} / (9 \times 9)_{tr}$  moiré structure. The x marks the HCP site that is favored for nucleation. From N'Diaye et. al. Phys. Rev. Lett. 97, 215501 (2006) [38] with permission from the American Physical Society. (h, j) Cross-sectional structural models of graphene on SiC(0001), Ge(110), and Ru(0001). Graphene/Ge model from Rogge et. al. MRS Commun. 5, 539-546 (2015) [39] under Creative Commons Attribution 4.0 International License. Graphene/Ir adapted from Hämäläinen et. al. Phys. Rev. B 88, 201406(R) (2013) [40] with permission from the American Physical Society.

within the plane, in addition to the buckling relaxations out- of- plane. These reconstructions introduce a new periodicity  $a_{\text{reconstruction}}$  which can be analyzed with the same Fourier analysis (Fig. 4(d)) and challenge the idea of graphene being "transparent" with regard to the substrate. We highlight a few representative examples and their impacts on epitaxial film ordering, drawing on the broader field of moiré epitaxy.

Buffer graphene on Si- face SiC (0001), which forms a  $(6\sqrt{3} \times 6\sqrt{3})R30^{\circ}$  reconstruction, is a canonical example. A scanning tunneling microscopy (STM) image of this surface is shown in Fig. 4(e). Here the buffer carbon layer is not fully graphitic. Instead, core level spectroscopy reveals that it has mixed hybridization with  $\sim 75\% sp^2$  and  $\sim 25\% sp^3$  character [30], strong bonding to the SiC substrate, out- of- plane dangling bonds, 0.4 Å buckling in the graphene, and both in- plane and out- of- plane distortions in the first layer of SiC [30, 41- 43]. This deviation from graphitic  $sp^2$  character also opens a bandgap in buffer graphene [31, 44]. The bandgap is important because it reduces the free carrier screening of the substrate potential, compared to the screening from metallic graphene. Thus, the remote potential through a semiconducting buffer graphene is expected to

be larger than the remote substrate potential through metallic graphene. However, the buckled buffer layer, with its dangling bonds, may introduce larger local potential fluctuations than flat graphene, potentially dominating over any remote field effects from the substrate.

The large structural distortion of buffer graphene has a significant impact on adatom sticking and film growth. Figure 5(b) shows an STM image of Co atoms deposited on a surface that contains regions of buffer graphene and regions with a second "epitaxial" layer of graphene on top of the buffer [45]. Co clusters stick with higher probability to buffer graphene, than to epitaxial graphene. This preferred sticking on buffer graphene likely arises from the dangling bonds in  $sp^2 /sp^3$  hybridized buffer graphene, compared to the more idealized  $sp^2$  character of epitaxial graphene. Presumably this change in bonding character would be relevant for the growth of remote epitaxial films on SiC buffer layer, indicating a large role for reconstruction in these systems.

Graphene on Ge (110) also reconstructs, into an apparent  $6 \times 2$  pattern (Fig. 4(f)). This reconstruction is characterized by lateral and out of plane reconstructions of the top two Ge layers, with minimal distortions in the graphene itself [37, 46, 47]. Here the graphene retains its semimetallic character. Note while this reconstruction is commonly referred to as  $6 \times 2$  its true periodicity is defined by  $\mathbf{b} = \begin{bmatrix} 5 & \mathbf{I} \\ 2 & 2 \end{bmatrix} \mathbf{a}$ , where  $\mathbf{b}$  are the vectors of the surface reconstruction and  $\mathbf{a}$  are the  $(1 \times 1)$  Ge(110) surface unit cell vectors [37].

Finally, even graphene on metallic surfaces induces reconstructions. Fig. 4(g) shows a STM image of graphene on Ir (111). The  $\sim 10\%$  lattice mismatch between graphene and Ir produces a supercell with  $\sim 2.5 \mathrm{nm}$  periodicity, corresponding to  $(9 \times 9)$  Ir unit cells and  $(10 \times 10)$  graphene unit cells. Photoemission and scanning probe measurements reveal that the graphene is buckled by  $\Delta z \approx 0.3 \mathrm{\AA}$ , due to the periodic modulation in Ir- C atomic alignment, which changes the Ir  $5d - \mathrm{C} 2p_z$  hybridization strength [38, 48, 49]. Moire- driven reconstructions have also been observed on  $\mathrm{gr / Ru(0001)[50 - 52]}$ ,  $\mathrm{gr / Rh(111)[53, 54]}$ ,  $\mathrm{gr / Ni(111)[55, 56]}$ ,  $\mathrm{gr / Pt(111)[57]}$ , and  $\mathrm{gr / Cu(111)[58 - 60]}$  with interaction strengths spanning from strong chemisorption (e.g., Ni, Rh) to weak van der Waals bonding (e.g., Cu, Pt) [48, 49].

These graphene/metal moire lattices are known to template the ordered assembly of adatoms and adatom clusters. Figure 5(d) shows an STM image of a fractional monolayer of Ir deposited on graphene/Ir(111). The Ir crystallizes in ordered arrays of metal clusters that follow the  $(9 \times 9)_{Ir} / (10 \times 10)_{gr}$  moire periodicity [38]. Here, the Ir clusters preferentially nucleate at the hexagonal close packed (HCP) sites within the moire cell. Similar moire ordered assembly has been observed in other graphene/metal systems including Pt deposition on graphene/Ru(0001) [54, 61- 63], Pt deposition on graphene/Cu(111)[59], and Ni deposition on graphene/Rh(111)[54].

![](https://cdn-mineru.openxlab.org.cn/result/2025-08-07/d6c606d7-b5fc-4ba1-8c91-63b6ed66274b/a1fea892f306b6ee56f61a5b3913e03c3812fd6183edca3967ec8d9008ee87d5.jpg)  
FIG. 5. Impact of graphene moire and reconstructions on nucleation and epitaxy. (a,b) Models for adatom sticking and ordering on graphene/SiC and graphene/Ir. (c) STM image of preferred Co sticking on buffer graphene vs. epitaxial graphene on SiC(0001). Adapted from Poon et. al. Phys. Chem. Chem. Phys., 12, 13522-13533 (2010) [45] with permission from the Royal Society of Chemistry. (d) Ordered superlattice of Ir clusters that follows the moire periodicity of graphene/Ir(111). Adapted from N'Drave et. al. Phys. Rev. Lett. 97, 215501 (2006) [38] with permission from the American Physical Society.

Epitaxial ordering on graphene/metal moire templates lies in apparent contrast to the polar bonding hypothesis for remote epitaxy. Recall that the electrostatic potential analysis by Kong et. al. suggested the remote potential fluctuations should be strongest for materials with polar bonding [24]. In contrast, Ir (111) has metallic bonding. For Ir on graphene/Ir (111) the ordering is thought to be driven by the reactivity of Ir to the HCP sites within the moire cell [38], rather than remote epitaxy through transparent graphene. Further studies are required to connect the ordering of adatom clusters or graphene/substrate moire templates, which have more periodicity of a few nanometers, to the continuous films of remote epitaxy that have lattice constant of a few Angstrom.

Furthermore, these reconstructions complicate the initial mechanistic picture of remote epitaxy that the graphene layer allows the film periodicity to less strongly match the substrate periodicity. Which lattice would the film be interacting with: the bulk substrate or the graphene induced reconstruction (or both)? If the insertion of graphene removes the film's lattice matching requirement with the bulk substrate, but replaces this with a lattice matching requirement with the resulting reconstruction, then remote epitaxy is arguably just an extension of regular epitaxial principles to a new surface induced by the addition of graphene.

# IV. HOW DO GRAPHENE/SUBSTRATE INTERACTIONS TUNE ADATOM KINETICS?

Just as the underlying substrate is expected to tune the remote lattice potential, the substrate is also expected to tune adatom diffusion on graphene- covered surfaces. Growth kinetics have been underexplored in the context of remote epitaxy, but have been considered more extensively in the surface science literature. Fig. 6 summarizes the DFT computed surface diffusion barrier heights  $E_{d}$  for several metal adatoms on graphene- covered metal surfaces [64- 71]. In Fig. 6(a) we plot  $E_{d}$  versus the measured or computed topographical corrugation height of graphene on these surfaces, since this corrugation is a proxy for the graphene- substrate interaction strength [49]. As the substrate is changed,  $E_{d}$  for Au adatoms systematically increases going from bare graphene  $\Delta z = 0.02 \mathrm{\AA}$  [72] to graphene/Cu (111)  $\Delta z = 0.12 \mathrm{\AA}$ , [73] to buffer graphene/SiC  $\Delta z = 0.86 \mathrm{\AA}$  [72] to graphene/Ru(0001)  $\Delta z = 1.7 \mathrm{\AA}$ . [74] For a fixed graphene/Ru(0001) substrate and varying the adatom (Fig. 6(b)), the barrier height also changes significantly and follows a general trend of valence electron count of the adatom. These data suggest that kinetics, which are tunable via the graphene/substrate interface, may play a significant role in tuning the growth mechanisms and structure of films grown on graphene- covered surfaces, in addition to the thermodynamic conditions discussed in the previous sections. "Remote" tuned diffusion barriers go beyond the typical kinetic tuning knobs of growth rate and sample temperature.

These kinetic factors are essential, yet underexplored, parameters for tuning between the anticipated remote epitaxy and other competing growth mechanisms. For conventional epitaxy on covalent surfaces, the growth mode is highly dependent on the relations between surface diffusivity  $D$  , adatom flux  $j$  , and spacing between atomic steps on the substrate  $L_{step}$  . Note that  $D$  relates to the barrier height via  $D = D_{0}exp(E_{d} / k_{B}T)$  .From these parameters one can define a dimensionless Peclet number  $P_e = (L_{step}^2 j) / D$  that separates different growth modes:  $P_e< 1$  leads to step- flow growth,  $P_e > 1$  to layer- by- layer growth, and  $P_e > > 1$  to statistical growth [76].

For epitaxy on graphene- covered surfaces, the kinetic regimes are not well known, although one limiting case has been studied. For transferred graphene- covered surfaces, where pinholes are the primary defect, Manzo et. al. showed that when the diffusion length  $\lambda$  is greater than the spacing between pinholes  $L_{p}$  , nucleation occurs preferentially at pinholes where there is direct bonding to the substrate [19]. Note that  $\lambda = 2\sqrt{D\tau}$  where  $\mathcal{T}$  is the diffusion time. This selective nucleation is followed by lateral coalescence of a continuous film. Since the pinholes are typically only a few nanometers in diameter, films grown by the pinhole mechanism can be exfoliated, and thus share many of the macroscopic hallmarks that are expected for films that grow by a re mote epitaxy mechanism. Further studies are required to investigate how tuning surface diffusion, and tuning both the identity and concentration of different types of defects, tunes the growth mode on graphene- covered surfaces. While a pinhole mechanism dominates when there is a high concentration of pinholes or larger openings in graphene [19, 77- 82], perhaps other sites such as graphene- covered atomic step edges or local variations in the graphene/substrate registry could be the nucleation sites for a true remote epitaxy mechanism (Fig. 6(c)).

![](https://cdn-mineru.openxlab.org.cn/result/2025-08-07/d6c606d7-b5fc-4ba1-8c91-63b6ed66274b/5d922c39b0125f1456372379f47ad1db4c2a2cfd37db5c2ecee8a9aa2a5ba9b8.jpg)  
FIG. 6. Tunable surface diffusion barriers on graphene-covered substrates. (a) Diffusion barrier for an Au adatom on graphene/substrate, for different substrates. (b) Diffusion barrier for different adatoms on graphene/Ru (0001). DFT computed diffusion barrier data from Refs [64-71]. Measured/computed corrugation heights, measured by STM and by X-ray standing wave (XSW) are from Refs [72-75]. (c) Typical defects observed on graphene-covered surfaces. Defects are expected to be the nucleation sites for remote epitaxy and for competing mechanisms.

# V.OUTLOOK

How transparent is graphene? Our critical analysis of DFT slab calculations [5, 24] and analytical modeling [34] suggests that for weakly interacting graphene/substrate systems, the remote potential of the substrate is significantly attenuated by graphene. For many commonly used substrates, the remote substrate potential and the graphene potential have similar magnitude. We proposed a Fourier analysis to analyze the interference patterns between graphene and substrate in a bias- free way.

The literature on graphene- induced reconstructions suggest that systems with strong graphene/substrate interactions are a significant deviation from the transparent limit. In these systems, deviations from ideal  $sp^2$  bonding and variations in local registry of the graphene lattice on the substrate lattice can significantly impact sticking and template long range ordering of adatoms. This epitaxial ordering stretches the concept of remote epitaxy: here the graphene is not a passive transparent layer. Instead, the substrate imprints a deformation or local symmetry breaking in the graphene, which then templates the ordering of adatoms on the graphene. This can be viewed as a series of direct (nearest neighbor) substrategraphene and graphene- film interactions, rather than a purely "remote" interaction that is transmitted through passive graphene. These effects are well studied in the limit of a few monolayers of adatoms on highly interacting graphene, and further studies are required to connect these insights to continuous films on graphene.

Many outstanding questions remain. What type(s) of interactions are most important for the ordering in remote epitaxy: covalent hybridization, van der Waals interactions, electrostatics, or some combination of these interactions? How can we distinguish a purely "remote" mechanism through transparent graphene, versus a series of direct substrate- graphene plus graphene- film interactions? How do kinetics tune the growth mechanisms, and how does nucleation on graphene- covered surfaces proceed? We suggest the following directions for the field:

1. Direct measurements of the remote potential, to test model predictions and distinguish effects of the remote potential versus growth kinetics. AFM-based force-distance spectroscopy [27, 28, 83, 84] and thermal desorption spectroscopy [35-87] are two possible methods to measure covalent and van der Waals contributions. Photoemission electron microscopy (PEEM) and low energy electron microscopy (LEEM) [88-90], Kelvin probe microsoppy (KPFM) [91, 92], and ballistic electron emission microscopy (BEEM) [93, 94] are suited for measuring electrostatic contributions.

2. Systematic growth studies that vary the kinetics. Growth temperature, growth rates, precursor type, and defect identity and density are all key parameters that may enable tuning of remote

epitaxy versus other mechanisms [19].

3. Cleaner graphene/substrate systems that avoid the use of solvents or etchants during transfer, or new methods for graphene growth directly on the substrate of interest. Cleaner graphene is critical identify intrinsic contributions to remote epitaxy rather than other mechanisms like pinhole-seeded lateral overgrowth.

To provide relevant information, we suggest that future first- principles theoretical calculations of remote epitaxy address these issues as well. Specifically, they must provide isolated slab calculations which include graphene layer(s) above the substrate, any relevant reconstructions of the graphene/substrate, and interaction between the substrate and film. Ideally, these calculations would capture information relevant to the kinetics of growth such as diffusion barriers for individual atoms or sliding barriers for islands. While requiring significant additional computation, calculations which also include graphene pinholes, defects, and step edges would be invaluable for understanding how these impact real- world bonding potentials and growth.

# VI. ACKNOWLEDGMENTS

JKK thanks Michael Arnold, Paul Evans, and Chris Palmstrom for helpful discussions.

This work was primarily supported by the U.S. Department of Energy, Office of Science, Basic Energy Sciences, under award no. DE- SC0023958 (AS and JKK). ZL and QTC were supported by the Laboratory Directed Research and Development Program at Sandia National Laboratories under project 233271. JKK and ZL acknowledge preliminary support from the Air Force Office of Scientific Research (FA9550- 21- 0127).

This work was performed, in part, at the Center for Integrated Nanotechnologies, an Office of Science User Facility operated for the U.S. Department of Energy (DOE) Office of Science. Sandia National Laboratories is a multi- mission laboratory managed and operated by National Technology & Engineering Solutions of Sandia, LLC (NTESS), a wholly owned subsidiary of Honeywell International Inc., for the U.S. Department of Energy's National Nuclear Security Administration (DOE/NNSA) under contract DE- NA0003525. This written work is authored by an employee of NTESS. The employee, not NTESS, owns the right, title and interest in and to the written work and is responsible for its contents. Any subjective views or opinions that might be expressed in the written work do not necessarily represent the views of the U.S. Government. The publisher acknowledges that the U.S. Government retains a non- exclusive, paid- up, irrevocable, world- wide license to publish or reproduce the published form of this written work or allow others to do so, for U.S. Government purposes. The DOE will provide public access to results of federally sponsored research in accordance with the DOE Public Access Plan.

[1] Y. Kim, S. S. Cruz, K. Lee, B. O. Alawode, C. Choi, Y. Song, J. M. Johnson, C. Heidelberger, W. Kong, S. Choi, et al., Nature 544, 340 (2017). [2] Y. Kim, J. M. Suh, J. Shin, Y. Liu, H. Yeon, K. Qiao, H. S. Kum, C. Kim, H. E. Lee, C. Choi, et al., Science 377, 859 (2022). [3] D. Du, S. Manzo, C. Zhang, V. Saraswat, K. T. Genser, K. M. Rabe, P. M. Voyles, M. S. Arnold, and J. K. Kawasaki, Nature communications 12, 2494 (2021). [4] Z. LaDuca, T. Samanta, N. Hagopian, T. Jung, K. Su, K. Genser, K. M. Rabe, P. M. Voyles, M. S. Arnold, and J. K. Kawasaki, Nano Letters 24, 10284 (2024). [5] L. Dai, J. Zhao, J. Li, B. Chen, S. Zhai, Z. Xue, Z. Di, B. Feng, Y. Sun, Y. Luo, et al., Nature Communications 13, 2990 (2022). [6] H. S. Kum, H. Lee, S. Kim, S. Lindemann, W. Kong, K. Qiao, P. Chen, J. Irwin, J. H. Lee, S. Xie, et al., Nature 578, 75 (2020). [7] Z. LaDuca, K. Su, S. Manzo, M. S. Arnold, and J. K. Kawasaki, Physical Review Materials 7, 083401 (2023). [8] L. K. H.- Y. K. S. Q. K. C. C. N. Y. K. H.- K. H. S. C. P. K. W. K. B.- S. K. C. L. J. B. Y. S. J. P. J. J. M. M. D. A. L. K. K. J. Bae, Sang- Hoon, Nanoscale 6, 7503 (2014), URL http://dx.doi.org/10.1039/C3NR06771H. [9] J. Jiang, X. Sun, X. Chen, B. Wang, Z. Chen, Y. Hu, Y. Guo, L. Zhang, Y. Ma, L. Gao, et al., Nature communications 10, 4145 (2019). [10] B. Liu, Q. Chen, Z. Chen, S. Yang, J. Shan, Z. Liu, Y. Yin, F. Ren, S. Zhang, R. Wang, et al., Nano Letters 22, 3364 (2022). [11] M. Yuan, J. Feng, H. Li, H. Gao, Y. Qiu, L. Jiang, and Y. Wu, Nature Nanotechnology 20, 381 (2025). [12] I. Roh, S. H. Goh, Y. Meng, J. S. Kim, S. Han, Z. Xu, H. E. Lee, Y. Kim, and S.- H. Bae, Nano Convergence 10, 20 (2023). [13] D. Du, J. Hu, and J. K. Kawasaki, Applied Physics Letters 122 (2023). [14] M. Park, T. Maekawa, K. Hwang, J. Cable, W. Noriyuki, K. Choi, Y.- K. Noh, Y. Oh, Y. Baek, and K. Lee, Nature Reviews Electrical Engineering 1, 680 (2024). [15] H. Kim, C. S. Chang, S. Lee, J. Jiang, J. Jeong, M. Park, Y. Meng, J. Ji, Y. Kwon, X. Sun, et al., Nature Reviews Methods Primers 2, 40 (2022). [16] J. Ji, H.- M. Kwak, J. Yu, S. Park, J.- H. Park, H. Kim, S. Kim, S. Kim, D.- S. Lee, and H. S. Kum, Nano Convergence 10, 19 (2023). [17] H. Ryu, H. Park, J.- H. Kim, F. Ren, J. Kim, G.- H. Lee, and S. J. Pearton, Applied Physics Reviews 9 (2022). [18] Z. Liu, B. Liu, Z. Chen, S. Yang, Z. Liu, T. Wei, P. Gao, and Z. Liu, National Science Open 2, 20220068 (2023). [19] S. Manzo, P. J. Strohbeen, Z. H. Lim, V. Saraswat, D. Du, S. Xu, N. Pokharel, L. J. Mawst, M. S. Arnold, and J. K. Kawasaki, Nature communications 13, 4014 (2022). [20] H. Kim, J. C. Kim, Y. Jeong, J. Yu, K. Lu, D. Lee, N. Kim, H. Y. Jeong, J. Kim, and S. Kim, Journal of Applied Physics 130 (2021). [21] H. Kim, K. Lu, Y. Liu, H. S. Kum, K. S. Kim, K. Qiao, S.- H. Bae, S. Lee, Y. J. Ji, K. H. Kim, et al., ACS nano 15, 10587 (2021). [22] H. Yoon, T. K. Truttmann, F. Liu, B. E. Matthews,

S. Choo, 
Q. Su, 
V. Saraswat, 
S. Manzo, 
M. 
S. Arnold, 
M. 
E. Bowden, et al., Science Advances 8, eadd5328 (2022). [23] 
D. Du, 
T. Jung, 
S. Manzo, 
Z. LaDuca, 
X. Zheng, 
K. Su, 
V. Saraswat, 
J. McChesney, 
M. 
S. Arnold, and 
J. 
K. Kawasaki, Nano Letters 22, 8647 (2022). [24] 
W. Kong, 
H. Li, 
K. Qiao, 
Y. Kim, 
K. Lee, 
Y. Nie, 
D. Lee, 
T. Osadchy, 
R. 
J. Molnar, 
D. 
K. Gaskill, et al., Nature materials 17, 999 (2018). [25] 
J. Rafiee, 
X. Mi, 
H. Gullapalli, 
A. 
V. Thomas, 
F. Yavari, 
Y. Shi, 
P. 
M. Ajayan, and 
N. 
A. Koratkar, Nature materials 11, 217 (2012). [26] 
C.-J. Shih, 
Q. 
H. Wang, 
S. Lin, 
K.-C. Park, 
Z. Jin, 
M. 
S. Strano, and 
D. Blankschtein, Physical review letters 109, 176101 (2012). [27] 
S. Ke, 
T. Uda, and 
K. Terakura, Physical Review B 59, 13267 (1999). [28] 
P. Allain, 
D. Damiron, 
Y. Miyazaki, 
K. Kaminishi, 
F. Pop, 
D. Kobayashi, 
N. Sasaki, and 
H. Kawakatsu, Applied Physics Letters 111 (2017). [29] 
E. Bauer, Reports on Progress in Physics 57, 895 (1994). [30] 
M. Conrad, 
J. Rault, 
Y. Utsumi, 
Y. Garreau, 
A. Vlad, 
A. Coati, 
J.-P. Rueff, 
P. 
F. Miceli, and 
E. 
H. Conrad, Phys. Rev. B 96, 195304 (2017), URL https://link.aps.org/doi/10.1103/PhysRevB.96.195304. [31] 
M. 
N. Nair, 
I. Palacio, 
A. Celis, 
A. Zobelli, 
A. Gloter, 
S. Kubsky, 
J.-P. Turmaud, 
M. Conrad, 
C. Berger, 
W. de Heer, et al., Nano letters 17, 2681 (2017). [32] 
M. 
S. Dresselhaus and 
G. Dresselhaus, Advances in Physics 30, 139 (1981). [33] 
Y. Wang, 
Y. Qu, 
Y. Xu, 
D. Li, 
Z. Lu, 
J. Li, 
X. Su, 
G. Wang, 
L. Shi, 
X. Zeng, et al., ACS nano 17, 4023 (2023). [34] 
J. 
K. Kawasaki and 
Q. 
T. Campbell, An analytical model for the remote epitaxial potential (2025), 2507.09913, URL https://arxiv.org/abs/2507.09913. [35] 
K. Qiao, 
Y. Liu, 
C. Kim, 
R. 
J. Molnar, 
T. Osadchy, 
W. Li, 
X. Sun, 
H. Li, 
R. 
L. Myers-Ward, 
D. Lee, et al., Nano letters 21, 4013 (2021). [36] 
F. Hiebel, 
P. Mallet, 
L. Magaud, and 
J.-Y. Veuillen, Phys. Rev. B 80, 235429 (2009), URL https://link.aps.org/doi/10.1103/PhysRevB.80.235429. [37] 
G. 
P. Campbell, 
B. Kiraly, 
R. 
M. Jacobberger, 
A. 
J. Mannix, 
M. 
S. Arnold, 
M. 
C. Hersam, 
N. 
P. Guisinger, and 
M. 
J. Bedzyk, Phys. Rev. Mater. 2, 044004 (2018), URL https://link.aps.org/doi/10.1103/PhysRevMaterials.2.044004. [38] 
A. 
T. N'Diaye, 
S. Bleikamp, 
P. 
J. Feibelman, and 
T. Michely, Phys. Rev. Lett. 97, 215501 (2006), URL https://link.aps.org/doi/10.1103/PhysRevLett.97.215501. [39] 
F. 
M. 
E.-W. 
J. 
M. 
M. 
K. 
F. 
B. 
N. 
C. 
D. 
O. 
D. Rogge, 
P. 
C., MRS Communications 5 (2015), URL https://doi.org/10.1557/mrc.2015.63. [40] 
S. 
K. Hamalainen, 
M. 
P. Booneschanscher, 
P. 
H. Jacobse, 
I. Swart, 
K. Pussi, 
W. Moritz, 
J. Lahti-nen, 
P. Liljeroth, and 
J. Sainio, Phys. Rev. B 88, 201406 (2013), URL https://link.aps.org/doi/10.1103/PhysRevB.88.201406. [41] 
K. Emtsev, 
F. Speck, 
T. Seyler, 
L. Ley, and 
J. 
D. Riley, Physical Review B—Condensed Matter and Materi-

als Physics 77, 155303 (2008). [42] A. Van Bommel, J. Crombeen, and A. Van Tooren, Surface Science 48, 463 (1975). [43] I. Forbeaux, J.- M. Themlin, and J.- M. Debever, Physical Review B 58, 16396 (1998). [44] M. Nevius, M. Conrad, F. Wang, A. Celis, M. Nair, A. Taleb- Ibrahimi, A. Tejeda, and E. Conrad, Physical review letters 115, 136802 (2015). [45] S. W. Poon, W. Chen, A. T. S. Wee, and E. S. Tok, Phys. Chem. Chem. Phys. 12, 13522 (2010), URL http: //dx.doi.org/10.1039/B927452A. [46] W. Chen, X. Wang, S. Li, C. Yan, L. He, P. Zhang, Y. Yang, D. Ma, J. Nie, and R. Dou, Phys. Chem. Chem. Phys. 22, 23711 (2020), URL http://dx.doi.org/10.1039/DOCP03322G. [47] B. Kiraly, R. M. Jacobberger, A. J. Mannix, G. P. Campbell, M. J. Bedzyk, M. S. Arnold, M. C. Hersam, and N. P. Guisinger, Nano Letters 15, 7414 (2015), pMID: 26506006, https://doi.org/10.1021/acs.nanolett.5b02833, URL https://doi.org/10.1021/acs.nanolett.5b02833. [48] Y. Dedkov, E. Voloshina, and M. Fonin, physica status solidi (b) 252, 451 (2015), https://onlinelibrary.wiley.com/doi/pdf/10.1002/pssb.201451466, L. Semidey- Flecha, D. Teng, B. F. Habenicht, URL https://onlinelibrary.wiley.com/doi/abs/10.1002/pssb.201451466. [49] A. B. Preobrajenski, M. L. Ng, A. S. Vinogradov, and N. Martensson, Phys. Rev. B 78, 073401 (2008), URL https://link.aps.org/doi/10.1103/PhysRevB.78.073401. [50] D. Martoccia, P. R. Willmott, T. Brugger, M. Bjorck, S. Gunther, C. M. Schleputz, A. Cervellino, S. A. Pauli, B. D. Patterson, S. Marchini, et al., Phys. Rev. Lett. 101, 126102 (2008), URL https://link.aps.org/doi/10.1103/PhysRevLett.101.126102. [51] H. T. Zhou, J. H. Mao, G. Li, Y. L. Wang, X. L. Feng, S. X. Du, K. Mullen, and H.- J. Gao, Applied Physics Letters 99, 153101 (2011), ISSN 0003- 6951, https://pubs.aip.org/aip/apl/article- pdf/doi/10.1063/1.3646406/14458449/153101_1_online.pdf, URL https://doi.org/10.1063/1.3646406. [52] B. Borca, S. Barja, M. Garnica, D. Sanchez- Portal, V. M. Silkin, E. V. Chulkov, C. F. Hermanns, J. J. Hinarejos, A. L. Vazquez de Parga, A. Arnau, et al., Phys. Rev. Lett. 105, 036804 (2010), URL https://link.aps.org/doi/10.1103/PhysRevLett.105.036804. [53] A. Holtsch, T. Kuwens, B. Uder, S. Grandthyll, F. Muller, and U. Hartmann, Surface Science 668, 107 (2018), ISSN 0039- 6028, URL https://www.sciencedirect.com/science/article/pii/S0039602817305551. [54] M. Sicot, S. Boavron, O. Zander, U. Reidiger, Y. S. Dedkov, and M. Fonin, Applied Physics Letters 96, 093115 (2010), ISSN 0003- 6951, https://pubs.aip.org/aip/apl/article- pdf/doi/10.1063/1.3341176/14427676/093115_1_online.pdf, URL https://doi.org/10.1063/1.3341176. [55] Z. Zou, V. Carnevali, M. Jugovac, L. L. Patera, A. Sala, M. Panighel, C. Cepek, G. Soldano, M. M. Mariscal, M. Peressi, et al., Carbon 130, 441 (2018), ISSN 0008- 6223, URL https://www.sciencedirect.com/science/article/pii/S0008622318300101. [56] A. Dahal and M. Batzill, Nanoscale 6, 2548 (2014). [57] M. P. P.- A. L. G. O.- I. L. M. F. M. J. M.- G. J. A.

Martinez, Jose I, Scientific Reports 6 (2016). [58] P. Sule, M. Szendro, C. Hwang, and L. Tapasztó, Carbon 77, 1082 (2014), ISSN 0008- 6223, URL https://www.sciencedirect.com/science/article/pii/S0008622314005703. [59] E. Soy, Z. Liang, and M. Trenary, The Journal of Physical Chemistry C 119, 24796 (2015), https://doi.org/10.1021/acs.jpcc.5b06472, URL https://doi.org/10.1021/acs.jpcc.5b06472. [60] L. Gao, J. R. Guest, and N. P. Guisinger, Nano Letters 10, 3512 (2010), pMID: 20677798, https://doi.org/10.1021/nl1016706, URL https://doi.org/10.1021/nl1016706. [61] Y. Pan, M. Gao, L. Huang, F. Liu, and H.- L. Gao, Applied Physics Letters 95, 093106 (2009), ISSN 0003- 6951, https://pubs.aip.org/aip/apl/article- pdf/doi/10.1063/1.3223781/14418505/093106_1_online.pdf, URL https://doi.org/10.1039/1.3223781. [62] K. Donner and P. Jakob, The Journal of Chemical Physics 131, 164701 (2009), ISSN 0021- 9606, https://pubs.aip.org/aip/jcp/article- pdf/doi/10.1063/1.3246166/13578030/164701_1_online.pdf, URL https://doi.org/10.1063/1.3246166. [63] M. Amft, B. Sanyal, O. Eriksson, and N. V. Skorodumova, Journal of Physics: Condensed Matter 23, 205301 (2011), URL https://dx.doi.org/10.1088/0953- 8984/23/20/205301. [64] P. Jensen, X. Blase, and P. Ordejon, Surface Science 564, 173 (2004), ISSN 0039- 6028, URL https://www.sciencedirect.com/science/article/pii/S0039602804008933. [65] R. Anton and I. Schneiderleit, Phys. Rev. B 58, 13874 (1998), URL https://link.aps.org/doi/10.1103/PhysRevB.58.13874. [66] X. Liu, Y. Han, J. W. Evans, A. K. Engstfeld, R. J. Behm, M. C. Tringides, M. Hupalo, H.- Q. Lin, L. Huang, K.- M. Ho, et al., Progress in Surface Science 90, 397 (2015), ISSN 0079- 6816, URL https://www.sciencedirect.com/science/article/pii/S0079681615000222. [67] L. Semidey- Flecha, D. Teng, B. F. Habenicht, D. S. Sholl, and Y. Xu, The Journal of Chemical Physics 138, 184710 (2013), ISSN 0021- 9606, https://pubs.aip.org/aip/jcp/article- pdf/doi/10.1063/1.4803893/13280902/184710_1_online.pdf, URL https://doi.org/10.1063/1.4803893/13280902/184710_1_online.pdf, URL https://doi.org/10.1063/1.4803893. [68] D. S. Sholl, and Y. Xu, The Journal of Chemical Physics 138, 184710 (2013), ISSN 0021- 9606, https://pubs.aip.org/aip/jcp/article- pdf/doi/10.1063/1.4803893/13280902/184710_2013_1.2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013- 2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013 0021- 9606, https://pubs.aip.org/aip/jcp/article- pdf/doi/10.1063/1.4803893/13280902/184710_1_online.pdf, URL https://doi.org/10.1063/1.4803893/13280902- 1.2013_1.2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_2013_20

URL https://doi.org/10.1063/1.4866876. [72] J. Sforzini, L. Nemec, T. Denig, B. Stadtmuller, T.- L. Lee, C. Klumpf, S. Soubatch, U. Starke, P. Rinke, V. Blum, et al., Phys. Rev. Lett. 114, 106804 (2015), URL https://link.aps.org/doi/10.1103/PhysRevLett.114.106804. [73] M. A. Stoodley, L. A. Rochford, T.- L. Lee, B. P. Klein, D. A. Duncan, and R. J. Maurer, Phys. Rev. Lett. 132, 196201 (2024), URL https://link.aps.org/doi/10.1103/PhysRevLett.132.196201. [74] M. Gao, Y. Pan, C. Zhang, H. Hu, R. Yang, H. Lu, J. Cai, S. Du, F. Liu, and H.- J. Gao, Applied Physics Letters 96, 053109 (2010), ISSN 0003- 6951, https://pubs.acip.org/epi/ap/article- pdf/doi/10.1063/1.3309671/14426049/053109_1. online.pdf, URL https://doi.org/10.1063/1.3309671. [75] D. Martoccia, P. R. Willmott, T. Brugger, M. Bjorck, S. Gunther, C. M. Schlepütz, A. Cervellino, S. A. Pauli, B. D. Patterson, S. Marchini, et al., Phys. Rev. Lett. 101, 126102 (2008), URL https://link.aps.org/doi/10.1103/PhysRevLett.101.126102. [76] J. Y. Tsao, Materials fundamentals of molecular beam epitaxy (Academic Press, 2012). [77] S. Manzo, K. Su, M. S. Arnold, and J. K. Kawasaki, ACS Applied Materials & Interfaces 15, 59905 (2023). [78] Z. H. Lim, S. Manzo, P. J. Strohbeen, V. Saraswat, M. S. Arnold, and J. K. Kawasaki, Applied Physics Letters 120 (2022). [79] J. Jeong, D. K. Jin, J. Cha, B. K. Kang, Q. Wang, J. Choi, S. W. Lee, V. Y. Mikhailovskii, V. Neplokh, N. Amador- Mendez, et al., ACS Applied Nano Materials 3, 8920 (2020). [80] H. Kim, S. Lee, J. Shin, M. Zhu, M. Ahl, K. Lu, N. M. Han, Y. Baek, C. S. Chang, J. M. Suh, et al., Nature Nanotechnology 17, 1054 (2022).

[81] B. Fazlioglu- Yalcin, M. Wang, N. Nayir, S. Law, and A. C. van Duin, The Journal of Physical Chemistry C 128, 14294 (2024). [82] M. Zulqurnain, O. J. Burton, M. Al- Hada, L. E. Goff, S. Hofmann, and L. C. Hirst, Nanotechnology 33, 485603 (2022). [83] P. M. Hoffmann, A. Oral, R. A. Grimble, H. Ozgür Ozer, S. Jeffery, and J. B. Pethica, Proceedings of the Royal Society of London. Series A: Mathematical, Physical and Engineering Sciences 457, 1161 (2001). [84] F. J. Gießbl, H. Bielefeldt, S. Hembacher, and J. Mannhart, Annalen der Physik 513, 887 (2001). [85] D. A. King, Surface Science 47, 384 (1975). [86] E. Habschendonk and J. Kappers, Surface science letters 138, L147 (1984). [87] L. R. Apker, Industrial & Engineering Chemistry 40, 846 (1948). [88] T. Schmidt, S. Heun, J. Slezak, J. Diaz, K. Prince, G. Lilienkamp, and E. Bauer, Surface Review and Letters 5, 1287 (1998). [89] H. Bethge and M. Klaua, Ultramicroscopy 11, 207 (1983). [90] A. Zakharov, A. Mikkelsen, and J. N. Andersen, Journal of Electron Spectroscopy and Related Phenomena 185, 417 (2012). [91] V. Panchal, R. Pearce, R. Yakimova, A. Tzalenchuk, and O. Kazakova, Scientific reports 3, 2597 (2013). [92] W. A. Behn, Z. J. Krebs, K. J. Smith, K. Watanabe, T. Taniguchi, and V. W. Brar, Nano Letters 21, 5013 (2021). [93] L. D. Bell, Journal of Vacuum Science & Technology B 34 (2016). [94] M. Prietsch, Physics Reports 253, 163 (1995).
