# Design principles for dual-phase lattice cylindrical tubes with excellent energy absorption capability

![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/fa6665ea950a6f8f851558d6c1f2e52b0edb6743de068a84a908e11c8a2feb49.jpg)


Yuan Tian a, Huitian Wang b, Zhuo Chen b, Qianqian Wu c, Sha Yin b,*

$^{a}$  School of Transportation Science & Engineering, Beihang University, Beijing 100191, China

b National Key Laboratory of Strength and Structural Integrity, School of Aeronautic Science and Engineering, Beihang University, Beijing 100191, China

$^{\mathrm{c}}$  National Key Laboratory of Science and Technology on Advanced Composites in Special Environments, Harbin Institute of Technology, Harbin 100086, China

# ARTICLEINFO

# Keywords:

Lattice materials

Cylindrical tube

Bioinspired design

Dual phase

Energy absorption

Deformation mechanism

# ABSTRACT

To further increase specific energy absorption capacity of lattice materials, this study proposed dual-phase lattice cylindrical tubes (DPLCTs) that emulated the sinusoidal-helicoidal architecture of the peacock mantis shrimp. The metamaterial composites were printed from austenitic stainless steel using additive manufacturing and compressed. Quasi-static axial compression tests revealed that DPLCTs exhibited higher specific energy absorption (SEA) than the corresponding single-phase lattice cylindrical tubes (SPLCTs). Those with the largest amplitude-to-width ratio, exhibited superior specific energy absorption, respectively  $74\%$  and  $14\%$  greater than that of matrix phase (MP) and reinforcement phase (RP) based SPLCTs. After the incorporation of the second phase, more complex deformation modes were observed associated with truss plastic buckling or twisting, RP grain rotation or connected RP grains moving along the phase boundary. In addition to the previously reported interaction deformation mechanism of "phase boundary slip", "reinforcement phase rotation" was observed as another deformation mechanism, which could improve the energy absorption capability by postponing densification strain. Together with computational analysis, the interaction deformation mechanism was found to vary depending on amplitude-to-width ratio  $(\gamma)$ . Finally, design principles for lattice cylindrical tubes with greater energy absorption capability were summarized. The study will provide further guidance for the development of impact-resistant engineering structures.

# 1. Introduction

Lightweight metamaterials possessed excellent energy absorption potential for impact protection and thus became more widely used in the fields of transportation, civil engineering and aerospace [1]. Lattice structures were lightweight periodic architectures designed to precisely control physical fields [2], with common cell configurations including truss-based cells [3], plate-based cells [4,5] and shell-based cells [6,7]. Lattice structures were referred to as metamaterials due to their ability to achieve mechanical properties beyond those of traditional materials. Their energy absorption performance could be effectively improved by optimizing constitutive architectures, for example, by introducing bioinspired designs such as hollow truss-based design [8], hierarchical design [9,10] and graded design [11,12]. Energy absorption structures were crucial components of passive safety systems, with applications including the front-end protection structure of vehicles [13-15] and high-speed trains [16], the landing buffer device for spacecraft [17], the

blast-resistant structures [18] and the bridge anti-collision facilities [19]. Higher specific energy absorption (SEA) was a key design objective for energy absorption structures.

The introduction of the second-phase had been shown to effectively improve the energy absorption of lattice metamaterials. Lattice materials with a single orientation were observed to suffer catastrophic failure due to shear bands [20]. Actually, most of nature's materials were hybrid composites with soft-hard multiphases, exhibiting heterogeneous architectures such as "brick-and-mortar" architectures in conch shells [21,22], precipitation hardening and multi-phase hardening architectures in alloys [23,24]. Also, dual-phase lattice metamaterials consisting of a matrix phase (MP) and reinforcement phase (RP) had already been demonstrated to possess greater energy-absorption capability in our previous study by incorporating the phase-boundary slip mechanism [25,26]. Heterogeneous strategies, designed based on existing configurations, significantly expanded the design space [27,28]. However, conventional research on lattice metamaterials mainly focused on regular polyhedral structures, which conflicted with the

<table><tr><td colspan="2">Nomenclature</td><td>d</td><td>Strut diameter of the cell</td></tr><tr><td></td><td></td><td>H</td><td>Height of tubular lattice</td></tr><tr><td>DPLCT</td><td>Dual-phase lattice cylindrical tube</td><td>D1</td><td>Inner diameter of tubular lattice</td></tr><tr><td>SPLCT</td><td>Single-phase lattice cylindrical tube</td><td>D2</td><td>Outer radius of tubular lattice</td></tr><tr><td>MP</td><td>Matrix phase</td><td>σ</td><td>Stress</td></tr><tr><td>RP</td><td>Reinforcement phase</td><td>ε</td><td>Strain</td></tr><tr><td>F-BCC</td><td>Fan-shaped body-centered cubic cell</td><td>E</td><td>Young&#x27;s modulus</td></tr><tr><td>F-FCC</td><td>Fan-shaped face-centered cubic cell</td><td>σtrue</td><td>True stress</td></tr><tr><td>SEA</td><td>Specific energy absorption</td><td>εtrue</td><td>True strain</td></tr><tr><td>x, y, z</td><td>Cartesian coordinate</td><td>m</td><td>Structural mass</td></tr><tr><td>ρ, θ, z</td><td>Polar coordinate</td><td>εD</td><td>Densification strain</td></tr><tr><td>h</td><td>Cell size</td><td>hD</td><td>Densification deformation of the lattice</td></tr><tr><td>α</td><td>Central angle of the fan-shaped cell</td><td>μ</td><td>Efficiency parameter of energy absorption</td></tr><tr><td>n</td><td>Cell numbers along the circumferential direction</td><td>k</td><td>RP grain size in circumferential direction</td></tr><tr><td>γ</td><td>Amplitude-to-width ratio</td><td>k&#x27;</td><td>RP grain size in the longitudinal direction</td></tr><tr><td>φ</td><td>Helicoidal angle</td><td></td><td></td></tr></table>

application requirements of curved components in aerospace vehicles [29], primarily cylindrical components such as the interstages and fuselages. Current research focused on single-phase lattice tubes, with an emphasis on improving their energy absorption properties through cell designs such as auxetic [30], multi-stable [31], sandwich-walled [32,33], and shell-based [34] structures. The dual-phase lattices had advantages in energy absorption, but studies on how a second-phase affected the energy absorption capability of lattice cylindrical tubes remained limited.

Meanwhile, biomimetic design had always been an effective way to improve mechanical performance [35]. Helicoidal architectures were found in the cuticle of most crustacean species [36]. By mimicking natural characteristics, tough double-helicoidal thermoplastic composite laminates [37], lightweight bi-directionally sinusoidal corrugated core sandwich structures [38] and carbon fiber laminates with a sinusoidal helicoidal architecture [39,40] all resulted in a notable enhancement of structural impact resistance.

Although heterogeneous dual-phase lattice metamaterials had provided valuable insights into enhanced energy absorption, the mechanism by which the distribution of the second-phase influenced energy absorption by affecting the deformation modes remained underexplored. Current research had primarily focused on regular polyhedral lattices, leaving their limitations in curved component applications largely unaddressed.

