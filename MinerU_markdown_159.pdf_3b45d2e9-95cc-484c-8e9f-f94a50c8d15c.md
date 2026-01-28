# Functionally graded lattice structures for energy absorption: Numerical analysis and experimental validation

![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/a92d4142acf33e1dc5b12f2f6a71c5ab3aee9a9c2689ce9d19b6ab667fe9bfe2.jpg)


Antonio Coluccia<sup>a, *</sup>, Guillaume Meyer<sup>b,c</sup>, Stefania Liseni<sup>a</sup>, Christian Mittelstedt<sup>b,c</sup>, Giorgio De Pasquale<sup>a</sup>

a Smart Structures and Systems Lab, Department of Mechanical and Aerospace Engineering, Politecnico di Torino, Corso Duca degli Abruzzi 24, Torino, Italy

b Lightweight Engineering and Structural Mechanics, Department of Mechanical Engineering, Technical University of Darmstadt, Darmstadt, Germany

cAdditive Manufacturing Center, Technical University of Darmstadt, Darmstadt, Germany

# ARTICLEINFO

# Keywords:

Lattice structures

Energy absorption

Lightweight structures

Additive manufacturing

Numerical modeling

Cellular materials

# ABSTRACT

Lattice structures show a high potential in fields where high structural performances are necessary, such as automotive and aerospace engineering. These structures offer excellent stiffness and strength, while being able to keep their weight limited: main outcome of such characteristics are appreciable specific mechanical properties. Since lattice structures are mostly produced using additive manufacturing, a large number of shapes and topologies are available. Moreover, it is possible to control geometrical features, like thickness of the struts, eventual reinforcements and in general the local relative density of the structure, through mathematical and analytical considerations. The principal aim of the model developed in this paper is the control over the thickness of the struts of a lattice structure: samples made of lattice with different topologies are object to a functionally grading process able to redefine the thickness of each strut of the sample based on homogenizing the stress state; as a main result, energy absorption and specific energy absorption levels are increased. Two grading processes are presented: the first one considers relative density into the relationship for the reformulation of the thickness value, together with an average level of the Von Mises stress, while the second only considers the stresses. A validating experimental campaign has been finally performed: graded samples, with both processes, and ungraded samples are produced via L-PBF (laser powder bed fusion) and tested under compression in order to compare their energy absorption levels.

# 1. Introduction

Over the last decades lattice structures have progressively gained attention in different fields of engineering research. This is due to their excellent mechanical properties [1,2] that, together with their controllable relative density, make lattice structures optimal when it comes to lightweight engineering [3]. Another important feature that makes lattice structure relevant and innovative is the way they are manufactured: classical manufacturing processes have been used as well over the years to create lattices [2,4], but additive manufacturing offers the possibility to generate and design lattice structures according to specific design requirements [5,6]. Given these assumptions, lattices are employed in many different engineering fields. Due to their nature and their variable relative density, these structures can be used and designed as heat exchangers; research is very active in this field, investigating different lattice solution with different fluids [7-9]. Lattices are extremely

functional metamaterials, in fact different aims can be pursued: in [10], these structures are employed as reinforcement in the leading edge of an aircraft wing, where both anti-icing, therefore specific heat flow design requirements, and energy absorption properties, in case of bird-strike or debris impact, are essential. In the aerospace sector they are used for the generation of panels for different purposes: [11] and [12] present investigations over cylindrical lattice panels and cylindrical lattice reinforcement for composite panels. Besides the aeronautical field, the concept of lattices can be found in the space sector as well; repetitive architecture unit panels are investigated in [13] for spacecraft shielding purposes. Also, lattices are largely employed in the design of orthopedic implants [14,15], both for their mechanical properties and their excellent biocompatibility.

The topic of energy absorption in lattices is widely investigated by means of different tools such as computational analyses using the finite element method (FEM). Both the static and the dynamic mechanical response of truss lattice structures under compression from the point of

# Nomenclature

FEM Finite element method

L-PBF Laser powder bed fusion

EA Energy absorption

VEA Volumetric energy absorption

SEA Specific energy absorption

bcc Body centered cubic

fcc Face centered cubic

fbcc Mixed body and face centered cubic

bccz Body centered cubic

$f c z$  Face centered cubic

fbccz Mixed body and face centered cubic

view of energy absorption are studied in [16-21]. More detailed investigations about the behavior of lattices under quasi-static crushing can be found in literature: in [22] energy absorption properties of a bioinspired corrugated lattices made of nylon are studied under the effects of quasi-static compression both using FEM and experimental tests. The process of using FEM, and in general computational analysis, for the simulation of the quasi-static behavior of lattices followed by validating experimental tests is common: in [23] both FEM and tests are employed for an investigation on energy absorption capabilities of polymers-filled steel lattices. The same process is employed for the investigation of both conventional and non-conventional lattice topologies and different materials: bio-inspired corrugated nylon lattices [22], diamond shell lattices object to a mapping method [24], strut-plate lattices inspired by fiber-reinforced composite materials [25], tetrahedral lattices [26], tessellated dual-material bio-inspired lattices improved for energy absorption [27], hybrid rhombic dodecahedron-octet lattices [28] and many different hybrid structures [29-31]. FEM can also be employed for studying the influence of manufacturing defects on the energy absorption properties of lattices [32]. Non-linear dynamic FEM is often used for impact and high speed crushing simulations [33-35], though experimental tests using dropping weight [36] and Hopkinson pressure bar [37] are necessary for an adequate characterization of the lattice materials involved.

The available literature also offers a wide collection of optimization processes for lattice structures inherent to different aspects of the lattice nature: in [38] the optimization process works on the shape of the single cell composing the lattices in order to minimize the relative density and at the same time satisfy the design constraints imposed. In a similar way, anoptimization process based on strut thickening is proposed in [39], yet this kind of process starts working at a more global level than the one of the single cell. Different features of the structure can be addressed by the process at the same time: in [40] the model works both at the macro-scale and the micro-scale level, including the possibility to create hybrid cells together with mathematical fields defining the local relative density of the analyzed structure. Multi-scale optimization processes have also been applied in presence of mixed boundary conditions [41] and together with the employment of non-uniform rational basis spline (NURBS) [42]. Similarly, [43] presents the possibility to both optimize the microstructure of the constituent material addition of specific particles and the general architecture of the structure. More classical optimization processes based on structural grading can be found as well: [44] presents the results of compressive tests performed on bidirectionally graded lattices, while in [45] a grading approach based on the stress is shown. Multi-morphology approaches are also common for lattice structures: in [46] and [47] investigations about the employment of topologically different cells in the same sample in order to enhance energy absorption, and mechanical properties of lattices, are presented. Optimization processes can also address thermal problems, besides purely structural ones, as it can be appreciated in [48]. As it can be seen

in the above-mentioned papers, structural grading and in general topological optimization, also by means of cell combination, play important roles in exploiting the possibilities which lattices offer with respect to mechanical properties, in particular energy absorption. Basically, optimization processes applied on lattices can be based both on using different types of lattice cells in order to obtain multi-morphology structures and on grading aimed at maximizing a specific mechanical property.

In this paper, a structural grading process based on the maximization of energy absorption that leads to a homogenization of the stress state of the considered lattice is presented. The degree of novelty that can be appreciated in this work lies in the fact that it is not simply the mere application of a grading design [49] and it does not consider the employment of different lattice cells (several problems regarding the geometrical connectivity can occur) for the maximization to lead to an energy absorption and stress distribution improvement. The innovative contribution of this work lies in the employment of an ad-hoc procedure aimed at the maximization of energy absorption and the homogenization of lattices, operating in parallel to the FEM model, without using pre-defined embedded optimization tools and based on the behavior of the lattice component when not graded yet. The grading procedure is based on the stress configuration the sample itself is showing when crushed and not on an external stress field imposed by the user, allowing the control of the load path as well. This tool can be used as a pre-sizing approach, allowing an initial dimensioning of the lattice structure involved in the design. For this investigation, the process is applied to samples, but it can be easily extended to lattice components. Material considered for both simulation and production of lattice structures for this study is aluminum alloy AlSi10Mg. At first, static compressive analyses are performed, and the stress configuration of the samples is mapped. Based on the consideration made about the stress distributions, two different grading approaches are proposed, aimed at homogenizing the stress state and redefining the load path inside the samples. The main difference between the two grading approaches is the implicit consideration of the relative density ratio between the final configuration and the initial one. Selected samples are later printed via L-PBF process both in the original configuration and the graded ones, and tested under compression load, as a validation of the computational results.

The paper is structured as it follows: chapter 2 deals with the definition of the model for the grading process and the description of the FEM model; chapter 3 describes the different features of the experimental campaign, including the sample manufacturing and testing; chapter 4 shows the results obtained from the grading process application and the comparison with the results from the experimental campaign, and the relative observation and discussions; conclusions are presented in chapter 5.

# 2. Model