To further increase the energy absorption capability, the above heterogeneous and bioinspired design strategies could be combined and investigated. In this study, we proposed a novel lattice cylindrical tube design that employed the arrangement of a second-phase to mimic toughening microstructures found in nature. The performance of obtained dual-phase lattice cylindrical tubes (DPLCTs) with helicoidal or sinusoidal-helicoidal RP patterns were investigated through experimental tests and numerical simulation.

# 2. Materials and methods

# 2.1. Design

Inspired by the microstructural features of the stomatopod dactyl club of the peacock mantis shrimp (as geometrically illustrated in Fig. 1a) [40,41], dual-phase lattice cylindrical tubes (DPLCTs) consisting of archetected truss materials with a matrix phase (MP) and reinforcement phase (RP) were designed. To obtain the cylindrical lattice structures, the key point was to map an initial three-dimensional cubic lattice unit cell to a three-dimensional fan-shaped hexahedron cell. The six faces of a fan-shaped hexahedral cell included two arc faces and four planes. The generic design guide for the truss-based lattice cell mapping

process was illustrated in Fig. 1b. The axial direction of the cylindrical lattice structure was considered as the  $z$ -axis.

Akin to the crystal microstructure of metals and alloys, the initial cubic cell consisted of an ordered arrangement of nodes (analogous to atoms) connected by struts (equivalent to atomic bonds). The design of the fan-shaped cell was also based on the crystal microstructure. The fan-shaped cell was constructed in two steps:

Step I: Determining the coordinates of lattice points in the fan-shaped cell with reference to the mapping method in Wang's work [42]. The lattice points in a cubic cell had the coordinates  $(x, y, z)$  in the Cartesian coordinate system. The cell size of the initial cubic cell was represented by  $h$ , and the central angle of the fan-shaped cell was  $\alpha$ . Then, the lattice points in the fan-shaped cells had the coordinates  $(\rho, \theta, z)$  in the polar coordinate system, where  $\rho = y$  and  $\theta = \frac{x}{h} \cdot \alpha$ .

Step II: Joining lattice points with struts. The struts included straight beams and curved beams in the fan-shaped cell. To adapt to the shape of the fan-shaped cell, the trusses in the two arc surfaces were curved beams and the others were straight beams.

After employing the above steps, we respectively constructed the fan-shaped body-centered cubic cell (F-BCC) and face-centered cubic cell (F-FCC). Then, a complete lattice cylindrical tube could be obtained by circumferentially and axially arraying fan-shaped cells, as shown in Fig. 1b. The number of unit cells  $n$  along the circumferential direction was determined by the  $\alpha$ , expressed as  $n = 2\pi /\alpha$ . Accordingly, dual-phase lattice cylindrical tubes (DPLCTs) were designed by selecting F-BCC as matrix phase (MP) and F-FCC as reinforcement phase (RP).

By mimicking the microstructure of the peacock mantis shrimp, the reinforcement phase grains of DPLCTs were patterned into sinusoidal-helicoidal forms and incorporated into matrix phase lattice materials, as shown in Fig. 1c.

Subsequently, five types of DPLCT structures were generated with five different arrangements (DPLCT-1, DPLCT-2, DPLCT-3, DPLCT-4 and DPLCT-5) as shown in Fig. 1d. For the sinusoidal-helicoidal RP patterns, amplitude-to-width ratio  $\gamma$  and helicoidal angle  $\varphi$  were two critical parameters and were summarized for the above five architectures in Table 1. The relative density of lattice structures was defined as the ratio of the volume of solid trusses to the overall volume [26]. The number of RP cells (or volume fraction of RP) was kept the same in each layer and column for all the DPLCTs to guarantee full compression in each column or layer [26]. However,  $2\%$  tolerance for relative density existed, because the phase microstructure at the phase boundary was different with the normal one as depicted in Fig. 1e. Note that for the DPLCTs, the central angle of the fan-shaped cell  $\alpha$  was selected as  $30^{\circ}$ , the height of each cell  $h = 6\mathrm{mm}$ , the strut diameter of the cell  $d = 0.8\mathrm{mm}$ , the height of tubular lattice  $H = 36\mathrm{mm}$  with an inner diameter  $D_{1} = 18\mathrm{mm}$  and an outer radius  $D_{2} = 30\mathrm{mm}$ .


a)



Structural configurations in nature


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/f0b767fff50f6ebdaf32eb04a40be459c15d2dbcee9e65dbdc8415a9783f6ad2.jpg)



b)



Cubic cell (C)



Fan-shaped cell (F)



Lattice cylindrical tubes


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/00d72c8f9cd3982ff7a49d6e9e3b50cc3d003a24b4701d4fb334d88d0b4dca4e.jpg)



C-BCC


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/3285ef69b630c3a4d3942ec82880a4e11fbd9e4dc5eba472bd48c3a01b77ffb5.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/ad37efda8b1be11e0f254e59570e81b9a04bbfa1a3db877d6e99c472b63a769c.jpg)



C-FCC


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/b638b61b60db7617e49d1c9501977947afdd991cdc90e175a1bd8860a9d70337.jpg)



$\rightarrow$  先点:  ${M}_{1}\left( {\frac{9}{4},\frac{7}{16}}\right)$


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/d857f03049c7f6baa28ff1e4443545bfe78f079cfee687e8171385a4d8dd91b0.jpg)



For example:



[ \Rightarrow  \;{h}^{2} - {4h} + 4 = 0]



A=（2,1，）



B=（0，R0,0）



$= \left( {{a}_{1} + {a}_{2} + {a}_{3}}\right)  + {a}_{4} + {a}_{5} + {a}_{6}$



$= {\left( -2\right) }^{2}\left( {{R}_{21} - {R}_{2}}\right)$



A=（B-）



2 2



$B_{2} = (R_{0},0,0)$



C.  $P = \left(\frac{a}{b}\right)^{\frac{1}{2}}$



2 1


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/86e71ee5f16fd6a346bad5f7f816970efb14bb6f81278675db6228828247a0c5.jpg)



Transition with  $\alpha$


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/138baf799c1a271b6dbf1145e14b20fc90238c91d7b721670b34baacf0adf2f8.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/79a91969e68c0404fe50ad7a899ea59ce9c24492531b7329d26d73639938e6e6.jpg)



：



D=（-R0）



$= \left( {{2}^{n - 1}\left( {n + 1}\right)  - 1}\right)$



E=（0，R2,0）



F=（0,Ro，）



Lattice points coordinate transition


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/cbe2810399e9e9ac09c7b4ec7c5061925298dfbc09b05c45137aa11abdf76d18.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/263b4228f044b67b4f4d8ac946ffacfe1f93dda92dc92c419af31095e001f9d0.jpg)



F-BCC


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/4fd5e4582d4c4c51b46cedbbda5f321b2f893689ef552a30690b3dc274ffdd3d.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/338b32590d9f6ba57a78f0de4dbb65080d9b41c837adad281d63eda9c5fa4df3.jpg)



F-FCC


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/7fd9303a7f34328435fe7914e2eab4a5d06e72d04b88f51e2f537c77fc54e6e6.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/40e0f5691195ed663f5fd0c94068b4c79736d0ea52544043a445989686929207.jpg)


# Bio-inspired Dual-phase Lattice Cylindrical Tubes (DPLCT)


c)



DPLCT-1


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/b73240f0f330d8755f6a1acba6966d193bd9c6bd99f8dd64974e69dd2716753a.jpg)



$\gamma = 1$ $\varphi = 0^{\circ}$