Based on previous investigations [16,50] and available literature [17,35], the lattices selected for this investigation are body centered cubic  $(bcc)$ , body centered cubic with the addition of z-oriented struts  $(bccz)$ , face centered cubic  $(fcc)$ , face centered cubic with the addition of z-oriented struts  $(fccz)$ , mixed body and face centered cubic  $(fbcc)$  and mixed body and face centered cubic with the addition of z-oriented struts  $(fbccz)$ . Such a group of lattices allows the study of how different topological features influence the effects on the energy absorption and mechanical properties. In this case these features are the different orientation of the struts, between  $bcc$  and  $fcc$ , combination of cells and vertical reinforcements through vertical struts. From here on cells with the addition of z-oriented struts at the corner will be referred to as z-reinforced. The representative volume element (RVE) is cubic and presents a fixed edge length of  $3\mathrm{mm}$ . Fig. 1 shows the group of lattices considered.

Energy absorption properties are commonly retrieved through the following expressions [51] using the stress-strain diagrams obtained by

![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/7038e0aec33c1ac8450cc6ea680fe5dbd6b3cbb0da39a5a07f54af1855c24ff8.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/5116e15b22788016f65a36d27762f0bd635d6614c70e0cf69e65c994d0e0a255.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/ef2ed0d2d23ed101cf6b55d78730afa3cf15b80cd920f744d012fd0b4e4cfdca.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/62d99ef6424532af647f4147f2bb42a9a08f2e92f6fbdc2088c16923f1730995.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/3fa5bba7ce8b01ecdaa5994c4bd8a0ffa03738b8e6b867779527fd7c86f5a3a6.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/cda281bb73cc08a4919058d6ba5cdf1995b721805988eb8e28187c210cdd735b.jpg)



Fig. 1. Lattice cells considered, from left to right: bcc, bccz, fcc, fccz, fbcc, fbccz.


the tests:

$$
V E A = \int_ {0} ^ {\varepsilon} \sigma (\varepsilon) d \varepsilon \tag {1}
$$

Therein, VEA is the volumetric energy absorption, while  $\sigma$  and  $\varepsilon$  are the equivalent stress and strain. Through VEA (1), the energy absorption (EA) (2) and the specific energy absorption (SEA) (3) can be obtained:

$$
E A = V E A ^ {*} V \tag {2}
$$

$$
S E A = \frac {E A}{m} \tag {3}
$$

Herein,  $V$  is the volume and  $m$  is the mass of the sample considered.

The first step of the process consists in assessing the stress state of the initial lattice configuration. To achieve this, static compression simulations are performed. The software used is Ansys Workbench, with its embedded static solver. Six homogeneous samples based on the representative unit cells shown in Fig. 1 are considered. The investigated samples consist of  $10 \times 10 \times 10$  unit cells with an initial strut diameter of  $0.37 \mathrm{~mm}$  and a cell size of  $3 \mathrm{~mm}$ . Cell size and initial strut diameter are chosen considering previous investigations made on the topic of energy absorption investigation and impact analysis [16,17,35,50]. The bilinear material model employed in the frame of FEM simulations is issued from a previous work [16]. The material properties are listed in Table 1.

Linear 2-noded beam elements employing the Timoshenko beam theory have been used in the FEM model, With each node presenting 6 degrees of freedom, 3 translational and 3 rotational. Based on a sensitivity analysis, the necessary characteristic length of one element is set to  $1.5\mathrm{mm}$ , resulting in 2 beam elements per strut. The sensitivity analysis conducted has been considering the stress output of fixed regions of the model to define the suitable mesh characteristic dimension. The following loading and boundary conditions are applied (Fig. 2): the bottom surface of the FEM model is rigidly fixed while a  $-2\mathrm{mm}$  displacement is imposed on the top surface, which represents a crushing plate. The displacement range from  $0\mathrm{mm}$  to  $-2\mathrm{mm}$  is divided into 150 equally spaced substeps. In Ansys Workbench, substeps division for nonlinear static analyses allows the generation of force-displacement diagrams, a very useful tool in particular when using a nonlinear material model, as in this case. Number of substeps to be imposed has been defined on the basis of a sensitivity analysis.

Stress-strain curves, necessary for the evaluation of energy absorption properties (1)-(3), are determined from force-displacement curves through:

$$
\sigma = F / a \varepsilon = \delta / L \tag {4}
$$

Therein,  $F$  is the registered force reaction,  $A$  is the horizontal section area of the specimen,  $\delta$  is the displacement of the upper surface and  $L$  is the vertical edge length of the specimen.

![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/4ca9f32a5dd80062cb5162449004c6becd0160d5cbda6c75864b22c22f077499.jpg)



Fig. 2. Graphical representation of the boundary and load conditions applied to the samples for the FEM simulations.


In order to obtain a discrete mapping of the stress distribution, the stresses of each element are extracted. Data extraction and matrix generation, as well as the whole grading process, are performed using a Matlab routine. The equivalent stress  $\sigma_{e}$  comes from the combination of two standard output of Ansys Workbench: the axial stress  $\sigma_{direct}$ , and the maximum bending stress  $\sigma_{bendingMAX}$ . These two contributions are able to keep track of the two main lattice solicitation modes, that are axial and bending, in a single indicator, allowing to generate an equivalent stress parameter that considers the mixed load configuration of the strut. The expression for the definition of  $\sigma_{e,i}$  for a given element  $i$  is:

$$
\sigma_ {e, i} = \left| \sigma_ {\text {d i r e c t}, i} + \sigma_ {\text {b e n d i n g M A X}, i} \right| \tag {5}
$$

The maximum equivalent stress registered in each cell of each sample is extracted from the output files of the analyses in order to generate a  $10 \times 10 \times 10$  matrix containing these maximum stress values. Based on this mapping, the process is developed based on a structural grading by means of strut diameter variation. This process relies on several assumptions. The first hypothesis stipulates that the displacement the ungraded sample is subject to is equal to the one of the graded one, therefore:

$$
\varepsilon = \varepsilon_ {0} \leftrightarrow \delta = \delta_ {0} \tag {6}
$$

Herein,  $\delta_0$  is the displacement of the upper surface of the ungraded sample. The second hypothesis assumes that the force reaction  $F$  for a single cell is proportional to both the maximum equivalent stress  $\sigma_{e}$  registered in the cell and the diameter of the struts  $t$ :

$$
F \propto \sigma_ {e, M A X} t ^ {2} \tag {7}
$$

At that point two grading approaches are developed. The first one es


Table 1 Properties used for the AlSi10Mg bilinear model employed in FEM simulations, where  $\rho$  is density, E is the elastic modulus,  $\nu$  is the Poisson ratio, G is the shear modulus,  $\sigma_U$  is the ultimate stress,  $\sigma_Y$  is the yield stress,  $\varepsilon_U$  is the ultimate strain,  $\varepsilon_Y$  is the yield strain and  $E_{T}$  is the tangential modulus.


<table><tr><td>ρ [g/mm3]</td><td>E [GPa]</td><td>ν</td><td>G [GPa]</td><td>σU [MPa]</td><td>σY [MPa]</td><td>εU</td><td>εY</td><td>ET [MPa]</td></tr><tr><td>0.00268</td><td>75</td><td>0.33</td><td>28.195</td><td>400</td><td>250</td><td>0.07</td><td>σY/E = 0.00333</td><td>σU - σY / (εU - εY) = 2250</td></tr></table>

tabilishes the relationship between force reaction and relative density  $\rho_{R}$  (8) while the second one only considers the force equilibrium for both graded and ungraded samples (9); in expressions (8) and (9) parameters with zero subscript refer to initial ones from the ungraded sample.

$$
\frac {F}{F _ {0}} = \frac {\rho_ {R}}{\rho_ {R 0}} \tag {8}
$$

$$
F = F _ {0} \tag {9}
$$

Therefore, different formulations of the strut diameter are employed.

$$
t _ {1} = \sqrt {\left(\frac {\sigma_ {e , M A X}}{\sigma_ {e T}}\right) \left(\frac {\rho_ {R}}{\rho_ {R 0}}\right) t _ {0} ^ {2}} \tag {10}
$$

$$
t _ {2} = \sqrt {\left(\frac {\sigma_ {e , M A X}}{\sigma_ {e T}}\right) t _ {0} ^ {2}} \tag {11}
$$

Where  $\sigma_{eT}$  is a stress threshold that is explained below, and  $t_0$  is the initial strut diameter.

In frame of the first process, the following relationship between relative density and diameter of the struts is used:

$$
\rho_ {R} = A \left(\frac {t}{\bar {l}}\right) ^ {2} + B \left(\frac {t}{\bar {l}}\right) ^ {3} \tag {12}
$$

Therein,  $l$  is the edge length of the cell, and the relationship between  $t$  and  $l$  is the aspect ratio of the cell relative the diameter.  $A$  and  $B$  are two coefficients that differ for each topology, and which are evaluated through a polynomial fit. Polynomial expression (12) gives the possibility to evaluate the relative density from the thickness over cell edge length ratio, based on the Ashby model [1] for open cells. Coefficients are given in Table 2.