DPLCT-2


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/865e83753d4167fc6b98040639a48e87a817ba6116013463f2f1a3e48ba51b64.jpg)



$\gamma = 1$



$\varphi = 30^{\circ}$



DPLCT-3


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/ef820e298eff529af8d9bb477f4c78178d25c03c7566e063f04726e600cb8eeb.jpg)



$\gamma = 1$



$\varphi = 90^{\circ}$



DPLCT-4


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/1dbd60d6f97ab9c710ebf90ffd31e53541c37f26940a2c0e04525314bfc70323.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/0eb2698328799fbd3d87a2df1c3188b428c274b9cf25ee3c88ff3804c6fed21b.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/dec4823782d8166914a46cb5892af1f30249ada82b4c2b88fb6269cab3dc9e94.jpg)



DPLCT-5


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/3efeada3df8bd0ac56cdfeed27ac21cf745864bd8d64050bb34dd359d8f8707e.jpg)



RP (FCC)



MP (BCC)



$\gamma = \frac{A}{W}$



d)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/686071d0ef150e94d75492ee747cd1e751f52e2e0ef09a143731b2ee1d61f26f.jpg)



e)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/4cf4e4ff8ad7bcef86ddc848c44e36e87b53f8d762751c74510374f9a1779021.jpg)



Phase boundary network


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/94f029e4e3eacf84fe8207beb727d00a2ad7f910a282c4a1748d8eb9b8cea4a0.jpg)



BCC at the phase boundary


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/cc43c6b19e4a207819d28a1622cbd0092c34198978df00aac127e13165b93a68.jpg)



Normal BCC



f)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/7dc0fd5ac69406e76c7741d7891858a86b8b50b35ad9dfec26633e9be1b09fdc.jpg)



DPLCT-1 DPLCT-2


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/83e88515bfcb2dea1958d8cd6cd3eacd835bf8bf19c39cd179087db481dca6b2.jpg)



DPLCT-4


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/723ce9774d37ccb7f913cd80c894ed53dd1b630383efd8e0af2b1b0fb1164d6f.jpg)



DPLCT-


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/6a0f642dca50941a26d65672b29cdb755893402e769af8b2402de3a69198fb8f.jpg)



MP SPLCT


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/4ef62fa143a0b29c9bef3752bec23122a65492ef7c18184a847427aefbb16e87.jpg)



g)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/073a9848d625fb07cf48856bbfd69372f25b336d2bca61a7b74708de34331c64.jpg)



Fig. 1. Bio-inspired dual-phase lattice cylindrical tubes (DPLCTs) with sinusoidal-helicoidal phase architectures: (a) sinusoidally architeetcd helicoidal structure from peacock mantis shrimp [40,41]; (b) mapping process for lattice cylindrical tubes: from a body-centered cubic (BCC) unit cell and from a face-centered cubic (FCC) unit cell; (c) cylindrical expansion diagrams illustrating five different RP patterns and (d) the corresponding DPLCTs; (e) the  $2\%$  relative density difference among DPLCTs due to BCC unit variations at phase boundaries; (f) samples fabricated by additive manufacturing; (g) mesoscopic printing details and manufacturing defects observed.



Table 1



Geometric parameters of the RP patterns of five types DPLCTs.


<table><tr><td>Samples</td><td>DPLCT-1</td><td>DPLCT-2</td><td>DPLCT-3</td><td>DPLCT-4</td><td>DPLCT-5</td></tr><tr><td>RP pattern</td><td>Sinusoidal-helicoidal</td><td>Sinusoidal-helicoidal</td><td>Sinusoidal-helicoidal</td><td>Sinusoidal-helicoidal</td><td>Helicoidal</td></tr><tr><td>Amplitude</td><td>18 mm</td><td>18 mm</td><td>18 mm</td><td>36 mm</td><td>36 mm</td></tr><tr><td>Width</td><td>18 mm</td><td>18 mm</td><td>18 mm</td><td>18 mm</td><td>36 mm</td></tr><tr><td>Amplitude-to-width ratio (γ)</td><td>1</td><td>1</td><td>1</td><td>2</td><td>1</td></tr><tr><td>Helicoidal angle (φ)</td><td>0°</td><td>30°</td><td>90°</td><td>-</td><td>-</td></tr></table>

# 2.2. Fabrication

Due to the complexity of lattice cylindrical structures, Powder Bed Fusion (PBF) technology was used to create all the samples and

demonstrate the design idea in this study. 316L stainless steel powder with particle size ranging from 15 to  $53~{\mu\mathrm{m}}$  was subjected to PBF fabrication. The chemical composition of the 316L stainless steel powder used in this study, as shown in Table 2, was based on the inspection


Table 2 Chemical composition of 316L stainless steel (wt.%)


<table><tr><td>Element</td><td>Fe</td><td>Cr</td><td>Ni</td><td>Mo</td><td>Mn</td><td>Si</td><td>P</td><td>S</td><td>C</td><td>O</td></tr><tr><td>Tested</td><td>bal</td><td>17.31</td><td>11.31</td><td>2.66</td><td>1.51</td><td>0.62</td><td>0.011</td><td>0.007</td><td>0.011</td><td>0.056</td></tr></table>

report provided by the supplier. To relieve the accumulated stresses during the laser forming process, the specimens were immediately subjected to heat treatment for annealing after the additive manufacturing process was completed. The printed samples were shown in Fig. 1f. To obtain the material properties required for the numerical simulation, the standard flat specimens for tensile testing were designed according to the ASTM E8/E8M [43]. Three standard tensile specimens were prepared using the same batch as the lattice cylindrical tubes. The fabricated tensile specimens and their geometric dimensions were shown in Fig. A1 (in the supplementary information).

A scanning optical microscope (Keyence VHX-6000, Keyence, Japan) was used to characterize the morphology and microstructural features of each lattice sample. A measured strut diameter was  $822.66\mu \mathrm{m}$ , with a standard deviation of  $83.5\mu \mathrm{m}$ . Additionally, images in Fig. 1g indicated the geometric flaws produced during the PBF process. For example, surface beads attributed by partially melted metal particles, strut waviness, strut thickness variation, strut oversizing or undersizing were all termed as printing defects [44].

# 2.3. Mechanical testing

All lattice cylindrical tube samples were subjected to quasi-static compression testing using a universal materials testing machine (Instron 8801, Instron Corp., USA) at a cross-head strain rate of  $10^{-3} / \mathrm{s}$ . Preloading  $(500\mathrm{N})$  was applied to all samples before the current quasi-static compression experiment in order to ensure appropriate contact. After the preloading was completed, displacement was reset to zero while keeping the load unchanged. To establish the repeatability of our experimental findings, at least two tests were employed on each set of samples. Furthermore, to facilitate comprehensive analysis in subsequent investigations, videos were recorded during the compression tests (Canon EOS 80D, Canon, Japan).

# 2.4. Numerical simulation

The numerical simulation was conducted using the explicit dynamic finite element analysis (FEA) method (Abaqus, Dassault Systemes, France) to investigate the influence of various geometric parameters on the performance of lattice cylindrical structures subjected to compressive loading. The geometric models of the DPLCTs were built up in CATIA (CATIA, Dassault Systemes, France) and then imported into Abaqus in the IGES (Initial Graphics Exchange Specification) file format.

The material properties used in the numerical simulations follow the properties obtained from uniaxial tensile tests. In order to describe the material's properties more accurately, the variation of the cross-sectional area of the samples during loading was considered. Therefore, true stress versus true strain was used to define the material's constitutive relationship in simulation. The relationship of true stress  $(\sigma_{\mathrm{true}})$  / strain  $(\varepsilon_{\mathrm{true}})$  with tested engineering stress / strain was as followed:

$$
\sigma_ {\text {t r u e}} = \sigma (1 + \varepsilon) \tag {1}
$$

$$
\varepsilon_ {\text {t r u e}} = \ln (1 + \varepsilon) \tag {2}
$$

where  $\sigma$  and  $\varepsilon$  respectively denoted as engineering stress and engineering strain. The true stress-strain curve of the material was calculated and then shown in Fig. A1 of the supplementary information. The Young's modulus, Poisson's ratio and density of the material were 75.32 GPa, 0.3 and  $7.7~\mathrm{g / cm^3}$ , respectively. The material followed the

isotropic hardening law in the plastic stage, with the stress versus plastic strain data summarized in Table A1 of the supplementary information.

In order to approximate the quasi-static compression, the reference point for one of the two parallel platens was given an encastre boundary condition, and the loading plate was given a downward displacement. In finite element simulations, a faster loading rate than that employed in experimental tests was utilized to reduce computational costs. Throughout the entire compression process in the simulation, the kinetic energy remained below  $5\%$  of the total internal energy and thus could be reasonably considered as quasi-static. The lattice materials were meshed with beam element B31 with the mesh size of  $2\mathrm{mm}$ , while the compression plates were meshed with shell element R3D4 with the mesh size of  $2\mathrm{mm}$ . The contact interaction was set to be general contact in Abaqus/Explicit. Hard contact was applied to avoid penetration, and a penalty algorithm with a 0.3 friction coefficient was used to describe the tangential behavior. As shown in the supplementary information, the simulation results fitted the experimental results well.

# 3. Results and discussion

# 3.1. Compressive responses

The compressive engineering stress-strain curve of dual-phase cylindrical tubular lattices and their corresponding deformation history were shown in Fig. 2. Generally, the compressive response of dual-phase lattice cylindrical tubes included three stages: MP dominated deformation (Stage I), RP dominated deformation (Stage II) and densification (Stage III), which was similar to those observed in bulk lattice materials [26]. In Stage I, the stress initially increased linearly until reaching a peak followed by a stress plateau stage. The plateau region was featured by different types of stress fluctuations accompanying with truss plastic buckling that formed macroscopic localized shear bands (indicated by the red lines) in the matrix phase (MP). Meanwhile, the reinforcement phase grains (RP), for those connected in a diagonal manner, were observed rotating around the connection nodes. In Stage II, after the full compression of weaker MP, the reinforcement phase became the main deformation part, inducing further stress increase prior to final densification. However, with different reinforcement grain patterns, the deformation mode and stress level after the peak in Stage I were different. For bioinspired sinusoidal-helicoidal RP patterns, comparing DPLCT-1 (Fig. 2a and g) with DPLCT-2 (Fig. 2b and h), the only little difference was that shear bands occurred depending on their specific patterns.

As the helicoidal angle varied, forming DPLCT-3 with a helicoidal angle  $(\varphi)$  of  $90^{\circ}$ , RP rotation was not observed, but instead significant truss twisting near RP connection nodes occurred, while interconnected RP grains deformed with MP (Fig. 2c and i). This phenomenon was known as phase boundary slip [26], while RP and MP combined squeezed contributing to strain hardening (indicated by the green region). Also, stress decreased by  $\sim 36\%$  after the first peak, while MP collapsed forming a whole circumferential shear band ring, attributed to a non-connected RP arrangement from the top to the bottom of the tube.

For DPLCT-4, the phase boundary slip phenomenon was even more obvious without RP rotation (Fig. 2j), but the compressive responses exhibited a relatively long plateau area without obvious stress fluctuation (Fig. 2d). In addition to truss yielding and plastic deformation as observed, trusses near RP connection nodes twisted more severely in DPLCT-4; this led to enhanced plastic deformation that occurred with the interacted reinforcement grains sliding along the phase boundaries. Before MP was fully compressed to densification, RP was already

![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/8c4cf530f7c4f3ebe5cdcfba01b9c4884298041c0a7b2d71e2064a069803cbd4.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/7a7699cbcb464d3595440ac313e13fc41acd3820b1b8a41180af09044a53cadb.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/2ac00f8d6abec2c13f2e12f60a880c178c0d76152dc59dea1773a9d1452accf0.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/7259fab837593ace4f3ce187de424bf89090a4071496f0f8b01b997aaf186d9a.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/61cac659df9771217ca701f987eddc25b005d48f9df122f1591c351ab1d5946d.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/9630aaf01378d00281f86e6ea0592396ac8761271fb9b8a9889cfabb0ea7198a.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/740e3e720aeeb893fdb6797294e1aa4fd7743eedfc80da06d9b3b55ebee0d4e3.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/69ac4a3819349eda45c7942098ede9d41cb5da5ea5c13776af743955de7f50da.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/7f39da76abce5c350611b2c7fcec0c7cc9741ed4f39223d42bf4a06cfe872d76.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/0f88474afa1a5f7fabfcc1cc785ae999b0d2f837009ddf643f16357c051bf27b.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/e8fb959c39e8b9ddfb6444c4dd5a2926d285c7ed51176bb1dff8910df8d324ff.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/657756629c86911ef6e2f740665650954e2236938d99c3b7f69217daea68f895.jpg)



Fig. 2. Compressive stress-strain curves, energy efficiency and deformation modes (localized shear bands indicated in red): (a, g) DPLCT-1, (b, h) DPLCT-2, (c, i) DPLCT-3, (d, j) DPLCT-4, (e, k) DPLCT-5 and (f, l) constituent single-phase lattice cylindrical tubes (SPLCTs).


involved in the squeeze with MP, creating a distinct strain-hardening stage (indicated by the green region). From previous publications [26], it was understood that the area of the phase-boundary slip area could be determined in terms of the contacting area between the blocks of matrix phase and reinforcement phase in the compression direction. However, DPLCT-4 with a larger amplitude-to-width ratio  $(\gamma = 2)$  but the same contacting area, possessing a continuous phase boundary in the compression direction, was found helpful in enhancing phase-boundary slip and energy absorption.

The phase boundary slip of DPLCT-5 was not significant, while RP rotation dominated deformation was observed (Fig. 2e and k). Here, RP grains were all connected in a diagonal type into multiple strips, and multiple inclined macroscopic shear bands were formed in the matrix phase during compression, accompanied by a slight rotation of RPs. The compressive stress continued to increase as further compressed.

Overall, two typical compressive responses were observed: one included the strain hardening period associated with phase boundary slip during MP dominated Stage I, while the other did not. Different from our previous study, RP rotation was newly observed. In another word,

despite the fact that reinforcement grains were interconnected and phase boundaries existed, phase boundary slip was not the only deformation mechanism in this work.

To understand the advantage of dual-phase lattice cylindrical tubes, compressive responses of single-phase ones were also carried out, as shown in Fig. 2f. The resulting curves of two single-phase lattice cylindrical tubes (SPLCTs) exhibited as the typical mode of elastic-plastic foams that Gibson and Ashby indicated [11]. Macroscopic shear bands occurred beyond the first stress peak, accompanied with localized plastic buckling of the trusses. Unlike DPLCTs, where shear bands were controlled by RP arrangements, the shear localization bands in SPLCTs occurred randomly in the four different repeated tests (Fig. 2l). No strain hardening behavior was observed here.