Not all of the strut diameters are changed: only selected cells are subject to the process, and those are chosen according to a threshold. If the maximum equivalent stress of the cell exceeds the threshold, the diameter of the cell can be changed according to (10) or (11). The concept defining a stress threshold that influences the modification of the lattice can also be found in [45]: the difference with the model method presented here works at the scale of the single cell. Three different thresholds are considered, in order to appreciate the potential of the processes at different levels:

- Threshold 1:  $25\%$  of the average maximum stresses registered in each cell. Hardly any maximum stress per cell will exceed the  $25\%$  of the average (this percentage allows though to at least catch border effects and stress peaks in most cases [52]

- Threshold 2: minimum of the maximum stresses registered in each cell. By employing this threshold, basically every cell of the lattice will change its diameter.

- Threshold 3: average of the maximum stresses registered in each cell. The third case represents a kind of middle condition, where there is a proper balance between the mass increase and the improvement of energy absorption properties.

New stress and strain outputs are recalculated for the new lattice configurations. Therefore EA, VEA and SEA of the graded sample can be


Table 2 Coefficients for the definition of the relative density (from [16].


<table><tr><td>Cell</td><td>A</td><td>B</td></tr><tr><td>bcc</td><td>5.4424</td><td>-4.9020</td></tr><tr><td>bccz</td><td>6.2274</td><td>-6.1502</td></tr><tr><td>fcc</td><td>4.4434</td><td>-3.9141</td></tr><tr><td>fccz</td><td>5.2295</td><td>-5.44177</td></tr><tr><td>fbcc</td><td>9.8981</td><td>-12.8319</td></tr><tr><td>fbccz</td><td>10.6694</td><td>-14.3042</td></tr></table>

recalculated via Matlab without performing another time-consuming FEM-analysis. In order to establish the correctness of such results, a final comparison with a FEM model has been performed and results of such comparisons will be shown in the results chapter.

# 3. Experimental tests

In order to validate the process, an experimental testing campaign is performed. Samples showing higher energy absorption (see Table 5 in section 4) and adaptivity to the grading process have been printed and tested under compression load:  $bcc$  and  $bccz$  samples are the considered ones. Such samples are printed in three different cases: the initial one and the graded ones via process 1 and 2. The threshold chosen for the grading of the samples to be printed is threshold 3, since its application results into high energy absorption.

# 3.1. Sample manufacturing

Table 3 shows information about the printed samples and their numeration.

Five specimens for each configuration have been printed, plus one for each initial configuration. The samples listed in Table 3 have been printed at the Lightweight Engineering and Structural Mechanics Institute of the Technical University of Darmstadt, using an EOS M290 L-PBF system processing AlSi10Mg powder. In particular, z-reinforced samples have been manufactured with the vertical extra strut aligned with the printing direction.

Samples are removed from the printing plate and manually grinded in order to remove the exceeding material, until the final height of 30 mm is reached. Later, in order to remove powder residues from the struts, an ultrasonic cleaning machine, where samples need to be immersed in distilled water, has been used; samples are then dried at  $80^{\circ}\mathrm{C}$  for  $16\mathrm{h}$ . Also, a vacuum desiccator has been used for removing air bubbles in order to properly measure the density of the samples via Archimedes' method [53]. The last step, before proceeding with static tests, is to perform a specific heat treatment identified as appropriate for  $\mathrm{AlSi}10\mathrm{Mg}$  [54], consisting of an annealing at  $350^{\circ}\mathrm{C}$  for  $2\mathrm{h}$ : as-built samples present, in fact, a brittle behavior that is not suited for energy absorption applications.

# 3.2. Compression tests

Experimental tests have been performed according to the German standard for the compression of cellular material [55]. The machine used for compression tests is a ZwickRoell Z100. Lattice specimens are compressed between two aluminum plates; the upper head of the machine is operated hydraulically in displacement control with a displacement rate of  $0,3\mathrm{mm / min}$ , while the force is measured. Samples are compressed along the printing direction, which is the direction normal to each layer of which the samples are composed.

Raw output data from the machine at the end of a test are force-displacement diagrams: those are easily convertible into stress-strain diagrams by means of expression (4). Once stress-strain diagrams are defined, it is possible to extract mechanical and energy absorption properties such as: Young modulus, yield stress  $\sigma_{\mathbf{y}}$  plateau stress  $\sigma_{pl}$  densification point  $\varepsilon_{D}$ , energy absorption efficiency  $\eta$ , EA, VEA and SEA. Standard used is DIN 50134 [55] whereby plateau stress is defined in the range between strain equal to  $20\%$  and  $40\%$ . Definition of  $\varepsilon_{D}$  alters from the standard: it has been defined as the strain equivalent with the  $\eta$


Table 3 Classification and numeration of the printed samples.


<table><tr><td>Cell</td><td>Initial</td><td>Process 1</td><td>Process 2</td></tr><tr><td>bcc</td><td>1-5/16</td><td>6-10</td><td>11-15</td></tr><tr><td>bccz</td><td>17-21/32</td><td>22-26</td><td>27-31</td></tr></table>

absolute maximum, as in a previous investigation [16]. Results of experimental tests, grading process, and their comparison, can be found in the next section.

# 4. Results

Results generated are shown in this chapter: early results from the static simulations can be considered the starting point of the investigation. Energetic properties improvements obtained from the processes application are evaluated on the basis of the initial properties. Such enhancements are verified through FEM simulation of the graded samples and later validated through results from the experimental campaign. Results will be discussed at the end of the chapter.

# 4.1. Results of the static simulations and stress state

The force reaction, EA (2), VEA (1) and SEA (3) from static simulations described in paragraph 2.1 are collected in Table 4.

Equivalent stress fringes of all the samples simulated can be seen in Figs. 3-5: such stress representations can be useful in the recognition of a common issue, especially for lattices, that is the load path. Stress is concentrated in specific zones of the sample, leaving others almost unloaded: this results in an incomplete exploitation of the possibility the lattice, and in particular that specific topology, is offering. Such problems can be found both in compression and in tension [52]. Higher stress concentrations are therefore isolated and schematized in Fig. 6, where it is possible to recognize specific behaviors: the  $bcc$  topology presents a cross-shaped load path, going from edge to edge, therefore generating a critical zone in the exact middle of the sample. This behavior is expected from  $bcc$  lattices, because of the presence of only diagonal struts. The situation is different when considering  $fcc$  lattices, that show stress concentrations on the vertical lateral surfaces. In fact, this topology presents struts aligned with the main horizontal axes only. Such concentrations are though hourglass-shaped since struts have a  $45^{\circ}$  angle orientation.  $Fbcc$ , as a combination of the two previous topologies, present a combination of the two stress fields: a cross-shaped load path is present going from corner to corner of the outside lateral surfaces. All of the z-reinforced counterparts of these configurations present a common stress concentration scheme, where the middle sector of the sample is the most loaded; also, concentrations are present at the corners of the sample, but those are due to border effects.

# 4.2. Results of the two grading processes

In this section, results from the grading process are shown. First of all, Table 5 shows the minimum and the maximum diameters reached for each specimen after one iteration of the process has been performed, for all of the thresholds. Subscript numbers define what grading process has been used.

Differences in term of diameters are clearly visible both from the table and from the pictures of the samples: only graded samples that have been verified through FEM simulations, using threshold 2 (the one that shows best results in terms of VEA and SEA enhancement) are represented in Figs. 7-8. Equivalent stress representations and schematizations are visible in Figs. 9-12, where it is possible to appreciate how the stress concentration pattern is changed: the load is distributed over the whole sample, rather than in specific areas, and this happens


Table 4 Properties defined from compression simulations for ungraded samples.


<table><tr><td></td><td>bcc</td><td>bccz</td><td>fcc</td><td>fccz</td><td>fbcc</td><td>fbccz</td></tr><tr><td>Force reaction [N]</td><td>1635.6</td><td>7447.4</td><td>4795.9</td><td>10,224</td><td>7740.8</td><td>13,351</td></tr><tr><td>EA [mJ]</td><td>683.1</td><td>3356.1</td><td>1917</td><td>4266</td><td>2937.6</td><td>5445.9</td></tr><tr><td>VEA[mJ/mm3]</td><td>0.0253</td><td>0.1243</td><td>0.0710</td><td>0.1580</td><td>0.1088</td><td>0.2017</td></tr><tr><td>SEA [mJ/g]</td><td>114.0</td><td>477.0</td><td>356.2</td><td>663.86</td><td>258.4</td><td>438.7</td></tr></table>

especially for z-reinforced samples modified via process 1. Stress concentration path modifications due to the grading can also be seen in the maps of the maximum equivalent stresses registered per cell of the horizontal central plane (the one lying on the x-y plane) of the sample, placed in the appendix.

With respect to the SEA and VEA values that can be found in Table 4, their increases in percentage are shown in Table 6. Gains obtained using threshold 3 are evident: this threshold has also been used for both the verification of the grading process through FEM and the validation of the model with the experimental tests.

In order to show the efficacy and the accuracy of the Matlab process in recalculating the VEA and SEA levels of the graded samples, histograms in Figs. 13-14 shows comparisons between VEAs and SEAs of the initial samples together with the ones redefined with the Matlab process and the validating FEM simulations performed on the graded samples. Results shown are inherent to the employment of threshold 2, while percentages on histograms are relative to the increase of VEA and SEA with respect to the original configuration.

# 4.3. Results of the experimental tests

Printed samples can be seen in Fig. 15 in their as-built configuration on the build platform. Medium densities measured through Archimedes' method for each configuration can be found in Table 7: given low standard deviations, it is possible to say that data acquired are valid. Stress-strain diagrams from experimental tests can be seen in Fig. 16. Differences between the two types of samples are evident:  $bcc$ , exception made for the sample graded via process 1 that has a quite higher relative density, has no local maximum at the beginning of the plateau, while  $bccz$  has the tendency to show more than one local maximum (less visible for  $bccz$  and  $bccz_{2}$ ) corresponding to the collapse of each layer. Such a trend has already been seen in a previous investigation [16].

Figs. 17-19 show obtained stress-strain diagrams, overlapped with efficiency diagrams, in order to allow a visual perspective of how the densification strain is defined. Also, these figures show the three main regions of the stress-strain diagrams, that define the mechanical behavior of lattice, and cellular solids in general. All of the mechanical properties defined in the DIN standard [55], including Young's modulus, yield stress, plateau stress and densification strain, together with energy absorption properties (1)-(3) are evaluated and collected in Table 8.

In order to allow a proper comparison between all of the tools used for the evaluation of the energetic properties of lattices involved in the validating experimental campaign, SEA and VEA bar graphs for all of the configuration tested are shown in Figs. 20-21: values obtained from FEM simulation evaluated though Matlab and obtained from experimental stress-strain diagrams are present.

# 4.4. Discussion

Results from the initial static simulations with the bilinear material model, presented in Table 4, are in line with results from previous investigations made about the same lattice topologies [16,17]. Z-reinforced lattices present a noticeable enhancement for both energy absorption and specific energy absorption. Best performing topology from the point of view of pure EA is  $fbccz$ , though it is surpassed by  $fccz$  when it comes to SEA, since this topology shows the best compromise between absorbed energy and mass.

Besides the main aim of the developed process, that is the enhancement of the EA properties, a secondary objective is the homogenization of the stress field, trying to generate configurations that can limit and mitigate stress concentration. Given the results obtained in terms of stress mitigation, load path of the sample is modified. In particular, it is clear from Figs. 9 and 11 that corners of the graded samples have been made stiffer, resulting into a homogenization of the stress in the top/bottom plane of the sample. A similar result has been obtained for tensile samples made of truss lattices in [52]. It has to be

![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/13550c2ab956832797e2feb687f8d992eb37648ce92ec6187f9a3744ccacfd72.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/1d7798e3fa1925ac855f364cdaed6deab70dbb6fb17966e2746e90f4c251e068.jpg)



Fig. 3. Representation of equivalent stress distribution for ungraded samples bcc (left) and bccz (right) from Ansys.


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/8b8f9621cf08c79328bdf5ae605408aa699602118b8a5f28d818493f8a95f6c3.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/b31a03f2edc7ba89cb093c76b400aadb3a6cf48d26ae3228956001aa3cc0a83d.jpg)



Fig. 4. Representation of equivalent stress distribution for ungraded samples fcc (left) and fccz (right) from Ansys.


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/94633b38db9e11419acda586a2fdd10ffec9043f33c7d2c6ee00cac8b1603771.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/4375c54892b722f6e60d0ffbd6db1f964bf0e157c9d5e996cba3958a6f9cabdb.jpg)