# 3.2. Mechanical properties

# 3.2.1. Compressive stiffness and strength

The compressive stress-strain curves for five DPLCTs were compared as shown in Fig. 3a. Within the elastic portion of experimentally

![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/413ea284b19904dea48c5abc6c152b4fb4536d4a79db29f964eb69d9df86f619.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/d6c32a95d0d490feff651c8aee125d46e0d0126f3038ede005e31769e4deb327.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/144af0832d624f7d19258d2f8579d42e880eeccfc50075e6e9fa4e95f03ad266.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/f3a72e2c7681dbfa171b48250219f718147fb18b49898625f0fa39f191ff9ee5.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/04175062323dbd7bbfa93e3988f96a476a494af9138c18371393a2efc5cacb7b.jpg)



Fig. 3. Mechanical properties of lattice cylindrical tubes: (a) Stress-strain curve comparison for five DPLCTs; (b) Specific stiffness, strength and energy absorption (SEA) of DPLCTs versus SPLCTs; (c) Two typical compressive responses: RP rotation without strain hardening and phase boundary slip with strain hardening in MP deformation dominated stage I; (d) Two main interaction deformation mechanisms: "phase boundary slip" and "RP rotation".


obtained stress-strain curves, the slope of the line between  $\sim 25\%$  and  $\sim 60\%$  strength values were used as the experimental stiffness values for comparison. The tested mechanical properties based on the average results of at least two experiments were summarized in Table 3. Note that all five DPLCT samples were designed with almost the same mass, while the tested mass differences were within  $5.5\%$ .

With regards to compressive strength, the experimental values of DPLCT-4, DPLCT-5, DPLCT-1, DPLCT-2, and DPLCT-3 were, respectively,  $\sim 45\%$ ,  $38\%$ ,  $35\%$ ,  $32\%$  and  $19\%$  larger than those of matrix phase SPLCTs; meanwhile, for compressive stiffness, the experimental values of DPLCT-4, DPLCT-5, DPLCT-3, DPLCT-1, and DPLCT-2 were, respectively,  $\sim 48\%$ ,  $45\%$ ,  $37\%$ ,  $37\%$  and  $35\%$  larger than those of the matrix phase SPLCTs. Obviously, DPLCT-4 performed the best. The amplitude-to-width ratio ( $\gamma =$  amplitude/width) of DPLCT-4 was 2, while it was 1 for the others. Accordingly,  $\gamma$  probably played an important role in enhancing compressive stiffness and strength values. Also, results for DPLCT-3 indicated that a non-connected RP arrangement design from the top to the bottom might have decreased performance.

Additionally, the specific stiffness and strength values for five types

of DPLCTs were also analyzed and compared with single-phase tubes (Fig. 3b); these specific values of DPLCTs were generally less than those of SPLCTs. However, the specific stiffness and strength values of DPLCT-4 outperformed MP lattice tubes.

# 3.2.2. Energy absorption

Energy absorption (EA) was obtained from the area under the force-displacement curve as the following Eqs. (3) [45],

$$
E A = \int_ {0} ^ {h _ {D}} F (x) d x \tag {3}
$$

where  $\varepsilon_{D} = h_{D} / H$  is the densification strain. Specific energy absorption (SEA) [46,47] is the energy dissipated energy absorption divided by structural mass  $m$ , given by  $SEA = EA / m$ . The efficiency parameter of energy absorption was proposed to calculate the densification strain and was defined as the absorbed energy per unit volume up to a given nominal strain divided by the corresponding stress value and given by

$$
\mu = \frac {\int_ {0} ^ {\varepsilon} \sigma (\varepsilon) d \varepsilon}{\sigma (\varepsilon)} \tag {4}
$$


Table 3 Mechanical properties of all types of lattice cylindrical tubes.


<table><tr><td>Lattice type</td><td>Relative density ( % )</td><td>Mass ( g )</td><td>Strength ( MPa )</td><td>Specific strength (MPa/ (g·cm-3))</td><td>Stiffness (MPa)</td><td>Specific stiffness (MPa/ (g·cm-3))</td><td>Densification strain</td><td>EA (J)</td><td>SEA (J /g)</td></tr><tr><td>MP</td><td>12.84</td><td>20.50</td><td>17.59</td><td>16.19</td><td>1580.30</td><td>1458.18</td><td>0.52</td><td>154.57</td><td>7.54</td></tr><tr><td>SPLCT</td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td><td></td></tr><tr><td>RP SPLCT</td><td>24.60</td><td>39.75</td><td>52.00</td><td>24.68</td><td>3258.79</td><td>1546.86</td><td>0.47</td><td>457.52</td><td>11.51</td></tr><tr><td>DPLCT-4</td><td>17.61</td><td>27.93</td><td>25.49</td><td>17.22</td><td>2341.73</td><td>1582.33</td><td>0.62</td><td>367.00</td><td>13.14</td></tr><tr><td>DPLCT-1</td><td>17.94</td><td>28.40</td><td>23.83</td><td>15.84</td><td>2160.65</td><td>1436.01</td><td>0.61</td><td>351.88</td><td>12.39</td></tr><tr><td>DPLCT-2</td><td>18.01</td><td>28.70</td><td>23.28</td><td>15.31</td><td>2131.63</td><td>1401.62</td><td>0.61</td><td>347.84</td><td>12.12</td></tr><tr><td>DPLCT-5</td><td>18.29</td><td>29.43</td><td>24.21</td><td>15.52</td><td>2286.95</td><td>1466.38</td><td>0.57</td><td>352.57</td><td>11.98</td></tr><tr><td>DPLCT-3</td><td>18.08</td><td>29.27</td><td>20.94</td><td>13.50</td><td>2170.54</td><td>1399.16</td><td>0.57</td><td>341.00</td><td>11.65</td></tr></table>

In the literature [48],  $\varepsilon_{D}$  was usually determined by the deflection point on the  $\mu -\varepsilon$  curve, as

$$
\left. \frac {d \mu}{d \varepsilon} \right| _ {\varepsilon = \varepsilon_ {D}} = 0 \tag {5}
$$

However, it was difficult to accurately determine  $\varepsilon_{D}$  for the dual-phase lattice due to the existence of the second plateau in the stress-strain curve, which was caused by the crushing of the second-phase region [26]. Hence, we took advantage of the following guidelines to determine the densification strain  $\varepsilon_{D}$  for calculating the energy absorption of multi-phase lattices. The densification point was selected as the last peak on the  $\mu -\varepsilon$  curve, or if there were plateau regions around the peaks or no obvious peaks, it was determined from the obvious drop on the  $\mu -\varepsilon$  curve [49]. The energy efficiency-strain curves  $(\mu -\varepsilon)$  for each DPLCT and SPLCT were plotted in Fig. 2a-f, respectively.

The SEA of all DPLCTs, as shown in Fig. 3b, was generally greater than that of the constituent MP and RP SPLCTs. DPLCT-4 possessed the greatest specific energy absorption capability, which was respectively  $74\%$  and  $14\%$  higher than those of MP and RP SPLCTs. Combining with the excellent specific stiffness and strength properties, DPLCT-4 was thus regarded as the best design in this study, which was again attributed to its higher  $\gamma$ . Meanwhile, DPLCT-3 exhibited the lowest specific energy absorption among the five DPLCTs, indicating the importance of connected RP from the top to the bottom.