Fig. 5. Representation of equivalent stress distribution for ungraded samples fbcc (left) and fbccz (right) from Ansys.


said that these two phenomena, stress concentrations mitigation and energy absorption maximization are linked to each other, since the absence of critical zones in the sample means that all of the sample is absorbing energy in the most efficient way possible.

Depending on the process used and the threshold for the selection of the cells to be modified imposed, the diameters distribution can vary

significantly as is evident from Table 5. As expected, threshold 1, that equals to applying the process only to cells where the maximum equivalent stress exceeds the  $25\%$  of the average maximum stresses registered in the whole sample, is the one affecting less the renewal of the diameters. In every sample, and for both processes, there are certain cells that are not object to the grading process; also, the maximum


BCC


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/87d726cb61bef93cecb737410ed8c7a4d0bedbd6b16c840863e256f3ec3588de.jpg)



BCCZ


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/2b5c16ddf5b3d9202d0f1f8b8ae65431994b99199a7adc250ed69d0c49e466fa.jpg)



FCC


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/e83aca82e3b0c08e786be30acdb2bb0c75a76b4422c1139b0350d8bcecb9ef87.jpg)



FCCZ


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/b0c4b5764517101f743654010160ea41f4d10d5879fe113af3d2da5553d998ff.jpg)



FBCC


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/8632f18e7f902a00dacf7f07ba17854376f546d5545eabbbb667ab4e08b78982.jpg)



FBCCZ


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/a4e9b001d2b39ba9cf26ee929052dd97f6c954a2085515b5430dc23e56cd28cb.jpg)



Fig. 6. Equivalent stress concentration schemes for all of the ungraded samples.



Table 5 Minimum and maximum diameters of the graded samples for process 1 and process 2 (numbers next to samples) considering all of the thresholds.


<table><tr><td rowspan="2">Sample</td><td colspan="2">Threshold 1</td><td colspan="2">Threshold 2</td><td colspan="2">Threshold 3</td></tr><tr><td>tMIN[mm]</td><td>tMAX[mm]</td><td>tMIN[mm]</td><td>tMAX[mm]</td><td>tMIN[mm]</td><td>tMAX[mm]</td></tr><tr><td>bcc1</td><td>0.37</td><td>0.9084</td><td>1.0144</td><td>2.9928</td><td>0.37</td><td>1.3929</td></tr><tr><td>bcc2</td><td>0.37</td><td>0.4091</td><td>0.4183</td><td>1.0952</td><td>0.37</td><td>0.4573</td></tr><tr><td>bccz1</td><td>0.37</td><td>0.9248</td><td>0.5038</td><td>2.2981</td><td>0.37</td><td>1.3474</td></tr><tr><td>bccz2</td><td>0.37</td><td>0.4157</td><td>0.3796</td><td>0.7027</td><td>0.37</td><td>0.4648</td></tr><tr><td>fcc1</td><td>0.37</td><td>0.7184</td><td>1.4051</td><td>2.6686</td><td>0.37</td><td>1.2559</td></tr><tr><td>fcc2</td><td>0.37</td><td>0.3932</td><td>0.4558</td><td>0.7509</td><td>0.37</td><td>0.4397</td></tr><tr><td>fccz1</td><td>0.37</td><td>0.8446</td><td>0.3701</td><td>1.6115</td><td>0.37</td><td>1.1869</td></tr><tr><td>fccz2</td><td>0.37</td><td>0.4028</td><td>0.3701</td><td>0.5202</td><td>0.37</td><td>0.4504</td></tr><tr><td>fbcc1</td><td>0.37</td><td>0.5873</td><td>1.1296</td><td>1.7025</td><td>0.37</td><td>0.8702</td></tr><tr><td>fbcc2</td><td>0.37</td><td>0.3840</td><td>0.4540</td><td>0.6597</td><td>0.37</td><td>0.4293</td></tr><tr><td>fbccz1</td><td>0.37</td><td>0.4138</td><td>0.4872</td><td>1.4390</td><td>0.37</td><td>0.7651</td></tr><tr><td>fbccz2</td><td>0.37</td><td>0.3727</td><td>0.3822</td><td>0.5658</td><td>0.37</td><td>0.4167</td></tr></table>

diameter never goes beyond less than three times the initial one. The situation is totally different for threshold 2, where the process is applied to all of the cells presenting a maximum equivalent stress higher than the minimum of the maximum stresses registered in each cell: that means all of the cell undergoes the grading process with no discrimination. The main problem with this threshold is that diameters reached can be extremely high; in  $bcc1$  and  $fcc1$  for example, the maximum diameter obtained is almost  $3\mathrm{mm}$  that is equal to the edge length of the single lattice cell. In other words, the concept of lattice as a cellular material is

lost, since it has almost become a bulk material, unable to absorb energy with the same behavior as a lattice, and therefore out of the interest of this investigation. Threshold 3 represents the midpoint between the previous ones, where the limit is the exact average of the maximum equivalent stresses registered. As for threshold 1, there are cells that are not modified, but maximum diameters obtained still allow the material to be defined as a lattice structure. Bcc and bccz graded samples (using threshold 3), that can be seen in Figs. 7-8, show evident differences in diameters between process 1 and 2.