Note that either higher plateau stress level or postponed densification strain  $\varepsilon_{D}$  would deduce enhanced specific energy absorption capability of DPLCTs. Because the mechanical properties of MP and RP were different, displacement inconsistency would occur during the phase interaction period. In DPLCT-1, DPLCT-2 and DPLCT-5, RP grains rotated and trusses twisted near the phase boundaries, while in DPLCT-3 and DPLCT-4, the connected RP grains moved along the phase boundary and squeezed together with MP. Generally, two deformation mechanisms were observed as "RP rotation dominated" and "phase boundary slip dominated" as shown in Fig. 3c, d. In the former one, displacement inconsistency deduced truss twisting near the connection node and RP rotation occurred; while in the "phase boundary slip dominated" mechanism, the connection node rotated instead of RP, and meanwhile, RP squeezed before MP densified. RP rotation or node rotation would both prolong deformation time and delay the densification strain. Besides, the RP squeeze during the interaction period would increase the stress level. Accordingly, "phase boundary slip dominated" mechanism would be more beneficial to the enhancement of the energy absorption capability of DPLCTs.

Moreover, as shown in Ashby chart (Fig. 4), SEA versus relative

density of lattice cylindrical tubes here was compared with those of the previously well-documented lightweight lattice metamaterials, similarly fabricated by additive manufacturing using 316L stainless steel powder. These lattice metamaterials included the family of truss-lattices (such as stretching-dominated octet truss-based lattices [3], bending-dominated rhombic dodecahedron (RD) truss-based lattices [50], and octet-RD hybrid truss-based lattices [51]), hollow truss-based lattice [52], shell-based lattices [53], and plate-based lattices [54].

# 3.3. Effects of grain refinement of RP

The simulated compressive stress-strain responses were shown in Fig. 5a and were compared with the tested ones (More types of samples were also simulated and validated by experimental results as shown in Fig. B1). Generally, the simulated curves and typical deformation mode agreed well with those measured; however, in the post-yield regime, a certain quantitative deviation between computed and experimentally measured stress occurred because simulations could not consider effects such as physical contact of lattice members. Despite this, the simulated stiffness and strength values had, respectively, about  $7\%$  and  $6\%$  discrepancies compared with the tested ones (see Table B1 of the supplementary information), indicating that the simulation models here were satisfactory to examine the effects of other various structural designs on stiffness, strength, and deformation modes.

Effects of grain refinement for RP were investigated and DPLCTs with six different RP dispersion patterns were simulated (Fig. 5b) by changing RP grain size  $(k^{*}k^{\prime})$  with the constant overall volume fraction in the circumferential and longitudinal directions. The simulated compressive curves and typical deformation modes were shown in Fig. 5c and d. Phase-boundary slip was observed with localized shear bands occurring around RP (Fig. 5d). The strength values of DPLCTs increased respectively by  $40.36\%$ $53.84\%$  and  $85.5\%$  as the grain size in circumferential direction  $k$  decreased from 3 to 1 (while  $k^{\prime}$  remains at 3) compared with that of MP SPLCTs. However, as the RP grain size in the longitudinal direction  $k^{\prime}$  decreased (from 3 to 1, for example), the stiffness decreased unexpectedly. The greatest strength and stiffness values were obtained by using a reinforcement phase arrangement pattern in which RPs in the same column were vertically connected with the maximum  $k^{\prime}$  while RPs in different columns were connected in an inclined manner with the minimum  $k$ .

# 3.4. Effects of amplitude-to-width ratio  $\gamma$

Four corrugation patterns with different amplitude-to-width ratios

![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/87cd582e6ea30c9fe183b5b5a28e20a4ba2ac2e05f3f49044cfd79bd83fe6b3f.jpg)


# The present study:

★ DPLCT

SPLCT

# Truss-lattices [3, 50, 51]:

Octet truss-lattices

$\times$  RD truss-lattices

Octet-RD hybrid truss-lattices

# Hollow truss-lattices [52]:

BCC hollow truss-lattices

Octet hollow truss-lattices

# Shell-lattices [53]:

SC TPMS lattices

BCC TPMS lattices

FCC TPMS lattices

# Plate-lattices [54]:

Isotropic plate-lattices


Fig. 4. Ashby chart comparing the specific energy absorption of the lattice cylindrical tubes with other lattice metamaterials.


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/72368f66fa28247679fb13ad5ce9c663f8bd352ffed29ffb4171303ff15e7483.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/3e1e0a83111719e0c7f35c91feb4c2b26e6d01796e9a57f74ecf888faa2736f9.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/4411d64ee365f9235805e3d19d6d4cde3b6cbf84013aaaa29f5890d098b8a158.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/c30c713f6ac89d9ed7c1fa69e84c6f7158cdc9d0d885291a0d0c69157acb1291.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/4021d4ed5e06723bd78962121f510fe506a7d2828c98ef096298a1994dce34b5.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/2388d13a12adf8ae58e340dd2a167ce6ec0af9127864e8c20f66c31871af06a2.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/a45619ab1d920f7a8793c6d431b14769ed3f4c7245960ca042886ee5c64d1350.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/4b15b54a19b6d0bf94512d8ee47a73516b2aea84b03562fecc78ced85d509f19.jpg)


![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/6b1e5de618083a1b4319e0ac1a5bfb90004da8d283e39a6e3a9ea720432dccb0.jpg)



Fig. 5. Effects of grain refinement and amplitude-to-width ratio of RP corrugations on mechanical properties of DPLCTs: (a) simulated models validated by experimental results; cylindrical expansion diagrams, compressive stress-strain curves, and deformation modes for: (b-d) six DPLCTs with different RP grain size ( $k^* k$ ) and (e-g) four DPLCTs with different amplitude-to-width ratios ( $\gamma$ ) of RP corrugations. Note that  $k$  and  $k'$  are RP grain sizes respectively in the circumferential and longitudinal directions.


$(\gamma = 4,2,1,0.5)$  were designed by keeping the constant overall volume fraction in the circumferential and longitudinal directions (Fig. 5e). The simulated compressive stress-strain curves were shown in Fig. 5f, and the stiffness and strength values increased slightly with  $\gamma$ . Also, the interaction deformation mechanisms between MP and RP in the DPLCTs were different, as shown in Fig. 5g. Phase boundary slip dominated deformation mechanism was observed for DPLCTs with  $\gamma = 4$  and  $\gamma = 2$ , while RP rotation dominated mechanism was observed for DPLCTs with  $\gamma = 1$  and  $\gamma = 0.5$ . Accordingly, the interaction deformation mechanism between RP and MP could be controlled and even predicted by the arrangement pattern of RPs, as illustrated in Fig. 6.

According to previous experimental results, to avoid a large drop

after the stress peak, RP grains should keep connected to each other from top to bottom (Fig. 2c). Whether RP grains were diagonally connected with two connection nodes was detected as an important issue:

(1) If RPs were diagonally connected with only two connection nodes, the interaction deformation mechanism between RP and MP varied depending on amplitude-to-width ratio  $\gamma$ . For  $\gamma \geq 2$ , phase boundary slip dominated deformation occurred; as for  $\gamma \leq 1$ , RP rotation dominated deformation was observed.