The influence of the process on initial diameters (Table 5) is reflected on the SEA and VEA percentage increases present in Table 6: threshold 1 presents very limited advantages, especially when relative density is high and process 1 is employed:  $fbc\bar{c}1$  and  $fbcz1$  present a SEA percentage increase below  $1\%$ . Threshold 2 on the contrary performs extremely high concerning SEA and VEA, but as already mentioned the material obtained cannot be interpreted as a lattice structure. Finally, threshold 3 offers a good enhancement of the properties, without increasing the mass excessively. Best performing samples have been both verified via FEM and experimentally validated. From the FEM verification, as it can be seen in Figs. 9-12, especially with process 1, stress concentrations are limited as well as border effects minimized. Best results from the point of view of the limitation of the border effects but also the homogenization of the stress field are obtained for  $bccz$  graded versions (Figs. 11-12), where corner concentrations are limited. FEM verification exhibits how the definition of both SEA and VEA for graded samples via Matlab is efficient and accurate within a certain margin: Figs. 13-14 show how the difference between SEA and VEA increases calculated with Matlab and FEM validation are in the order of  $1 - 5\%$ . Advantages of this tool are present also from the point of view of time elapsed for the definition of these properties, considering that the Matlab routine takes from the 3 to  $4\mathrm{min}$  while the FEM simulations (without considering the post-processing of the data obtained) take between 3 and  $8\mathrm{h}$ .

Samples selected for the FEM verification are also experimentally validated via compression load. Results obtained in Table 8 show how mechanical properties are influenced by the two processes. Process 1 tends to reduce the densification strain, therefore limiting the displacement until where the lattice is able to absorb energy. At the same time, the plateau stress is increased, enhancing the area defining the absorbed energy on the stress-strain diagram in the vertical direction. Figs. 20-21 show a comparison between VEAs and SEAs evaluated through FEM, Matlab and experimental tests (at the same strain, for sake of confrontation). Trends are the same for every way the properties have been evaluated, though it is evident how for  $bcc$ , and its graded versions, both VEA and SEA from experimental tests are two times or more higher than the ones evaluated from FEM and Matlab routine. The difference between these values lies in different factors; first, simulations are

![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/dff4bca4f50daeef84413c1abcaf3a25216e46c8737c69e199f0b80acbd3c2b8.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/feb10d60b634b9c7808f1354e0482920648b5cbc412611818cb7bc79d5af4551.jpg)



Fig. 7. Bcc1 and bcc2 graded samples (using threshold 3).


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/282685a8dc7c731ca48d88fb071f12acd78a0795a37a61f0d3e36758fe85867a.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/faa616598c4fd91985565e1c98698d1772c143604115571347392f524f3e9594.jpg)



Fig. 8. Bccz1 and bccz2 graded samples (using threshold 3).


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/54ef9869961ab174d5ff9d9ce1b682d3a929518bb9dc657f6f465f2f93f65344.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/816cf4ef10a0a76b325bd32635a32874c73a2f31713f23893b5254c803b43470.jpg)



Fig. 9. Representation of equivalent stress distribution for bcc1 (left) and relative equivalent stress concentration scheme (right).


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/18ad528bc1935dff0a68579ef7b60e3d1c1f3cea2ba32afc49ecfc48762c7149.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/7cd18a0ee53cc190f21c5884dcdc2dbe5c429fc60507637081ac9b5742919ade.jpg)



Fig. 10. Representation of equivalent stress distribution for bcc2 (left) and relative equivalent stress concentration scheme (right).


performed using beam elements that can result into less accurate results than solid elements, that would have required a higher computational effort for simulations that already lasted between 3 and  $8\mathrm{h}$  to be performed. Another reason for this discrepancy can be found in the properties used for the definition of the constituent material of lattices:

modeled AlSi10Mg (from Table 1) can differ from the actual one. First of all, a bilinear model is used for the simulation, which means that the plastic stage of the material is not perfectly replicated; also, as described in chapter 3, samples additively manufactured have been object to an annealing process in order to obtain an improved ductile behavior,

![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/cf8fadd321ebe6e5def40c2b83d6cb2ab9812a15ee4baa85b856b768732c5683.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/a7fe363c3b254fbd32111fb8c2efffe9df1c1cad08906037382b5b3adb00592e.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/4e460cc7d97d2182a42d7a3fff49e7137a2359e1c0c6c76e6af08dc23e3386e6.jpg)



Fig. 11. Representation of equivalent stress distribution for bccz1 (left) and relative equivalent stress concentration scheme (right).


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/82675bbf672581d7cd7145afd0db8655cb436f68f7c505c4fdcad44d8c9ad922.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/d5ab28a1f0c9c5eea438be86a497de0d6208ec8b80e37ab6ac5b6eed42cecf04.jpg)



Fig. 12. Representation of equivalent stress distribution for bccz2 (left) and relative equivalent stress concentration scheme (right).



Table 6 SEA and VEA percentage increases for process 1 and 2 (numbers next to the samples) considering all of the thresholds, with respect of SEA and VEA values present in table 4.


<table><tr><td rowspan="2">Sample</td><td colspan="2">Threshold 1</td><td colspan="2">Threshold 2</td><td colspan="2">Threshold 3</td></tr><tr><td>SEA increase</td><td>VEA increase</td><td>SEA increase</td><td>VEA increase</td><td>SEA increase</td><td>VEA increase</td></tr><tr><td>bcc1</td><td>+8.1611 %</td><td>+14.6250 %</td><td>+97.9656 %</td><td>+373.5205 %</td><td>+62.0911 %</td><td>+168.7713 %</td></tr><tr><td>bcc2</td><td>+7.1197 %</td><td>+7.5099 %</td><td>+125.7209 %</td><td>+404.7419 %</td><td>+10.7631 %</td><td>+16.6012 %</td></tr><tr><td>bccz1</td><td>+9.2978 %</td><td>+17.1360 %</td><td>+92.4692 %</td><td>+355.8356 %</td><td>+48.5460 %</td><td>+120.5102 %</td></tr><tr><td>bccz2</td><td>+7.0102 %</td><td>+7.6109 %</td><td>+51.6923 %</td><td>+127.5933 %</td><td>+12.6380 %</td><td>+17.6990 %</td></tr><tr><td>fcc1</td><td>+5.0125 %</td><td>+9.1549 %</td><td>+99.0058 %</td><td>+376.2092 %</td><td>+54.3633 %</td><td>+140.7094 %</td></tr><tr><td>fcc2</td><td>+7.0102 %</td><td>+7.3239 %</td><td>+70.6327 %</td><td>+189.152 %</td><td>+8.4243 %</td><td>+12.9581 %</td></tr><tr><td>fccz1</td><td>+1.5395 %</td><td>+2.5316 %</td><td>+86.4743 %</td><td>+326.5852 %</td><td>+25.6130 %</td><td>+55.1275 %</td></tr><tr><td>fccz2</td><td>+8.0490 %</td><td>+9.1041 %</td><td>+15.8018 %</td><td>+33.5443 %</td><td>+9.7483 %</td><td>+11.8992 %</td></tr><tr><td>fbcc1</td><td>+0.5929 %</td><td>+1.1029 %</td><td>+75.9475 %</td><td>+321.2357 %</td><td>+18.1493 %</td><td>+41.9122 %</td></tr><tr><td>fbcc2</td><td>+4.4623 %</td><td>+4.5037 %</td><td>+54.1981 %</td><td>+136.4180 %</td><td>+5.3055 %</td><td>+7.5368 %</td></tr><tr><td>fbccz1</td><td>+0.1041 %</td><td>+0.2478 %</td><td>+72.2363 %</td><td>+305.5611 %</td><td>+19.2940 %</td><td>+46.7538 %</td></tr><tr><td>fbccz2</td><td>+0.9273 %</td><td>+0.9419 %</td><td>+35.9917 %</td><td>+84.1840 %</td><td>+4.7786 %</td><td>+7.3376 %</td></tr></table>

leading to a variation of the initial properties. However, the main reason of discrepancy between experimental and modeled values of absorbed energy lies into the local deformations experienced by the samples. In fact, the experiments show the comparison of plastic hinges positioned at struts intersections that behaves differently from the rest of the lattice structure. This effect is limited to bcc cells, while is largely reduced in

case of z-reinforced samples. The local plasticization of the material is accompanied by large displacements and rotations at each node, which is not captured by the models although they contribute to increase sensitively the energy absorption of the entire structure. Finally, simulations do not take into consideration the friction that can be present between the sample and the crushing plates: this is also a main cause of

![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/3995fccc135d43d047d6f78e35b0827425a65ac8b55271a8925c779d44464d1d.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/ef4a1ad8cd85667e5807d0532c3e922256037548f8412ff8d71e852359ea6003.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/a7bea4cb2795b48e6978203968edf80d609a669adafcd645d535047bc5ade6f7.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/2c6e84c10f7bc1b64264f85eb892835e0fff1fe3eff5a90bfb2679041bd8ec22.jpg)



Fig. 13. SEA and VEA for bcc (left) and bccz (right) histograms, respectively for the initial configuration (blue), the graded via process 1 configuration with SEA and VEA evaluated via Matlab (green) and the graded via process 1 configuration with SEA and VEA evaluated via FEM (yellow).


the difference between models and experimental data. FEM and Matlab results are more accurate and in line with experimental results when it comes to z-reinforced samples, showing that differences also depend on the topology of the constituent cell of the samples.

Considering results obtained from experimental tests, SEA and VEA increases of the graded samples with respect to uniform samples can be compared to different data that can be found in literature concerning the application of graded design to lattices subject to uniaxial compression. In [56], a  $+23\%$  VEA increase has been registered for a functional linear grading design of a lattice sample presenting  $f2bcc$  cells. The grading applied in this study aims at obtaining an average relative density of the graded sample equal to the one of the uniform one, obtaining same masses for both samples. The VEA increase of this design can be therefore compared to the  $bccz2$  VEA increase present in this investigation, that is equal to  $+22\%$ . Both  $bccz$  and  $f2bcc$  presents in fact similar behaviors in terms of structural behaviors (as it can also be appreciated in [16]. Comparable results has been obtained in [57] as well, where  $+60\%$  for VEA has been performed by functionally graded sheet lattices with respect to uniform ones. Considering the evident differences between the structures involved in the comparison, such increases still are in the same order of magnitude of the ones that can be found in this study  $(+23\% bcc2, +92\% bccz1)$ . A gradient based on modifying the side lengths of  $sc-fcc$  lattice cells has been applied in [58], obtaining comparable results with the ones presented in terms of SEA.

Two different kinds of grading, based on reinforcing specific zones of the sample have been applied, leading to two configuration presenting respectively  $+41\%$  and  $+21\%$  SEA increases with respect to uniform samples. Such values can be compared to the SEA increases evaluated in this investigation  $(+80\% bcc1, +13\% bcc2, +40\% bccz1, +14\% bccz2)$ .

Overall, it can be said that the grading process, in particular the first one, together with the employment of threshold 3, is able to produce local reinforcements in the lattices aimed at generating significant changes in the configuration of the selected samples from different points of view: including the homogenization of the stress field, that makes the compression process much more efficient, and the improvement of the energy absorption properties also when it comes to obtaining a good compromise between the energy absorbed and the low mass of the sample. Benefits of the process from the point of view of the homogenization of the stresses can be appreciated in the maps of the maximum stresses registered presented in the appendix: this works better for z-reinforced samples, especially bccz. Moreover, similar, if not superior, performances can be appreciated in terms of SEA and VEA variations with respect to the application of simply linear and functionally graded design applied to lattice structures found in literature. The approach of the process presents limitations as well: at the moment, the developed routine is able to modify the diameter of the struts at the level of a whole cell; in other words, every cell must present the same diameter. Better results could be achieved by allowing the modification

![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/1a903ae6fce8326e85d812a6226637262f484518adb778a8c451fd49f0905f0b.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/3b83e6f853f8a60b0160b9a0d652bb1ea26c94463967297c3680c0990b493432.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/0cbe469e7af624ab5e55d4a31ef032c4aa684803e3264b2fed9f1cd6e105e533.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/0ca339ef79c114edd3c08f43f92c965a7680511df329f01e21d4402541c11eb5.jpg)



Fig. 14. SEA and VEA for bcc (left) and bccz (right) histograms, respectively for the initial configuration (blue), the graded via process 2 configuration with SEA and VEA evaluated via Matlab (green) and the graded via process 2 configuration with SEA and VEA evaluated via FEM (yellow).


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/56bf8b154280e39320e48be57c65f22249e6a37663696082fdca761e93de9478.jpg)



Fig. 15. As built samples still attached to the printing plate.


of the diameter at the level of the struts and not the cells: a more homogeneous stress field together with less critical zone to be manufactured (sudden changes in strut diameter within cells can result in difficulties while printing the samples) would be obtained.

# 5. Conclusions

A new grading tool for the improvement of mechanical properties of lattice structure has been developed: an analysis of the initial stress state


Table 7 Average densities and relative deviations for manufactured samples.


<table><tr><td>Cell</td><td>bcc</td><td>bcc1</td><td>bcc2</td><td>bccz</td><td>bccz1</td><td>bccz2</td></tr><tr><td rowspan="3">Average density [g/cm3]</td><td>2.6301</td><td>2.6254</td><td>2.6303</td><td>2.6274</td><td>2.6198</td><td>2.6428</td></tr><tr><td>±</td><td>±</td><td>±</td><td>±</td><td>±</td><td>±</td></tr><tr><td>0.0044</td><td>0.0106</td><td>0.0022</td><td>0.0064</td><td>0.0134</td><td>0.0372</td></tr></table>

of the structure is performed and energetic parameters are estimated. Based on the stress configuration obtained, the structure is locally reinforced through grading and therefore its mechanical properties, especially energetic ones, are improved. The process also offers a reliable predictability of improved properties and efficiency. The following points should be highlighted:

- The main aim of the process is achieved: energetic properties such as EA, VEA and SEA are improved for all of the samples processed, and results obtained via grading tools have been both verified via FEM and validated via experiments.

- The process is able to change the load path and stress distribution within the samples, allowing a better exploitation of the whole sample; this could lead to the enhancement of whole components or parts meant to be produced and eventually customized with lattice structures.

- The process used for the grading also allows the following evaluation of the energetic properties of the modified samples at a properly accurate level and in far less time than FEM data to be generated. The Matlab routine developed for the application of the process can be efficiently used as a pre-sizing tool for structural design and first assessment of the energetic performances.

Besides the achieved results, the process can be improved as well by allowing the grading to be applied on single struts rather than whole cells. Also, further investigations could be conducted about how this process could work when applied to a whole component meant to be designed employing lattice structures.

# CRediT authorship contribution statement

Antonio Coluccia: Writing - original draft, Visualization,

![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/45d18fcf9f0f55cebd39092a5cfb47324c21ff20567e290ab31acbea971e43b4.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/10a516f601f3321cb51433684a79161f8e2b828e63145a9bbe07b16d0480c816.jpg)



Fig. 16. Averaged stress-strain diagrams for bcc (left) and bccz (right) ungraded and graded samples from experimental compression tests.


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/6de6d9a1fdc827fe1de4d67d2036ba5ba8e5206a478faa3ffc73e3ff5eec01a3.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/5f6cad9c2c34045d1a1ae168e84ba1319a0cc2e173dd0c7990f71177099b5114.jpg)



Fig. 17. Stress-strain diagrams for bcc (left) and bccz (right) with relevant points: yield, begin of the plateau and densification.


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/158db63e4393bccc7c09bbdfdefc87289577a7bcf56070732bfe0e644d34691c.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/a42c266d7daa97d735109a9b2ab366b56eeea764d6af5e3603c51c0b3d160756.jpg)



Fig. 18. Stress-strain diagrams for bcc1 (left) and bccz1 (right) with relevant points: yield, begin of the plateau and densification.


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/034e3c96641a3c6f662801c37bda4d92e0c24e83e2bfd3fd032780ac2bc0b11a.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/546c28148884b2673fdf3713ea03b53c0dd6d345f53fefcb789143753c673c20.jpg)



Fig. 19. Stress-strain diagrams for bcc2 (left) and bccz2 (right) with relevant points: yield, begin of the plateau and densification.



Table 8 Mechanical properties of the samples experimentally tested under compression load; EA, VEA and SEA are evaluated at the same displacement as FEM simulations.


<table><tr><td>Sample</td><td>σy [MPa]</td><td>σpl [MPa]</td><td>εD</td><td>E [MPa]</td><td>EA [mJ]</td><td>SEA [mJ/g]</td><td>VEA [mJ/mm3]</td></tr><tr><td>bcc</td><td>0.8816</td><td>0.9918</td><td>0.6044</td><td>47.4662</td><td>1353.0</td><td>227.4227</td><td>0.0501</td></tr><tr><td>bcc1</td><td>2.9519</td><td>4.4047</td><td>0.2838</td><td>100.0545</td><td>6193.2</td><td>410.9877</td><td>0.2294</td></tr><tr><td>bcc2</td><td>1.0750</td><td>1.2097</td><td>0.5615</td><td>54.7060</td><td>1665.6</td><td>257.9249</td><td>0.0617</td></tr><tr><td>bccz</td><td>2.1218</td><td>2.2357</td><td>0.6015</td><td>173.5501</td><td>3755.8</td><td>562.7412</td><td>0.1391</td></tr><tr><td>bccz1</td><td>4.2741</td><td>4.8169</td><td>0.3576</td><td>319.5192</td><td>7232.7</td><td>794.7331</td><td>0.2679</td></tr><tr><td>bccz2</td><td>2.5830</td><td>2.7124</td><td>0.5555</td><td>201.5159</td><td>4577.7</td><td>646.4311</td><td>0.1695</td></tr></table>

Methodology, Investigation, Data curation, Conceptualization. Guillaume Meyer: Writing - review & editing, Validation, Methodology, Investigation, Data curation, Conceptualization. Stefania Liseni: Validation, Software, Investigation, Formal analysis, Data curation, Conceptualization. Christian Mittelstedt: Writing - review & editing, Supervision, Project administration, Methodology, Conceptualization. Giorgio De Pasquale: Writing - review & editing, Supervision, Project

administration, Methodology, Conceptualization.

# Declaration of competing interest

The authors declare that they have no known competing financial interests or personal relationships that could have appeared to influence the work reported in this paper.

![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/87722cb4569f20d192fc445a35ca57530fa82d03c50207e00fc3d3cfa296daf6.jpg)