(2) If RP were connected in other patterns (e.g., with more connection nodes), phase boundary slip dominated deformation would occur.

![](file://D:/MinerU/转换结果/151.pdf-0b14eb3f-55d8-4304-840f-fe18a778139c/images/684a888886852bcbde37f0448eefb0548daacafd5071323fb8085dae17fa551d.jpg)



Fig. 6. Design principles for RP patterns of DPLCTs with different interaction deformation mechanism between two phases.


# 4. Conclusion

Bioinspired dual-phase lattice cylindrical tubes (DPLCTs) were designed to enhance specific energy absorption (SEA) by tailoring the reinforcement phases (RP) arrangement. The tubes were designed using a mapping method and fabricated by additive manufacturing, followed by quasi-static compression tests. After the introduction of RP, DPLCTs exhibited greater SEA than single-phase lattice cylindrical tubes (SPLCTs). Numerical simulations were used to discuss the typical geometrical parameters. Then, the design guidance for lattice cylindrical tubes with greater energy absorption capability was summarized. The main conclusions include:



(1) SEA of all DPLCTs was generally greater than those of the constituent matrix phase (MP) and RP based cylindrical tubes. DPLCT-4 with higher amplitude-to-width  $\gamma$  exhibited the "phase boundary slip dominated" deformation mechanism between MP and RP, possessing the greatest specific absorption energy capability, which was respectively  $74\%$  and  $14\%$  greater than those of MP and RP based single-phase cylindrical tubes. Also, DPLCT-4 exhibited the greatest specific strength and stiffness values among all DPLCTs.





(2) Besides the "phase boundary slip dominated" mechanism, a "RP rotation dominated" deformation mechanism was newly found in this study, which could delay the densification strain. However, the "phase boundary slip dominated" mechanism could both increase the stress level and delay the densification strain, which was more beneficial to the energy absorption capability enhancement of DPLCTs.





(3) The interaction deformation mechanism between RP and MP could be controlled and predicted by RP patterning. The designing principles of dual-phase metamaterials with excellent specific energy absorption included:





(i) RP grains should be connected from the top to the bottom;





(ii) RP should be strongly connected to ensure phase boundary slip occurred by uncoordinated deformation between MP and RP; if RP was connected with only two diagonal nodes, the deformation mechanism would depend on the  $\gamma$ .



# CRediT authorship contribution statement

Yuan Tian: Writing - original draft, Validation, Methodology, Investigation, Formal analysis. Huitian Wang: Visualization, Software, Methodology. Zhuo Chen: Software, Formal analysis. Qianqian Wu: Methodology, Funding acquisition. Sha Yin: Writing - review & editing, Supervision, Resources, Methodology, Funding acquisition, Conceptualization.

# Declaration of competing interest

The authors declare that they have no known competing financial interests or personal relationships that could have appeared to influence the work reported in this paper.

# Acknowledgments

This research is supported by Natural Science Foundation of China (Nos. 12172025, 12322204), National Key Research and Development Program of China (2023YFB2504600), Science Foundation of National Key Laboratory of Science and Technology on Advanced Composites in Special Environments (No.6142905222707).

# Appendix A. Supplementary data

Supplementary data to this article can be found online at https://doi.org/10.1016/j.compstruct.2025.119015.

# Data availability

Data will be made available on request.

# References



[1] Yin H, Zhang W, Zhu L, Meng F, Liu J, Wen G. Review on lattice structures for energy absorption properties. Compos Struct 2023;304:116397.





[2] Ding J, Ma Q, Li X, Zhang L, Yang H, Qu S, et al. Imperfection-enabled strengthening of ultra-lightweight lattice materials. Adv Sci 2024;11:2402727.





[3] Tancogne-Dejean T, Spierings AB, Mohr D. Additively-manufactured metallic micro-lattice materials for high specific energy absorption under static and dynamic loading. Acta Mater 2016;116:14-28.





[4] Andrew JJ, Schneider J, Ubaid J, Velmurugan R, Gupta NK, Kumar S. Energy absorption characteristics of additively manufactured plate-lattices under low-velocity impact loading. Int J Impact Eng 2021;149:103768.





[5] Zeng Z, Gao S, Pokkalla DK, Zhang S, Han C, Liu F, et al. Additive manufacturing of metallic metamaterials with enhanced mechanical properties enabled by microstructural and structural design. Int J Mach Tool Manu 2024;199:104172.





[6] Miralbes R, Ranz D, Pascual FJ, Zouzias D, Maza M. Characterization of additively manufactured triply periodic minimal surface structures under compressive loading. Mech Adv Mater Struct 2022;29:1841-55.





[7] Arsentev M, Topalov E, Balabanov S, Sysoev E, Shulga I, Akhmatnabiev M, Sychov M, Skorb E, Nosonovsky M. Crystal-inspired cellular metamaterials and triply periodic minimal surfaces. Biomimetics (Basel, Switzerland) 2024;9.





[8] Evans AG, He MY, Deshpande VS, Hutchinson JW, Jacobsen AJ, Carter WB. Concepts for enhanced energy absorption using hollow micro-lattices. Int J Impact Eng 2010;37:947-59.





[9] Zhang W, Yin S, Yu TX, Xu J. Crushing resistance and energy absorption of pomelo peel inspired hierarchical honeycomb. Int J Impact Eng 2019;125:163-72.





[10] Yin S, Chen H, Li J, Yu TX, Xu J. Effects of architecture level on mechanical properties of hierarchical lattice materials. Int J Mech Sci 2019;157-158:282-92.





[11] Maskery I, Aboulkhair NT, Aremu AO, Tuck CJ, Ashcroft IA, Wildman RD, et al. A mechanical property evaluation of graded density Al-Si10-Mg lattice structures manufactured by selective laser melting. Mater Sci Eng A 2016;670:264-74.





[12] Qiu N, Zhang J, Li C, Shen Y, Fang J. Mechanical properties of three-dimensional functionally graded triply periodic minimum surface structures. Int J Mech Sci 2023;246:108118.





[13] Wang C, Wang W, Zhao W, Wang Y, Zhou G. Structure design and multi-objective optimization of a novel NPR bumper system. Compos B Eng 2018;153:78-96.





[14] Li Y, You Z. Open-section origami beams for energy absorption. Int J Mech Sci 2019;157-158:741-57.





[15] Liu Q, Shen H, Wu Y, Xia Z, Fang J, Li Q. Crash responses under multiple impacts and residual properties of CFRP and aluminum tubes. Compos Struct 2018;194: 87-103.





[16] Zhang H, Wu Y, Wang K, Peng Y, Wang D, Yao S, et al. Materials selection of 3D-printed continuous carbon fiber reinforced composites considering multiple criteria. Mater Des 2020;196:109140.





[17] Ma J, Chai S, Chen Y. Geometric design, deformation mode, and energy absorption of patterned thin-walled structures. Mech Mater 2022;168:104269.





[18] Nurick GN, Langdon GS, Chi Y, Jacob N. Behaviour of sandwich panels subjected to intense air blast - Part 1: experiments. Compos Struct 2009;91:433-41.





[19] Fang H, Mao Y, Liu W, Zhu L, Zhang B. Manufacturing and evaluation of Large-scale Composite Bumper System for bridge pier protection against ship collision. Compos Struct 2016;158:187-98.





[20] Pham M-S, Liu C, Todd I, Lertthanasarn J. Damage-tolerant architected materials inspired by crystal microstructure. Nature 2019;565:305-11.





[21] Gu GX, Takaffoli M, Buehler MJ. Hierarchically enhanced impact resistance of bioinspired composites. Adv Mater 2017;29:1700060.





[22] A. A J, A. S. Studies on effect of failure modes on mechanical properties of staggered composites. Bioinspir Biomim 2024;19:036019.





[23] Wu G, Chan K-C, Zhu L, Sun L, Lu J. Dual-phase nanostructuring as a route to high-strength magnesium alloys. Nature 2017;545:80-3.





[24] Jin S, Ngai T, Zhang G, Zhai T, Jia S, Li L. Precipitation strengthening mechanisms during natural ageing and subsequent artificial aging in an Al-Mg-Si-Cu alloy. Mater Sci Eng A 2018;724:53-9.





[25] Guo W, Huang Y, Ritchie RO, Yin S. Dissipative dual-phase mechanical metamaterial composites via architectural design. Extreme Mech Lett 2021;48.





[26] Yin S, Guo W, Wang H, Huang Y, Yang R, Hu Z, et al. Strong and tough bioinspired additive-manufactured dual-phase mechanical metamaterial composites. J Mech Phys Solids 2021;149.





[27] Banait S, Liu C, Campos M, Pham MS, Pérez-Prado MT. Effect of microstructure on the effectiveness of hybridization on additively manufactured Inconel718 lattices. Mater Des 2023;236:112484.





[28] Tian Y, Zhang X, Hou B, Jarlov A, Du C, Zhou K. Programmable heterogeneous lamellar lattice architecture for dual mechanical protection. Proc Natl Acad Sci 2024;121:e2407362121.





[29] Li M, Zhu H, Lai C, Bao W, Han H, Lin R, et al. Recent progresses in lightweight carbon fibre reinforced lattice cylindrical shells. Prog Aerosp Sci 2022;135:100860.





[30] Lee W, Jeong Y, Yoo J, Huh H, Park S-J, Park SH, et al. Effect of auxetic structures on crash behavior of cylindrical tube. Compos Struct 2019;208:836-46.





[31] Giri TR, Mailen R. Controlled snapping sequence and energy absorption in multistable mechanical metamaterial cylinders. Int J Mech Sci 2021;204.





[32] Yang J, Xiong J, Ma L, Zhang G, Wang X, Wu L. Study on vibration damping of composite sandwich cylindrical shell with pyramidal truss-like cores. Compos Struct 2014;117:362-72.





[33] Xiong J, Ghosh R, Ma L, Vaziri A, Wang Y, Wu L. Sandwich-walled cylindrical shells with lightweight metallic lattice truss cores and carbon fiber-reinforced composite face sheets. Compos A Appl Sci Manuf 2014;56:226-38.





[34] Cao X, Huang Z, He C, Wu W, Xi L, Li Y, et al. In-situ synchrotron X-ray tomography investigation of the imperfect smooth-shell cylinder structure. Compos Struct 2021;267:113926.





[35] Mirhakimi As, Dubey D, Elbestawi MA. Laser powder bed fusion of bio-inspired metamaterials for energy absorption applications: a review. J. Mater. Res. Technol. 2024;31:2126-55.





[36] Ha NS, Lu G. A review of recent research on bio-inspired structures and materials for energy absorption applications. Compos B Eng 2020;181.





[37] Yin S, Yang R, Huang Y, Guo W, Chen D, Zhang W, et al. Toughening mechanism of coelacanth-fish-inspired double-helicoidal composites. Compos Sci Technol 2021; 205.





[38] Yang X, Ma J, Shi Y, Sun Y, Yang J. Crashworthiness investigation of the bioinspired bi-directionally corrugated core sandwich panel under quasi-static crushing load. Mater Des 2017;135:275-90.





[39] Zhao S, Yin X, Zhang D. A study of a bio-inspired impact resistant carbon fiber laminate with a sinusoidal helicoidal structure in the mandibles of trap-jaw ants. Acta Biomater 2023;169:179-91.





[40] Yang R, Wang H, Wang B, Zhang S, Huang Z, Yin S. Sinusoidally architected helicoidal composites inspired by the dactyl club of mantis shrimp. Int J Smart Nano Mater 2023;14:321-36.





[41] Weaver JC, Milliron GW, Miserez A, Evans-Lutterodt K, Herrera S, Gallana I, et al. The stomatopod dactyl club: a formidable damage-tolerant biological hammer. Science 2012;336:1275-80.





[42] Wang Y, Ren X, Chen Z, Jiang Y, Cao X, Fang S, et al. Numerical and experimental studies on compressive behavior of Gyroid lattice cylindrical shells. Mater Des 2020;186.





[43] I.J.W.C. Astm, PA, USA: ASTM International, ASTM E8/E8M-16a: standard test methods for tension testing of metallic materials, 2016.





[44] Liu L, Kamm P, Garcia-Moreno F, Banhart J, Pasini D. Elastic and failure response of imperfect three-dimensional metallic lattices: the role of geometric defects induced by Selective Laser Melting. J Mech Phys Solids 2017;107:160-84.





[45] Kumar AP, Nagarjun J, Ma Q. Potentiallyity of MWCNT fillers on the lateral crashworthiness behaviour of polymer composite cylindrical tubes under quasi-static loading. J Ind Text 2021;51:7014S-33S.





[46] Kumar AP, Maneiiah D. Crashworthiness behaviour of capped cylindrical aluminium tubular structures subjected to lateral compression. Int J Mech Prod Eng Res Devel 2019;9:1167-72.





[47] Kumar AP. Quasi-static crushing behaviour of axially compressed combined aluminium-composite tubes. Int J Mech Eng Technol 2018;9:907-14.





[48] Avalle M, Belingardi G, Montanini R. Characterization of polymeric structural foams under compressive impact loading by means of energy-absorption diagram. Int J Impact Eng 2001;25:455-72.





[49] Bian Y, Wang R, Yang F, Li P, Song Y, Feng J, et al. Mechanical properties of internally hierarchical multiphase lattices inspired by precipitation strengthening mechanisms. ACS Appl Mater Interfaces 2023;15:15928-37.





[50] Cao X, Duan S, Liang J, Wen W, Fang D. Mechanical properties of an improved 3D-printed rhombic dodecahedron stainless steel lattice structure of variable cross section. Int J Mech Sci 2018;145:53-63.





[51] Xiao L, Xu X, Feng G, Li S, Song W, Jiang Z. Compressive performance and energy absorption of additively manufactured metallic hybrid lattice structures. Int J Mech Sci 2022;219:107093.





[52] Xiao L, Feng G, Li S, Mu K, Qin Q, Song W. Mechanical characterization of additively-manufactured metallic lattice structures with hollow struts under static and dynamic loadings. Int J Impact Eng 2022;169:104333.





[53] Bonatti C, Mohr D. Smooth-shell metamaterials of cubic symmetry: anisotropic elasticity, yield strength and specific energy absorption. Acta Mater 2019;164: 301-21.





[54] Duan S, Wen W, Fang D. Additively-manufactured anisotropic and isotropic 3D plate-lattice materials for enhanced mechanical performance: simulations & experiments. Acta Mater 2020;199:397-412.