Fig. 20. SEA values extracted from Ansys FEM simulations, Matlab and Experimental tests for all of the samples considered for the experimental validation.


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/714666041862303287c812742c36bf682d47d9bedbb820938105448aaea154c6.jpg)



Fig. 21. VEA values extracted from Ansys FEM simulations, Matlab and Experimental tests for all of the samples considered for the experimental validation.


# Appendix

In this appendix, maps of the maximum stress registered per cell on the horizontal central plane (fig. A1) of each ungraded and graded sample are shown in Figs. A2-A7. Although the two processes have a different formulation for the definition of the new diameters, they produce the same stress field, therefore those maps are valid for both process 1 and 2. Threshold 3 is used for the generation of these maps. It is clear from the maps how stress is homogenized through the whole plane for all of the graded samples: peaks are minimized, and stress discontinuities are limited.

![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/429022a3adf56a64d452dcceb898b416d4676fbb7e2217782d3710aaea04b547.jpg)


CENTRAL PLANE XY


Fig. A1. Representation of the central plane, where stress maps are extracted from


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/1c4cac2b97e89b3d56d56d9ce13a9c884ad1f197dd51a03e35538928ab2fc30a.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/f250cc9f72af7e657c1b91ea03aac76261430308aff2d62bb17e4c8d05d3fb7a.jpg)



Fig. A2. Map of the maximum equivalent stresses registered per cell concerning ungraded (left) and graded (right) bcc samples.


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/c61b9579f31cc7dbc55748c1d6330ebcb0bbeecd0213d04ec0228ec153f0984c.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/ce2151cc2a220647cfdbbf163114c0f3da1bfa847c6485b482c97a8f64e34747.jpg)



Fig. A3. Map of the maximum equivalent stresses registered per cell concerning ungraded (left) and graded (right) bccz samples.


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/b136893cfb13888bc79a5557b0136bd6c0b3e6404610914018d6ffb717128061.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/04ef94e56dbced1b1baf1930f9ec4522a51e6dc4d38e1bcc031b0aef144dd41f.jpg)



Fig. A4. Map of the maximum equivalent stresses registered per cell concerning ungraded (left) and graded (right) fcc samples.


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/867e357aa3eb21341c9bb27c6f410c30df6b3c4acec72fe79aabd7387aa2d5f9.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/dff00f528a6b5d4253f4a5b082a94cd40164b262a67187310b38799d4d1fa8e1.jpg)



Fig. A5. Map of the maximum equivalent stresses registered per cell concerning ungraded (left) and graded (right) fccz samples.


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/322e6e1d411c03e69fc30c3ba3fd8b3013206385cd25d96439454c9bb1f18135.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/0ba2cae992ec7578e643220d1867e5f26ab63cdfb736417fbce2a05f019f33e0.jpg)



Fig. A6. Map of the maximum equivalent stresses registered per cell concerning ungraded (left) and graded (right) fbcc samples.


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/ff3faf2be8c7328bf7ef8a7002ccac26505c0831ae6bb3b83bbe268306e14236.jpg)


![](file://D:/MinerU/转换结果/159.pdf-c7fd0f52-9426-455f-bb2e-2948e14ab756/images/15cdd8af28e73839abdb3e7d176a685271897f0917852eac275eb5b0c4af8c9d.jpg)



Fig. A7. Map of the maximum equivalent stresses registered per cell concerning ungraded (left) and graded (right) fbccz samples.


# Data availability

Data will be made available on request.

# References



[1] Ashby MF. Mechanical Properties of Cellular Solids. Metall Trans A Phys Metall Mater Sci 1983;14:1755-69. https://doi.org/10.1007/BF02645546.





[2] Deshpande VS, Fleck NA, Ashby MF. Effective properties of the octet-truss lattice material. J Mech Phys Solids 2001;49:1747-69.





[3] Seharing A, Azman AH, Abdullah S. A review on integration of lightweight gradient lattice structures in additive manufacturing parts. Adv Mech Eng 2020;12(6):1-21. https://doi.org/10.1177/1687814020916951.





[4] Dong L, Deshpande V, Wadley H. Mechanical response of Ti-6Al-4V octet-truss lattice structures. Int J Solids Struct 2015;60:107-24. https://doi.org/10.1016/j.ijsolstr.2015.02.020.





[5] Beyer C, Figueroa D. Design and Analysis of Lattice Structures for Additive Manufacturing. J Manuf Sci Eng Trans ASME 2016;138(12):1-15. https://doi.org/10.1115/1.4033957.





[6] Helou M, Kara S. Design, analysis and manufacturing of lattice structures: An overview. Int J Comput Integr Manuf 2018;31(3):243-61. https://doi.org/10.1080/0951192X.2017.1407456.





[7] Wang X, Zhong Z, Zeng T, Xu G, Cui Y, Zhang K. Heat transfer property of C/SiC composite pyramidal lattice core sandwich structures. Compos Struct 2022;301: 116215. https://doi.org/10.1016/j.compstruct.2022.116215.





[8] Shi X, Yang Z, Chen W, Chyu MK. Investigation of the effect of lattice structure on the fluid flow and heat transfer of supercritical CO2 in tubes. Appl Therm Eng 2022;207:118132. https://doi.org/10.1016/j.applthermaleng.2022.118132.





[9] Ott A, Biehs SA. Topological near-field heat flow in a honeycomb lattice. Int J Heat Mass Transf 2022;190:122796. https://doi.org/10.1016/j.ijheatmasstransfer.2022.122796.





[10] De Pasquale G, Tagliaferri A. Modeling and characterization of mechanical and energetic elastoplastic behavior of lattice structures for aircrafts anti-icing systems. Proc Inst Mech Eng Part C J Mech Eng Sci 2021;235(10):1828-39. https://doi.org/10.1177/0954406219853857.





[11] Kim Y, Kim I, Park J. An approximate formulation for the progressive failure analysis of a composite lattice cylindrical panel in aerospace applications. Aerosp Sci Technol 2020;106:106212. https://doi.org/10.1016/j.est.2020.106212.





[12] Smeets BJR, et al. Structural testing of a shear web attachment point on a composite lattice cylinder for aerospace applications. Compos Part B Eng 2021;212 (November):108691. https://doi.org/10.1016/j.compositesb.2021.108691.





[13] Davidson M, et al. Investigating amorphous metal composite architectures as spacecraft shielding. Adv Eng Mater 2013;15(1-2):27-33. https://doi.org/10.1002/adem.201200313.





[14] Feng J, Liu B, Lin Z, Fu J. Isotropic octet-truss lattice structure design and anisotropy control strategies for implant application. Mater Des 2021;203:109595. https://doi.org/10.1016/j.matdes.2021.109595.





[15] Liverani E, Rogati G, Pagani S, Brogini S, Fortunato A, Caravaggi P. Mechanical interaction between additive-manufactured metal lattice structures and bone in compression: implications for stress shielding of orthopaedic implants. J Mech Behav Biomed Mater 2021;vol. 121, no. March;104608. https://doi.org/10.1016/j.jmbbm.2021.104608.





[16] Coluccia A, Jiang G, Meyer G, De Pasquale G, Mittelstedt C. Nonlinear static and dynamic modeling of energy absorption lattice structures behavior. Mech Adv Mater Struct 2022. https://doi.org/10.1080/15376494.2022.2064016.





[17] Maconachie T, et al. The effect of topology on the quasi-static and dynamic behaviour of SLM AlSi10Mg lattice structures. Int J Adv Manuf Technol 2022;118 (11-12):4085-104. https://doi.org/10.1007/s00170-021-08203-y.





[18] Xiao L, Feng G, Li S, Mu K, Qin Q, Song W. Mechanical characterization of additively-manufactured metallic lattice structures with hollow struts under static and dynamic loadings. Int J Impact Eng 2022;vol. 169, no. June:104333. https://doi.org/10.1016/j.ijimpeng.2022.104333.





[19] Yin H, Zhang W, Zhu L, Meng F, Liu J, Wen G. Review on lattice structures for energy absorption properties. Compos Struct 2023;304(P1):116397. https://doi.org/10.1016/j.compstruct.2022.116397.





[20] M. F. Guo, H. Yang, and L. Ma, "3D lightweight double arrow-head plate-lattice auxetic structures with enhanced stiffness and energy absorption performance," Compos. Struct., vol. 290, no. March, 2022, 10.1016/j.compstruct.2022.115484.





[21] Sun ZP, Guo YB, Shim VPW. Static and dynamic crushing of polymeric lattices fabricated by fused deposition modelling and selective laser sintering – an experimental investigation. Int J Impact Eng 2022;160(October):104059. https://doi.org/10.1016/j.ijimpeng.2021.104059.





[22] B. Li, H. Liu, Q. Zhang, X. Yang, and J. Yang, “Crushing behavior and energy absorption of a bio-inspired bi-directional corrugated lattice under quasi-static compression load,” Compos. Struct., vol. 286, no. January, 2022, 10.1016/j.comstract.2022.115315.





[23] De Pasquale G, Sibona S. Hybrid materials based on polymers-filled AM steel lattices with energy absorption capabilities. Mech Adv Mater Struct 2021:1-13. https://doi.org/10.1080/15376494.2020.1871536.





[24] Zhu H, Wang P, Wei D, Si J, Wu Y. Energy absorption of diamond lattice cylindrical shells under axial compression loading. Thin-Walled Struct 2022;vol. 181, no. September:110131. https://doi.org/10.1016/j.tws.2022.110131.





[25] Baishya MJ, Sahariah BJ, Muthu N, Khanikar P. Composite Strut-Plate Lattice: A High-Stiffness Design of Cellular Metamaterial Having Excellent Strength and Energy Absorption Ability. SSRN Electron J 2022;vol. 33, no. September:104939. https://doi.org/10.2139/ssrn.4220781.





[26] Xue Y, Mu J, Huang Y, Shi Z. Experimental and Simulation Analysis on the Mechanical Behavior of 3D-Enhanced Al-Based Tetrahedral Lattice Materials. Phys Status Solidi A 2022;2200580:1-11. https://doi.org/10.1002/pssa.202200580.





[27] Sharma D, Hiremath SS. Experimental and FEM study on the in-plane and outplane loaded reversible dual-material bio-inspired lattice structures with improved energy absorption performance. Compos Struct 2023;303(March):116353. https://doi.org/10.1016/j.compstruct.2022.116353.





[28] Xiao L, Xu X, Feng G, Li S, Song W, Jiang Z. Compressive performance and energy absorption of additively manufactured metallic hybrid lattice structures. Int J Mech Sci 2022;vol. 219, no. January:107093. https://doi.org/10.1016/j.ijmecsci.2022.107093.





[29] Li L, Yang F, Li P, Wu W, Wang L. A novel hybrid lattice design of nested cell topology with enhanced energy absorption capability. Aerosp Sci Technol 2022; 128:107776. https://doi.org/10.1016/j.est.2022.107776.





[30] Habib FN, Ivenitti P, Masood SH, Nikzad M. Fabrication of polymeric lattice structures for optimum energy absorption using Multi Jet Fusion technology. Mater Des 2018;155:86-98. https://doi.org/10.1016/j.matdes.2018.05.059.





[31] Dara A, Bahubalendruni MAR, Johnny Mertens A, Balamurali G. Numerical and experimental investigations of novel nature inspired open lattice cellular structures for enhanced stiffness and specific energy absorption. Mater Today Commun 2022; 31(November):103286. https://doi.org/10.1016/j.mtccomm.2022.103286.





[32] Riot A, Panettieri E, Cosculluela A, Montemurro M. Influence of manufacturing process-induced geometrical defects on the energy absorption capacity of polymer lattice structures. Def Technol 2024;35:47-59. https://doi.org/10.1016/j.dt.2023.09.003.





[33] Sun ZP, Guo YB, Shim VPW. Influence of printing direction on the dynamic response of additively-manufactured polymeric materials and lattices. Int J Impact Eng 2022;167(December):104263. https://doi.org/10.1016/j.ijimpeng.2022.104263.





[34] Ramos H, Santiago R, Soe S, Theobald P, Alves M. Response of gyroid lattice structures to impact loads. Int J Impact Eng 2022;vol. 164, no. February:104202. https://doi.org/10.1016/j.ijimpeng.2022.104202.





[35] Červinek O, Pettermann H, Todt M, Koutny D, Vaverka O. Non-linear dynamic finite element analysis of micro-strut lattice structures made by laser powder bed fusion. J Mater Res Technol 2022;18:3684-99. https://doi.org/10.1016/j.jmrt.2022.04.051.





[36] Belingardi G, Montanini R, Avalle M. Characterization of polymeric structural foams under compressive impact loading by means of energy-absorption diagram. Int J Impact Eng 2001;25(5):455-72.





[37] Fíla T, et al. Dynamic impact testing of cellular solids and lattice structures: Application of two-sided direct impact Hopkinson bar. Int J Impact Eng 2021;148. https://doi.org/10.1016/j.ijimpeng.2020.103767.





[38] Bertolino G, Montemurro M, De Pasquale G. Multi-scale shape optimisation of lattice structures: an evolutionary-based approach. Int J Interact Des Manuf 2019; 13(4):1565-78. https://doi.org/10.1007/s12008-019-00580-9.





[39] Zhao M, Zhang DZ, Li Z, Zhang T, Zhou H, Ren Z. Design, mechanical properties, and optimization of BCC lattice structures with taper struts. Compos Struct 2022; vol. 295, no. April:115830. https://doi.org/10.1016/j.compstruct.2022.115830.





[40] Costa MR, Sohouli A, Suleman A. Multi-scale and multi-material topology optimization of gradient lattice structures using surrogate models. Compos Struct 2022;vol. 289, no. March:115402. https://doi.org/10.1016/j.compstruct.2022.115402.





[41] Bertolino G, Montemurro M. Two-scale topology optimisation of cellular materials under mixed boundary conditions. Int J Mech Sci 2022;216(August):106961. https://doi.org/10.1016/j.ijmecsci.2021.106961.





[42] Montemurro M, Roine T, Palihes J. Multi-scale design of multi-material lattice structures through a CAD-compatible topology optimisation algorithm. Eng Struct 2022;273(October):115009. https://doi.org/10.1016/j.engstruct.2022.115009.





[43] Zhang J, et al. Enhancing specific energy absorption of additively manufactured titanium lattice structures through simultaneous manipulation of architecture and constituent material. Addit Manuf 2022;vol. 55, no. February:102887. https://doi.org/10.1016/j.dddma.2022.102887.





[44] Yang J, et al. Compressive properties of bidirectionally graded lattice structures. Mater Des 2022;218:110683. https://doi.org/10.1016/j.matdes.2022.110683.





[45] Song J, Tang Q, Feng Q, Ma S, Guo F, Han Q. Investigation on the modelling approach for variable-density lattice structures fabricated using selective laser melting. Mater Des 2021;212(174):110236. https://doi.org/10.1016/j.matdes.2021.110236.





[46] Yu G, Xiao L, Song W. Deep learning-based heterogeneous strategy for customizing responses of lattice structures. Int J Mech Sci 2022;vol. 229, no. March:107531. https://doi.org/10.1016/j.ijmecsci.2022.107531.





[47] Alberdi R, et al. Multi-morphology lattices lead to improved plastic energy absorption. Mater Des 2020;194:108883. https://doi.org/10.1016/j.matdes.2020.108883.





[48] Montemurro M, Refai K, Catapano A. Thermal design of graded architected cellular materials through a CAD-compatible topology optimisation method. Compos Struct 2022;280(August):114862. https://doi.org/10.1016/j.compstruct.2021.114862.





[49] J. Plocher and A. Panesar, "Effect of density and unit cell size grading on the stiffness and energy absorption of short fibre-reinforced functionally graded lattice structures," Addit. Manuf., vol. 33, no. March, p. 101171, 2020, 10.1016/j.addma.2020.101171.





[50] A. Coluccia, G. Meyer, C. Mittelstedt, and G. De Pasquale, "Nonlinear dynamic modeling of the energetic behavior of multisheped lattice cells," 2021.





[51] Li QM, Magkiriadis I, Harrigan JJ. Compressive strain at the onset of densification of cellular solids. J Cell Plast 2006;42(5):371-92. https://doi.org/10.1177/0021955X06063519.





[52] Meyer G, Schelleis K, Weeger O, Mittelstedt C. Tensile specimen design proposal for truss-based lattice structures. Mech Adv Mater Struct 2022:1-28. https://doi.org/10.1080/15376494.2022.2097352.





[53] ISO/ASTM International, "ISO 3369: 2006 - Impermeable sintered metal materials and hardmetals - Determination of density," pp. 1-4, 2006, [Online]. Available: https://www.iso.org/standard/44435.html.





[54] Li D, Qin R, Xu J, Chen B, Niu X. Effect of heat treatment on AlSi10Mg lattice structure manufactured by selective laser melting: Microstructure evolution and compression properties. Mater Charact 2022;vol. 187, no. April:111882. https://doi.org/10.1016/j.matchar.2022.111882.





[55] Deutsches Institut für Normung, DIN 50134 Testing of metallic materials - Compression test of metallic cellular materials. 2008.





[56] Al-Saedi DSJ, Masood SH, Faizan-Ur-Rab M, Alomarah A, Ponnusamy P. Mechanical properties and energy absorption capability of functionally graded





F2BCC lattice fabricated by SLM. Mater Des 2018;144:32-44. https://doi.org/10.1016/j.matdes.2018.01.059.





[57] Zhao M, Zhang DZ, Liu F, Li Z, Ma Z, Ren Z. Mechanical and energy absorption characteristics of additively manufactured functionally graded sheet lattice structures with minimal surfaces. Int J Mech Sci 2019;167(September):2020. https://doi.org/10.1016/j.ijmecsci.2019.105262.





[58] Yue L, Liu H, Cheng Z, Kan Q, Kang G. Dynamic crushing behavior of a novel bidirectional gradient lattice structure under axial and oblique impact loadings. Thin-Walled Struct 2024;198(November):111697. https://doi.org/10.1016/j.tws.2024.111697.

