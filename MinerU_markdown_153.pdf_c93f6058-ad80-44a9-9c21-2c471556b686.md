# Energy absorption characteristics of butterfly-shaped multi-cellular honeycomb structures under compressive loading

![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/71dd655bf3fc55529925f461e0f4f46372b3ddf0fdb334ffb0959078745c24aa.jpg)


Zhong Yifeng a,b,c,\*, Liu Rong a,b, Poh Leong Hien c, Liu Xiaquan a,b, Tang Yuxin a,b

$^{a}$  School of Civil Engineering, Chongqing University, Chongqing, PR China

<sup>b</sup> Key Laboratory of New Technology of Construction of Cities in Mountain Area (Chongqing University), Ministry of Education, Chongqing 400045, PR China

$^{c}$  Department of Civil and Environmental Engineering, National University of Singapore, 1 Engineering Drive 2, E1A-07-03, Singapore 117576, Singapore

# ARTICLE INFO

Keywords:

Multi-cellular honeycomb

Auxetic effect

Elastic compressive behavior

Equivalent Cauchy model

Variational asymptotic method

# ABSTRACT

Replacing the inclined struts in re-entrant honeycombs with butterfly-shaped curved struts is intended to enhance both stiffness and energy absorption. To reduce modeling complexity, a three-dimensional equivalent Cauchy model (3D-ECM) for butterfly-shaped multi-cellular honeycomb structures (butterfly MHS) was developed within the framework of variational asymptotic method. The 3D-ECM's accuracy in predicting elastic compressive behavior was validated against 3D finite element model results and compression tests on 3D-printed specimens, with maximum errors within  $8.67\%$  for displacement, strain energy, and local field distribution. Strain energy analysis revealed that the normal strain energy (SE22) primarily contributes to transverse contraction, while the high shear strain energy along the 1-2 plane (SE12) indicates notable auxetic deformation. Energy-displacement curve analysis indicated that butterfly MHS exhibits the highest strain energy, demonstrating strong energy absorption capacity. Parameter studies revealed that increasing the arc radius and cell height enhances the auxetic effect, improving elastic compressive behavior. Importantly, the 3D-ECM reduced number of elements and model complexity, improving computational efficiency without loss of accuracy. Notably, the butterfly MHS outperformed both re-entrant and hexagonal MHS in elastic compressive behavior and specific energy absorption by  $32\%$  with identical dimensions and materials, significantly expanding its potential applications in construction engineering requiring lightweight and high-strength materials.

# 1. Introduction

Recently, there has been growing interest in cellular honeycombs exhibiting auxetic or negative Poisson's ratio (NPR) effect due to their excellent impact resistance and compression performance [1,2]. The concept of auxency refers to a phenomenon wherein material deforms in a manner aligning the deformation in the orthogonal direction with the loading axis [3,4]. Specifically, auxetic metamaterials demonstrate a contraction trend in the orthogonal direction when compression [5-8]. Certain specialized cellular honeycombs exhibit this auxetic deformation mode, particularly in multi-cellular configurations [9]. Furthermore, auxetic metamaterials result in internal convergence towards the compressed region when compressed, transiently increasing material density in that area, thereby enhancing its stiffness and strength [10, 11]. This feature has emerged as a focal point in honeycomb structure research [12,13]. Recent developments in metamaterials have demonstrated their potential for energy absorption and harvesting, as discussed by Govindarama et al. [14], which underscores the significance of optimized design for multifunctional performance in structural

applications. Furthermore, the nested multi-cell structures studied in le et al. [15] demonstrate superior crashworthiness through hierarchical design, highlighting the value of bio-inspired principles in honeycomb configurations.

Re-entrant structures are extensively studied auxetic structures recognized for their easily controllable mechanical properties [16,17]. Common examples include the re-entrant hexagonal [18], star-shaped [19], and double-V cellular honeycombs [20]. To enhance structural performance while preserving their inherent characteristics, researchers have introduced hybrid structures with innovative configurations by combining two or more types of unit cells (as illustrated in Fig. 1). Through strategic design, these hybrid structures demonstrate unique features that are unattainable with individual unit cell, all while maintaining the auxetic effect [21,22].

For instance, Alomarah et al. [23] combined chiral structures with re-entrant hexagonal structures, resulting in a chiral dilatation structure that exhibited superior energy absorption capacity. Zhang et al. [24] introduced a novel hybrid dilatation structure by merging vertically

<table><tr><td colspan="2">Nomenclature</td></tr><tr><td>η</td><td>parameter representing the ratio of micro-to macro-dimensions</td></tr><tr><td>Γ</td><td>three-dimensional strain field</td></tr><tr><td>&lt;·&gt;</td><td>average volume over the unit-cell</td></tr><tr><td>ρ*</td><td>equivalent density</td></tr><tr><td>θ</td><td>included angle of the butterfly-shaped strut</td></tr><tr><td>εij, εij</td><td>strain field of original structure and equiv-alent model, respectively</td></tr><tr><td>a,b</td><td>height and length of the unit cell, respec-tively</td></tr><tr><td>Ce*</td><td>Cauchy stiffness matrix</td></tr><tr><td>fi, mi</td><td>generalized force and moment</td></tr><tr><td>R</td><td>arc radius</td></tr><tr><td>s</td><td>cell boundary</td></tr><tr><td>t</td><td>strut thickness</td></tr><tr><td>U,W</td><td>strain energy and virtual work generated by the applied load</td></tr><tr><td>ui,ūi</td><td>displacement fields of original structure and 3D-ECM, respectively</td></tr><tr><td>V</td><td>volume occupied by the unit-cell</td></tr><tr><td>w</td><td>difference function</td></tr><tr><td>xi, yi</td><td>macro- and micro-coordinates, respectively</td></tr><tr><td>3D-ECM</td><td>three-dimensional equivalent Cauchy model</td></tr><tr><td>3D-FEM</td><td>three-dimensional finite element model</td></tr><tr><td>MHS</td><td>multi-cellular honeycomb structure</td></tr><tr><td>VAM</td><td>variational asymptotic method</td></tr></table>

reinforced re-entrant structures with hexagonal structures, leading to stress-strain curves featuring a secondary plateau stress. Wang et al. [25,26] designed re-entrant-star structures, highlighting their advantages in deformation patterns under varying impact velocities. Hybrid design has proven to be an effective and reliable approach, enabling the combination of two or more basic configurations to create new hybrid honeycombs with diverse connection types [27,28]. Consequently, enhancing the mechanical properties of cellular honeycombs through hybrid design strategies is indeed feasible [29,30].

Drawing inspiration from various naturally occurring curved structures, such as mollusk shells [31], turtle shells [32], and beetle elytra [33], known for their high stiffness, strength, and energy absorption capabilities for self-protection [34], circular shapes are among the most prevalent in curved structures [35]. Several innovative auxetic structures have incorporated arc elements [36-38]. Qi et al. [39,40] developed a circular honeycomb structure by substituting semi-circular arcs for the diagonal supports in conventional re-entrant structures. Zhang et al. [41] enhanced the biomimetic re-entrant hexagonal honeycomb cell by replacing the inclined struts with curved ones, and simulation results demonstrated a smoother and more stable in-plane compressive response. Yan et al. [42] replaced the inclined walls of honeycombs with double arcs to enhance energy dissipation. Tatlier et al. [43] enhanced the overall rigidity of the conventional re-entrant structure by integrating circular elements while maintaining its auxetic effect. These investigations underscore the feasibility of designing innovative structures by combining conventional re-entrant hexagonal configurations with arc elements, resulting in enhanced mechanical performance while retaining the auxetic effect [44-46].

For evaluating quasi-static mechanical performance of auxetic cellular honeycombs, commonly employed theoretical models are used for predictive calculations [47-51], supported by quasi-static experiments

and finite element simulations [52-54]. However, due to their intricate geometric characteristics, comprehensive numerical simulations through finite element analysis may pose challenges in fully assessing their performance under various conditions and could potentially lead to convergence issues during the solution process [55,56]. This complexity impedes initial design and performance prediction, highlighting the critical need for an efficient and precise analytical approach to address these limitations [57,58].

Recently, Zhong et al. [59,60] introduced a multiscale modeling technique for analyzing periodic composite materials and structures using the variational-asymptotic method (VAM) [61-63]. This technique involves asymptotically expanding the energy functional of a unit cell by utilizing small structural parameters (e.g., thickness-to-width ratio) and systematically discarding higher-order terms to obtain different-order approximate energies and their corresponding simplified models [64]. Compared to high-order theories [65,66] and zig-zag theories [67,68], this method simplifies model complexity and reduces computational costs while ensuring accuracy and efficiency.

This work extends the VAM to develop the three-dimensional equivalent Cauchy model (3D-ECM) for analyzing the elastic compressive behavior – encompassing stiffness, deformation, and energy absorption – of butterfly-shaped multi-cellular honeycomb structures (abbreviated as butterfly MHS), laying a foundation for understanding its deformation and energy absorption capabilities. The Cauchy continuum model, commonly referred to as the classical continuum model, is widely used in engineering applications [69,70]. To the best of the authors' knowledge, there are currently no reports on the elastic compressive behavior and energy absorption capabilities of the butterfly MHS.

This paper is organized as follows: Section 2 provides a detailed description of the geometry of the butterfly MHS. Section 3 establishes the theoretical formulas and constitutive relationships of the 3D-ECM for butterfly MHS using the VAM. Section 4 validates the accuracy of the equivalent model through uniaxial compression tests on 3D-printed specimens. Section 5 investigates the impact of different structural parameters on the elastic compressive behavior of the butterfly MHS. Section 6 compares the elastic compressive behaviors of different MHS configurations. Finally, Section 7 summarizes the main conclusions.

# 2. Geometry of butterfly-shaped honeycomb structure

This section outlines the geometric design and parameters of the butterfly-shaped honeycomb structure. Inspired by butterfly wings, this structure features polygonal wings and a central connecting element. The advantages of this design include: (1) increased strength and stiffness along with a lightweight construction, resulting in reduced overall weight and optimized material efficiency [71]; (2) the polygonal wing design provides resistance to bending and compression, enhancing structural robustness under external loads; and (3) the geometric configuration effectively distributes external loads, reducing stress concentrations and thereby improving overall mechanical performance and load-bearing capacity [72].

The bio-inspired design of the butterfly-shaped honeycomb structure, illustrated in Fig. 2(b), was conceived based on auxetic honeycombs, particularly the re-entrant auxetic honeycomb (RAH) shown in Fig. 2(a). This structure not only retains the traditional advantages of honeycombs - lightweight construction and high strength - but also effectively incorporates the auxetic effect. The innovation lies in replacing the inclined struts of the re-entrant honeycomb with butterfly-shaped struts. This unique design enables the butterfly-shaped honeycomb structure to generate additional plastic hinges during failure, thereby efficiently dissipating excess energy under external impacts.

The geometric parameter in Fig. 2(c) are clarified as follows:  $R$  symbolizes the arc radius,  $\theta$  denotes the included angle of the butterfly-shaped strut;  $t$  signifies the thickness of the horizontal tie, whereas the connecting tie has a thickness of  $2t$ . In addition,  $a$  and  $b$  correspond to the height and length of a unit cell, respectively, with the cell's depth

![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/208ac9f21642501c799a534dbb55c81bdf53e3bd22614e0ca90896f8c5b13859.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/4bcb9c4ee9feaf280aa0336e063b0eaa8465559cb29291aec31ecee43e2a9d77.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/92501180d68114ea457eb2da17bccc711af4164b591f6f02591656e138cb5c52.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/f32f4168ee14af5ece459da66046e4af42a34dc05e1695bbf190eef02633930f.jpg)



Fig. 1. Hybrid design of cellular honeycombs with auxetic effect, (a) re-entrant-chiral auxetic structure [23], (b) vertical-reinforced re-entrant structure [24], (c) re-entrant-star honeycomb structure [25,26], (d) circular-re-entrant structure [41], and circle-reinforced re-entrant structure [43].


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/db9a2bc094502b80ce71fb3366e7e8e56d3fde906f3d2b082ea61b5db94752d4.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/85aa8047be2e969971180337434006b42b1d253e6d9f17fe4688603eb7260e6b.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/cdb0f8ad326fa2074012e10defb581c6239bad11c96e722622f55227ec183f58.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/353ffc1034ffb440909ffe34a6fafde1e3235a99ed6b9a51c51453b2826615dc.jpg)



Fig. 2. Geometries of the re-entrant auxetic honeycomb (a) and the butterfly-shaped honeycomb structure (b), along with the dimensions of the unit cell (c) and a quarter of the unit cell (d).


denoted as  $h$ . All struts feature a rectangular cross-section of  $h \times t$ , except for the tie having a rectangular cross-section of  $h \times 2t$ . The projected length of the cell in the 1- and 2-directions can be obtained as

$$
a = 2 R \sin \theta , b = 2 R \cos \theta + R. \tag {1}
$$

It is important to note that butterfly inclined struts should not overlap and need to adhere to specified constraints as

$$
2 R <   b. \tag {2}
$$

To ensure the proper functioning of the connecting tie and the auxetic effect, certain criteria must be met as

$$
0 ^ {\circ} <   \theta <   9 0 ^ {\circ}. \tag {3}
$$

The total mass of the butterfly MHS cell is

$$
m = 4 \left(2 R t + 2 R \frac {\theta \pi}{1 8 0}\right) h \rho , \tag {4}
$$

where  $\rho$  is mass density of base material.

The total volume occupied by the unit-cell is

$$
V = a b h = 2 R \sin \theta (2 R \cos \theta + R) h. \tag {5}
$$

The equivalent density of butterfly MHS can be obtained as

$$
\rho^ {*} = \frac {4 \left(t + \frac {\theta \pi}{1 8 0}\right)}{R \sin \theta (2 \cos \theta + 1)} \rho . \tag {6}
$$

# 3. VAM-based equivalent Cauchy model for butterfly MHS

This section outlines the derivation procedure for the VAM-based 3D-ECM tailored for the butterfly MHS. While the Cauchy continuum model can be applied to analyze various behaviors of heterogeneous structures, this study specifically focuses on their linear elastic behavior. The material stiffness parameters are derived through the homogenization of the unit cell within the butterfly MHS and are subsequently incorporated into the 3D-ECM, as depicted in Fig. 3.

To highlight the butterfly MSH design, the derivation process for the equivalent model (3D-ECM) has been relocated to the Supplementary

![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/0ebbc51db290a3c0ed35d453d2f1122fc48814ff039961402369524cd43dcb1b.jpg)



Fig. 3. Flowchart for constructing (c) three-dimensional equivalent Cauchy model (3D-ECM) for (a) butterfly MHS through (b) VAM-based homogenization of the unit cell (Homo.).


Materials. The linear elasticity constitutive relation of the Cauchy continuum model can be obtained as

$$
2 U = \left\{ \begin{array}{l} \bar {\epsilon} _ {1 1} \\ \bar {\epsilon} _ {2 2} \\ \bar {\epsilon} _ {3 3} \\ 2 \bar {\epsilon} _ {2 3} \\ 2 \bar {\epsilon} _ {1 3} \\ 2 \bar {\epsilon} _ {1 2} \end{array} \right\} ^ {T} \left[ \begin{array}{c c c c c c} C _ {1 1} & C _ {1 2} & C _ {1 3} & C _ {1 4} & C _ {1 5} & C _ {1 6} \\ C _ {1 2} & C _ {2 2} & C _ {2 3} & C _ {2 4} & C _ {2 5} & C _ {2 6} \\ C _ {1 3} & C _ {2 3} & C _ {3 3} & C _ {3 4} & C _ {3 5} & C _ {3 6} \\ C _ {1 4} & C _ {2 4} & C _ {3 4} & C _ {4 4} & C _ {4 5} & C _ {4 6} \\ C _ {1 5} & C _ {2 5} & C _ {3 5} & C _ {4 5} & C _ {5 5} & C _ {5 6} \\ C _ {1 6} & C _ {2 6} & C _ {3 6} & C _ {4 6} & C _ {5 6} & C _ {6 6} \end{array} \right] \left\{ \begin{array}{l} \bar {\epsilon} _ {1 1} \\ \bar {\epsilon} _ {2 2} \\ \bar {\epsilon} _ {3 3} \\ 2 \bar {\epsilon} _ {2 3} \\ 2 \bar {\epsilon} _ {1 3} \\ 2 \bar {\epsilon} _ {1 2} \end{array} \right\}. \tag {7}
$$

where  $[C]$  represents the  $6\times 6$  material stiffness matrix of the Cauchy continuum model.

For orthotropic materials, Eq. (7) can be reformulated as

$$
\left\{ \begin{array}{l} \varepsilon_ {1 1} \\ \varepsilon_ {2 2} \\ \varepsilon_ {3 3} \\ 2 \varepsilon_ {2 3} \\ 2 \varepsilon_ {1 3} \\ 2 \varepsilon_ {1 2} \end{array} \right\} = \left[ \begin{array}{c c c c c c} \frac {1}{E _ {1}} & - \frac {\nu_ {2 1}}{E _ {2}} & - \frac {\nu_ {3 1}}{E _ {3}} & 0 & 0 & 0 \\ - \frac {\nu_ {1 2}}{E _ {1}} & \frac {1}{E _ {2}} & - \frac {\nu_ {3 2}}{E _ {3}} & 0 & 0 & 0 \\ - \frac {\nu_ {1 3}}{E _ {1}} & - \frac {\nu_ {2 3}}{E _ {2}} & \frac {1}{E _ {3}} & 0 & 0 & 0 \\ 0 & 0 & 0 & \frac {1}{G _ {2 3}} & 0 & 0 \\ 0 & 0 & 0 & 0 & \frac {1}{G _ {1 3}} & 0 \\ 0 & 0 & 0 & 0 & 0 & \frac {1}{G _ {1 2}} \end{array} \right] \left\{ \begin{array}{l} \sigma_ {1 1} \\ \sigma_ {2 2} \\ \sigma_ {3 3} \\ \sigma_ {2 3} \\ \sigma_ {1 3} \\ \sigma_ {1 2} \end{array} \right\}. \tag {8}
$$

where  $E_{1}, E_{2}, E_{3}$  are Young's moduli in three directions,  $G_{12}, G_{13}, G_{23}$  are shear moduli in 1-2, 1-3, and 2-3 planes,  $\nu_{12}, \nu_{13}, \nu_{23}$  and  $\nu_{21}, \nu_{31}, \nu_{32}$  are two set of Poisson's ratios, in which only  $\nu_{12}, \nu_{13}, \nu_{23}$  are given and the other Poisson's ratios are calculated as

$$
\nu_ {2 1} = \nu_ {1 2} E _ {2} / E _ {1}, \quad \nu_ {3 1} = \nu_ {1 3} E _ {3} / E _ {1}, \quad \nu_ {3 2} = \nu_ {2 3} E _ {3} / E _ {2}, \tag {9}
$$

due to the symmetry of the compliance matrix.

Eq. (8) can be inverted to obtain the same expression in Eq. (7) with

$$
\begin{array}{l} C _ {1 1} = \frac {E _ {1} \left(1 - v _ {2 3} v _ {3 2}\right)}{\Delta}, \quad C _ {1 2} = \frac {E _ {2} \left(v _ {1 2} + v _ {1 3} v _ {3 2}\right)}{\Delta}, \quad C _ {1 3} = \frac {E _ {3} \left(v _ {1 3} + v _ {1 2} v _ {2 3}\right)}{\Delta}, \\ C _ {2 2} = \frac {E _ {2} \left(1 - v _ {1 3} v _ {3 1}\right)}{\Delta}, \quad C _ {2 3} = \frac {E _ {3} \left(v _ {2 3} + v _ {1 3} v _ {2 1}\right)}{\Delta}, \quad C _ {3 3} = \frac {E _ {3} \left(1 - v _ {1 2} v _ {2 1}\right)}{\Delta}, \tag {10} \\ C _ {4 4} = G _ {2 3}, \quad C _ {5 5} = G _ {1 3}, \quad C _ {6 6} = G _ {1 2}, \\ \end{array}
$$

with  $\Delta = 1 - \nu_{12}\nu_{21} - \nu_{23}\nu_{32} - \nu_{13}\nu_{31} - 2\nu_{21}\nu_{13}\nu_{32}$  and other items being zero.

# 4. Results and discussion

# 4.1. Uniaxial compression verification

The uniaxial compression test is a foundational experiment employed to evaluate mechanical performances. This test allows for the determination of key parameters such as the elastic modulus, yield strength, and failure modes of the butterfly MHS. The insights gained from these findings are invaluable for material selection, structural design, and performance enhancement.

# 4.1.1. Material properties testing

In this section, the butterfly MHS specimens are fabricated using Fused Deposition Modeling (FDM) technology, with key parameters set as follows: layer height of  $0.2\mathrm{mm}$ , infill density of  $100\%$  for structural integrity, print speed at  $50~\mathrm{mm / s}$ , nozzle temperature set to  $230^{\circ}\mathrm{C}$ , bed temperature maintained at  $90^{\circ}\mathrm{C}$ , and nozzle diameter of  $0.4\mathrm{mm}$ . Polylactic Acid (PLA) was selected as the printing material due to its cost-effectiveness and rapid printing capabilities.

Both the tensile test coupons and the butterfly MHS specimens were prepared using the ELEGOO Mars 3D printer known for its improved print quality achieved through a dual gear structure that ensures accurate filament delivery to the print head. Moreover, the lightweight design of the print head facilitates faster printing speeds. The selected universal electronic testing machine is the CMT-5205 model by New Sinsun, which provides several advantages, including high precision, user-friendly operation, and a high degree of automation, making it well-suited for a wide range of testing applications. With a maximum load capacity of  $50\mathrm{kN}$ , the machine accurately outputs load and displacement data via a data acquisition system.

To minimize systematic errors, three "dog bone" tensile coupons, each measuring  $330 \times 60 \times 2 \mathrm{~mm}$  according to ASTM D638 standards, as shown in Fig. 4(a), were employed and labeled as coupons 1 to 3. A uniaxial strain rate of  $0.5 \mathrm{~mm} / \mathrm{min}$  was applied until the specimens fractured while load data was recorded in real-time. Based on the stress-strain curves in Fig. 4(b), the material's elastic modulus was calculated to be  $3410 \mathrm{MPa}$ , with a standard deviation of  $34 \mathrm{MPa}$ . The calculation assumes initial linear elasticity, reflecting the material's behavior up to its elastic limit. Additionally, the Poisson's ratio and density were determined to be 0.36 and  $1.25 \mathrm{~g} \cdot \mathrm{cm}^{-3}$ , respectively, with corresponding standard deviations of 0.0021 and  $0.0005 \mathrm{~g} \cdot \mathrm{cm}^{-3}$  (see Table 1). In this study, all specimens were subjected to loads kept within the elastic limit of ABS plastic, with a yield stress of  $40 \mathrm{MPa}$ .

# 4.1.2. Uniaxial compression test

To verify the accuracy of the VAM-based equivalent model in predicting the uniaxial elastic compressive behavior of the butterfly MSH, the baseline dimensions of the unit cell are selected as follows:  $t_1 = t_2 = 0.5t_3 = 0.5$  mm,  $R = 3$  mm,  $h = 2$  mm,  $l_1 = 2.4$  mm,  $a = 5$  mm, and  $b = 9.6$  mm, as illustrated in Fig. 5. The butterfly MHS is composed of  $5 \times 5 \times 5$  honeycomb cells, with plates added to the top and bottom. The length, width and depth of multi-cellular MHS are measured as  $48$  mm,  $25$  mm, and  $10$  mm, respectively.

The butterfly MHS specimens were 3D-printed with PLA material based on the structural 3D model. To ensure consistency with the material properties results from "dog bone" tensile coupons, it is necessary to match the printing path, layer height, and printing speed employed for the compressive specimens. The CMT-5205 electronic universal testing machine was employed for the uniaxial compression test. Following the installation of the support shaft, the specimen was positioned between the platens, and loading commenced at a velocity


(a)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/248ba492f81ad3c414a16e3b757d817cd8f9b364aa736532458507c570a547a2.jpg)



(b)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/ac47fabba2a783d7adf26159c14d9e494e821eaddd1a5521f7fec8048477b108.jpg)



Fig. 4. (a) Setup for standard tensile test and (b) stress-strain curve of PLA material.



(a)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/d56cf9f4f56975e499859d6e096c127d9afceb90de354e5187f4a368709f4d86.jpg)



(b)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/04675401b577d0a26d243d89015889fed88bb04561411fd708fa92ada44f5511.jpg)



Fig. 5. (a) Dimensions of butterfly MHS cell and (b) its  $1/4$  unit cell.



Table 1 Elastic modulus of PLA material obtained from standard tensile test.


<table><tr><td>Coupons</td><td>Ultimate load [N]</td><td>Ultimate deformation [mm]</td><td>Modulus [MPa]</td><td>Average modulus [MPa]</td><td>Standard deviation [mm]</td><td>Error [%]</td></tr><tr><td>Coupon 1</td><td>10,351.137</td><td>3</td><td>3450.379</td><td></td><td></td><td>1.17</td></tr><tr><td>Coupon 2</td><td>10,775.155</td><td>3.2</td><td>3367.236</td><td>3410.421</td><td>34.020</td><td>-1.27</td></tr><tr><td>Coupon 3</td><td>9,899.579</td><td>2.9</td><td>3413.648</td><td></td><td></td><td>0.095</td></tr></table>

of  $2.5\mathrm{mm / min}$ . The universal testing machine was connected to a computer for continuous capture of applied load on the specimen and displacement. The compressive deformation process of the specimen was recorded using a digital camera, as illustrated in Fig. 6.

Fig. 7 illustrates the elastic compression process, beginning with uniaxial loading applied to the specimen in Fig. 7(a), inducing initial internal concave deformation as shown in Fig. 7(b). Upon reaching the elastic limit  $(\varepsilon_{33} = 0.029)$  in Fig. 7(c), the butterfly-shaped inclined struts begin bending and folding at their connections to the horizontal ties, exhibiting significant "X"-shaped deformation. The local bending and folding of the inclined struts highlight primary energy dissipation zones, consistent with previous studies on auxetic cellular structures. Lateral contraction during compression is more pronounced at the edges, while the deformation inside the specimen is smaller or takes different forms, such as folding formation. This localized deformation, driven by the geometric design, amplifies the auxetic effect at the specimen's edges. Although the curved struts do not exhibit distinct buckling, their 'folding' behavior, resulting from the structure's re-entrant geometry, contributes to energy absorption.

This auxetic effect enhances load-bearing capacity until fracture occurs in the inclined struts. Fracture initiates at high-stress points and propagates along the strut length, as shown in Fig. 7(d), reflecting the tensile failure typical of brittle materials like PLA. The high print quality prevented visible delamination or inter-layer detachment during testing. The pronounced "X"-shaped deformation pattern seen in the specimen's center further illustrates the auxetic design's ability to convert axial load into distributed transverse strain energy, maximizing resilience under compression. It is worth noting that while the model primarily focuses on elastic response, the implications of plastic deformation and energy absorption at higher loads are acknowledged as part of the structure's performance.

# 4.1.3. Numerical simulation of uniaxial compression

Furthermore, two three-dimensional models, as shown in Fig. 8(b) and (c), were developed utilizing ABAQUS software to simulate the uniaxial elastic compression of the butterfly MHS. In these models, the lower part was fixed, while a displacement load of  $-2.5 \times 10^{-3}$


(a)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/f2910ed4dd8d80f58e1e53edef75377e0b2057fd998be6b4cc7f34e214eddd0c.jpg)



(b)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/a3cfca79f9849dbaa785e239140008a5c70971e5da82c852c720ab4f70786300.jpg)



Fig. 6. Uniaxial compression test of the multi-cell specimen: (a) compression specimen (unit: mm); (b) compression setup.



(a)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/9790c594609636b934a0e97943c1af5b77dd1749913717e732af325765cdb063.jpg)



(b)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/a317ef430aa3c8a89a7df9d5cc4840ff377c751c2ce3a99fea773feecb8db18c.jpg)



(c)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/d272436facb953e5ef136430ca9aec85a8ff9d17136f63764eedac2db9171d1d.jpg)



(d)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/57ddce251f2fee55a4cfe361e13a795d6c0ee8f9bbc229e508576a1e95eecb5d.jpg)



Fig. 7. Uniaxial elastic compression process of the butterfly MHS specimen, (a)  $\varepsilon_{33} = 0$  (initial state), (b)  $\varepsilon_{33} = 0.001$  (early stage of deformation), (c)  $\varepsilon_{33} = 0.029$  (elastic limit), and (d)  $\varepsilon_{33} = 0.282$  (failure state).


m was applied in the 3-direction to the top platen to replicate the experimental loading and boundary conditions illustrated in Fig. 8(a). To ensure the reliability and accuracy of the numerical simulations, a mesh convergence study was conducted for both the 3D-FEM and 3D-ECM, as shown in Fig. 9. The choice of C3D10 elements was justified based on their suitability for complex curved geometries. Local mesh refinement was applied in high-stress regions to minimize errors due to stress concentration. Initially, there is a noticeable difference in the maximum elastic displacements predicted by the two models, likely due to the coarse mesh. However, as the mesh is refined, both

models converge to a maximum elastic displacement of  $3.94\mathrm{mm}$ . While refining the mesh enhances computational accuracy, it also increases computational time and resource demands. For subsequent analyses, a balance between accuracy and efficiency was achieved by selecting a setup with 104,664 solid elements (C3D10) for 3D-FEM and 6,624 solid elements (C3D10) for 3D-ECM.

# 4.1.4. Load-displacement curve under uniaxial elastic compression

The load-displacement curve is a valuable tool for evaluating both the stiffness (indicated by the slope) and the strength (represented by

![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/035638d1daa5701917f7343f365dfeaaad00c00bd1cc80acc248edd36cb8f00d.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/1e251c3e3443b5205764173d1d965df7ec3d94779048b2f777e3dced5452d939.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/89d372d6e54ea9b0ab62219aadd299fc2c097669e911a3fd7a2525721a98aa1a.jpg)



Fig. 8. Three-dimensional models for simulating uniaxial elastic compression deformation of butterfly MHS, (a) boundary and loading conditions with letters C and F representing clamped and free boundaries, respectively, (b) 3D-FEM, and (c) 3D-ECM.


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/73d4ae38d97d3c611550438626187dc783bd031a0cf6b8bd0865adeb83023b2a.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/136c35154313f68714eaeaddbb9f727ffa9e65e353ccdb3f53143e35c14d6d4e.jpg)



Fig. 9. Mesh convergence analysis of C3D10 element number for the compressive displacement of the butterfly MHS: (a) 3D-FEM and (b) 3D-ECM.


the peak force) of the butterfly MHS, providing insight for optimizing its design for practical applications. Load-displacement curves under uniaxial elastic compression were generated through numerical simulations and then compared with experimental data to ensure accuracy and reliability.

Fig. 10(a) to (c) compare the load-displacement curves for three MHS configurations: butterfly MHS, hexagonal MHS, and re-entrant MHS under uniaxial elastic compression. The discrepancies between the experimental curves and the predictions from both 3D-FEM and 3D-ECM for all three configurations are below  $5\%$ , confirming that the proposed equivalent model can accurately capture their elastic compression behaviors. Analysis of the deformation modes reveals that the hexagonal MHS undergoes lateral expansion, whereas both the re-entrant MHS and butterfly MHS exhibit notable lateral contraction. The comparison also indicates that the butterfly MHS demonstrates approximately  $15\%$  improved elastic compressive behavior over the re-entrant MHS, highlighting its superior load-bearing characteristics under identical material and dimensional conditions. Further investigation into the butterfly MHS shows that its butterfly-shaped inclined struts bend inward under compressive loads, forming a densified structure that significantly enhances load-bearing capacity.

Fig. 10(d) compares the energy-displacement curves for the two models under identical conditions, clearly illustrating the energy variation throughout the loading process. The butterfly MHS demonstrates the highest strain energy, followed by the re-entrant MHS, with the hexagonal MHS showing the lowest, highlighting the butterfly MHS's strong energy absorption capacity and suitability for energy-absorbing applications. The curves for the two models align closely, with a maximum discrepancy of only  $4.47\%$  in the butterfly MHS, meeting the prescribed accuracy criteria. These results suggest that the 3D-ECM serves as a reliable alternative to the 3D-FEM in analyzing strain energy.

Table 2 compares the specific energy absorption  $(SEA = \frac{EA}{M}$ , where  $M$  is the specimen's mass;  $EA = \int_0^d F(x_2)dx_2$ , where  $d$  is compressive displacement and  $F$  is force) for three MHS configurations. The butterfly MHS shows a  $21.3\%$  improvement over the re-entrant MHS and  $30.9\%$  improvement over the hexagonal MHS in specific energy absorption, demonstrating superior crashworthiness while maintaining a lightweight design. Specifically, as the structure undergoes lateral contraction, structural densification enhances local stiffness, reduces stress concentration, and improves the overall stability and energy absorption capacity. Due to the unique geometry of butterfly MHS, structural densification also helps in promoting a more uniform distribution of stresses, thus enhancing the compressive strength of the structure during the compression process.

# 4.2. Elastic compressive mode verification

Table 3 compares the elastic deformation maps among different MHS configurations as predicted by 3D-FEM and 3D-ECM. The analysis indicates that 3D-ECM can accurately predict the elastic compression behavior of three MHS configurations up to the elastic limit, particularly highlighting the symmetrical distribution patterns of total displacement  $(u_{\mathrm{magnitude}})$  and lateral displacement  $(u_{1})$  on both sides of the MHS configurations. Examination of the deformation patterns reveals that the hexagonal MHS exhibits a pronounced outward expansion under elastic compressive loads, highlighting the deformation characteristics of the positive Poisson's ratio cellular honeycomb. Notably, there is a significant maximum expansion in the middle margin, while the displacements in the bottom margin are relatively minor, likely due to constraints imposed by the plates.

In contrast, the re-entrant MHS and butterfly MHS demonstrate distinctive features compared to the hexagonal MHS, manifesting significant contraction behavior. This contraction behavior highlights the

![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/f120d75c78abb9a44139cd2c0d52ad765a81d08a91c47fd142494bc99845e303.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/680c70260a3e14f8a5daf8ae40e67af937ec480ac329b4c9da9ce79662d03a2a.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/2c037a86eefd95e206a4c5121daf8ef5e96e33f1ff798f724bf3682637e96d45.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/cfa4294a8d702147fe1a8acd99c6c059ed4aa213f07f698a3e033d3a2cae817c.jpg)



Fig. 10. Comparison between numerical simulation and experimental load-displacement curves for three MHS configurations under uniaxial elastic compression: (a) butterfly MHS, (b) hexagonal MHS, (c) re-entrant MHS, and (d) strain energy-displacement curves.



Table 2 Comparison of specific energy absorption in different MHS configurations.


<table><tr><td>Metric</td><td>Butterfly MHS</td><td>Re-entrant MHS</td><td>Hexagonal MHS</td><td>Improvement (%) vs Re-entrant MHS</td><td>Improvement (%) vs Hexagonal MHS</td></tr><tr><td>SEA (J/g)</td><td>1.245</td><td>1.026</td><td>0.951</td><td>+21.3%</td><td>+30.9%</td></tr></table>

auxetic effect, in which the structure contracts perpendicular to the applied stress direction instead of expanding. Notably, the primary contraction area is located in the middle margin of the MHS, exhibiting a distinctive "X"-shaped deformation pattern that further highlights its auxetic effect.

Quantitatively, the maximum value of  $u_{\mathrm{magnitude}}$  predicted by 3DFEM for the butterfly MHS is  $3.935 \times 10^{-3} \mathrm{~m}$ , whereas the corresponding value from 3D-ECM is  $3.954 \times 10^{-3} \mathrm{~m}$ , resulting in a prediction error of only  $0.48\%$ . Conversely, the prediction error for the lateral displacement  $u_{1}$  is slightly higher at  $2.42\%$ . These error margins are considered acceptable, underscoring the precision and reliability of the 3D-ECM in predicting elastic compressive displacements for this specific MHS. In conclusion, the 3D-ECM accurately predicts the macroscopic distribution of elastic compressive displacement, elucidating the variations within the butterfly MHS and identifying the regions of peak displacements. This observation has significant implications for understanding and leveraging the auxetic behavior of the butterfly MHS in engineering design and optimization.

# 4.3. Local field recovery verification

Before structural compression failure, local deformation typically occurs within the honeycomb cell. It is crucial to closely monitor the variations in the local field within the honeycomb structure. The point of maximum displacement is designated as the recovery point, where global displacements, generalized strains, and curvatures are used as key inputs to determine the local stress, strain, and displacement fields within the unit cell. This recovery enables a comparative analysis with the relevant results obtained from the 3D-FEM, enhancing the understanding of the elastic compressive behavior of the multi-cellular structure. Tables 4-5 compare the local field distributions within the central unit cell of the butterfly MHS under uniaxial compression. Compared to the results from the 3D-FEM, the relative differences of the recovered local stresses and displacements from 3D-ECM are all below  $8.67\%$ . The displacement clouds of the two models show substantial agreement, indicating that the local recovered field demonstrates high accuracy.


Table 3 Comparison of the displacement clouds for three MHS configurations under uniaxial elastic compression, as predicted by the 3D-ECM and 3D-FEM (unit: m).


<table><tr><td rowspan="2">Model</td><td colspan="2">\( u_{\text{magnitude}} \)</td><td colspan="2">\( u_1 \)</td></tr><tr><td>3D-FEM</td><td>3D-ECM</td><td>3D-FEM</td><td>3D-ECM</td></tr><tr><td rowspan="2">butterfly MHS</td><td>Max: 3.935e-03</td><td>Max: 3.954e-03</td><td>Max: 3.668e-03</td><td>Max: 3.581e-03</td></tr><tr><td>Max: 2.532e-03</td><td>Max: 2.523e-03</td><td>Max: 1.549e-03</td><td>Max: 1.555e-03</td></tr><tr><td>hexagonal MHS</td><td>Max: 3.381e-03</td><td>Max: 3.393e-03</td><td>Max: 1.090e-03</td><td>Max: 1.094e-03</td></tr><tr><td rowspan="8">re-entrant MHS</td><td>Max: 3.989e-03</td><td>Max: 3.989e-03</td><td>Max: 1.090e-03</td><td>Max: 1.094e-03</td></tr><tr><td>Max: 3.989e-03</td><td>Max: 3.989e-03</td><td>Max: 1.090e-03</td><td>Max: 1.094e-03</td></tr><tr><td>Max: 3.989e-03</td><td>Max: 3.989e-03</td><td>Max: 1.090e-03</td><td>Max: 1094e-03</td></tr><tr><td>Max: 3.989e-03</td><td>Max: 3.989e-03</td><td>Max: 1.090e-03</td><td>Max: 1.094e-03</td></tr><tr><td>Max: 3.989e-03</td><td>Max: 3.989e-03</td><td>Max: 1.094e-03</td><td>Max: 1.094e-03</td></tr><tr><td>Max: 3.989e-03</td><td>Max: 3.989e-03</td><td>Max: 1.094e-03</td><td>Max: 1.094e-03</td></tr><tr><td>Max: 3.989e-03</td><td>Max: 3.989e-</td><td>Max: 1.094e-03</td><td>Max: 1.094e-03</td></tr><tr><td>Max: 3.989e-03</td><td>Max: 3.989e-</td><td>Max: 1.094e-03</td><td>Max: 1.094e-03</td></tr></table>


Table 4 Comparison of local stress field distribution within the central unit cell of the butterfly MHS, as predicted by 3D-FEM and 3D-ECM (unit: MPa).


<table><tr><td>Stresses</td><td colspan="2">σ11</td><td colspan="2">σ12</td><td colspan="2">σ13</td></tr><tr><td rowspan="10">3D-FEM</td><td>S,S11(Avg. 75%)</td><td>S,S12(Avg. 75%)</td><td>S,S13(Avg. 75%)</td><td>S,S14(S,S15)</td><td>S,S15(Avg. 75%)</td><td>S,S16(S,S17)</td></tr><tr><td>+2.087e+00</td><td>+1.549e+00</td><td>+1.269e+01</td><td>+1.272e+01</td><td>+1.245e+01</td><td>+1.270e+01</td></tr><tr><td>+1.719e+00</td><td>+1.719e+00</td><td>+1.719e+01</td><td>+1.719e+01</td><td>+1.719e+01</td><td>+1.719e+01</td></tr><tr><td>+1.351e+00</td><td>+1.039e+00</td><td>+1.039e+01</td><td>+1.039e+01</td><td>+1.039e+01</td><td>+1.039e+01</td></tr><tr><td>+8.633e-01</td><td>+7.692e-01</td><td>+7.692e-01</td><td>+7.692e-01</td><td>+7.692e-01</td><td>+7.692e-01</td></tr><tr><td>+2.414e-01</td><td>+2.494e-01</td><td>+2.494e-01</td><td>+2.494e-01</td><td>+2.494e-01</td><td>+2.494e-01</td></tr><tr><td>+4.884e-01</td><td>+2.704e-01</td><td>+2.704e-01</td><td>+2.704e-01</td><td>+2.704e-01</td><td>+2.704e-01</td></tr><tr><td>+3.593e-01</td><td>+3.303e-01</td><td>+3.303e-01</td><td>+3.303e-01</td><td>+3.303e-01</td><td>+3.303e-01</td></tr><tr><td>+1.592e-00</td><td>+1.050e-00</td><td>+1.050e-00</td><td>+1.050e-00</td><td>+1.050e-00</td><td>+1.050e-00</td></tr><tr><td>+2.328e-00</td><td>+1.570e-00</td><td>+1.570e-00</td><td>+1.570e-00</td><td>+1.570e-00</td><td>+1.570e-00</td></tr><tr><td rowspan="12">3D-ECM</td><td>S,S11(Avg. 75%)</td><td>S,S12(Avg. 75%)</td><td>S,S13(Avg. 75%)</td><td>S,S14(S,S15)</td><td>S,S15(Avg. 75%)</td><td>S,S16(S,S17)</td></tr><tr><td>+2.288e+00</td><td>+1.646e+00</td><td>+1.646e+00</td><td>+1.646e+00</td><td>+1.646e+00</td><td>+1.646e+00</td></tr><tr><td>+1.888e+00</td><td>+1.373e+00</td><td>+1.373e+00</td><td>+1.373e+00</td><td>+1.373e+00</td><td>+1.373e+00</td></tr><tr><td>+1.719e+00</td><td>+1.199e+00</td><td>+1.199e+00</td><td>+1.199e+00</td><td>+1.199e+00</td><td>+1.199e+00</td></tr><tr><td>+1.103e+00</td><td>+8.293e-01</td><td>+8.293e-01</td><td>+8.293e-01</td><td>+8.293e-01</td><td>+8.293e-01</td></tr><tr><td>+7.143e-01</td><td>+5.537e-01</td><td>+5.537e-01</td><td>+5.537e-01</td><td>+5.537e-01</td><td>+5.537e-01</td></tr><tr><td>+6.250e-02</td><td>+1.050e-02</td><td>+1.050e-02</td><td>+1.050e-02</td><td>+1.050e-02</td><td>+1.050e-02</td></tr><tr><td>+4.621e-01</td><td>+3.347e-01</td><td>+3.347e-01</td><td>+3.347e-01</td><td>+3.347e-01</td><td>+3.347e-01</td></tr><tr><td>+3.393e-01</td><td>+8.072e-01</td><td>+8.072e-01</td><td>+8.072e-01</td><td>+8.072e-01</td><td>+8.072e-01</td></tr><tr><td>+1.278e-00</td><td>+1.215e-00</td><td>+1.215e-00</td><td>+1.215e-00</td><td>+1.215e-00</td><td>+1.215e-00</td></tr><tr><td>+2.005e-00</td><td>+1.352e-00</td><td>+1.352e-00</td><td>+1.352e-00</td><td>+1.352e-00</td><td>+1.352e-00</td></tr><tr><td>+2.393e-00</td><td>+1.625e-00</td><td>+1.625e-00</td><td>+1.625e-00</td><td>+1.625e-00</td><td>+1.625e-00</td></tr><tr><td>Max. error</td><td colspan="2">8.67%</td><td colspan="2">6.28%</td><td colspan="2">3.58%</td></tr><tr><td>Stresses</td><td colspan="2">σ22</td><td colspan="2">σ23</td><td colspan="2">σ33</td></tr><tr><td rowspan="9">3D-FEM</td><td>S,S22(Avg. 75%)</td><td>S,S23(Avg. 75%)</td><td>S,S23(Avg. 75%)</td><td>S,S23(Avg. 75%)</td><td>S,S23(Avg. 75%)</td><td>S,S23(Avg. 75%)</td></tr><tr><td>+3.394e+00</td><td>+8.698e-01</td><td>+8.698e-01</td><td>+8.698e-01</td><td>+8.698e-01</td><td>+8.698e-01</td></tr><tr><td>+3.394e+00</td><td>+8.698e-01</td><td>+8.698e-01</td><td>+8.698e-01</td><td>+8.698e-01</td><td>+8.698e-01</td></tr><tr><td>+3.394e+00</td><td>+8.698e-01</td><td>+8.684e-01</td><td>+8.684e-01</td><td>+8.684e-01</td><td>+8.684e-01</td></tr><tr><td>+3.394e+00</td><td>+8.698e-01</td><td>+8.698e-01</td><td>+8.698e-01</td><td>+8.698e-01</td><td>+8.698e-01</td></tr><tr><td>+3.394e+00</td><td>+8.698e-01</td><td>-3.800e-03</td><td>-3.800e-03</td><td>-3.800e-03</td><td>-3.800e-03</td></tr><tr><td>+3.394e+00</td><td>+8.698e-01</td><td>-3.800e-03</td><td>-3.800e-03</td><td>-3.800e-03</td><td>-3.800e-03</td></tr><tr><td>+3.394e+00</td><td>+8.698e-01</td><td>-3.844e-01</td><td>-3.844e-01</td><td>-3.844e-01</td><td>-3.844e-01</td></tr><tr><td>+3.394e+00</td><td>+8.698e-01</td><td>-3.844e-01</td><td>-3.844e-01</td><td>-3.844e-01</td><td>-3.844e-01</td></tr><tr><td>Max. error</td><td colspan="2">5.84%</td><td colspan="2">6.32%</td><td colspan="2">2.59%</td></tr></table>

Table 4 illustrates that the localized stress predominantly concentrates at the intersection of the butterfly-shaped inclined strut and connecting tie. This finding aligns with the deformation mechanism of the butterfly-shaped honeycomb, highlighting the crucial role of the inclined strut in the compressive deformation process. Consequently, in subsequent parameter analyses, design elements of the inclined strut - such as strut thickness, included angle, and radius - must be carefully evaluated and optimized to enhance the inclined strut's strength, thereby mitigating or preventing potential damage. Table 5 illustrates that the butterfly MHS demonstrates a distinctive "X" deformation pattern under elastic compressive loading, which corresponds closely with the deformation modes detailed in Section 4.2. This alignment not only validates the model's accuracy but also enhances the understanding of the deformation characteristics of the butterfly MHS.

# 4.4. Strain energy components

The anisotropy exhibited by the butterfly MHS under uniaxial compressive loads result in varying amounts of stored elastic energy in different directions, emphasizing the necessity of analyzing the structural strain energy components. Each distinct strain energy component represents a unique mechanism of energy retention and dissipation. Examining these individual strain energy components enables a deeper understanding of structural behavior and energy absorption performance.

Since the strain energy components of 3D-ECM cannot be directly output in ABAQUS software, this section calculates the strain energy components  $SE_{ij}$  for the butterfly MHS under uniaxial compressive


Table 5 Comparison of local displacement distribution within the central unit cell of the butterfly MHS, as predicted by 3D-FEM and 3D-ECM (unit: mm).


<table><tr><td>Displacements</td><td colspan="2">\( u_{\text{magnitude}} \)</td><td>\( u_1 \)</td><td>\( u_2 \)</td></tr><tr><td rowspan="12">3D-FEM</td><td>U, Magnitude</td><td>U, U1</td><td>U, U2</td><td>U, U2</td></tr><tr><td>+1.631e+00</td><td>+7.212e-01</td><td>+8.501e-01</td><td></td></tr><tr><td>+1.502e+00</td><td>+4.013e-01</td><td>+9.149e-01</td><td></td></tr><tr><td>+1.437e+00</td><td>+3.615e-01</td><td>+1.045e+00</td><td></td></tr><tr><td>+1.373e+00</td><td>+2.418e-01</td><td>+1.108e+00</td><td></td></tr><tr><td>+1.308e+00</td><td>+1.217e-01</td><td>+1.174e+00</td><td></td></tr><tr><td>+1.244e+00</td><td>+1.750e-03</td><td>+1.239e+00</td><td></td></tr><tr><td>+1.179e+00</td><td>+1.304e+00</td><td>+1.366e+00</td><td></td></tr><tr><td>+1.115e+00</td><td>-2.381e-01</td><td>-1.434e+00</td><td></td></tr><tr><td>+1.050e+00</td><td>-4.980e-01</td><td>-1.458e+00</td><td></td></tr><tr><td>+9.215e-01</td><td>-5.978e-01</td><td>-1.563e+00</td><td></td></tr><tr><td>+8.570e-01</td><td>-7.177e-01</td><td>-1.628e+00</td><td></td></tr><tr><td rowspan="13">3D-ECM</td><td>U, Magnitude</td><td>U, U1</td><td>U, U2</td><td>U, U2</td></tr><tr><td>+1.741e+00</td><td>+7.532e-01</td><td>+9.080e-01</td><td></td></tr><tr><td>+1.669e+00</td><td>+6.311e-01</td><td>+9.725e-01</td><td></td></tr><tr><td>+1.598e+00</td><td>+1.037e+00</td><td>+1.102e+00</td><td></td></tr><tr><td>+1.526e+00</td><td>+3.888e-01</td><td>+1.166e+00</td><td></td></tr><tr><td>+1.454e+00</td><td>+2.646e-01</td><td>+1.231e+00</td><td></td></tr><tr><td>+1.353e+00</td><td>+1.425e-01</td><td>+1.295e+00</td><td></td></tr><tr><td>+1.311e+00</td><td>+2.035e-02</td><td>+1.380e+00</td><td></td></tr><tr><td>+1.239e+00</td><td>-1.018e-01</td><td>-1.424e+00</td><td></td></tr><tr><td>+1.168e+00</td><td>-4.361e-01</td><td>-1.489e+00</td><td></td></tr><tr><td>+1.096e+00</td><td>-4.652e-01</td><td>-1.553e+00</td><td></td></tr><tr><td>+9.525e+00</td><td>-9.918e-01</td><td>-1.618e+00</td><td></td></tr><tr><td>+8.812e-01</td><td>-7.125e-01</td><td>-1.682e+00</td><td></td></tr><tr><td>Max. error</td><td colspan="2">6.72%</td><td>4.37%</td><td>6.81%</td></tr></table>

![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/f6571bc16d812542117873c2aea2bfce1980703ba47ad0201cbebd578b9868ae.jpg)



Fig. 11. Comparison of strain energy component distributions of butterfly MHS under uniaxial compression, as predicted by different models.


loading as

$$
S E _ {i j} = \frac {U _ {i j}}{U _ {\text {t o t a l}}} (i, j = 1, 2, 3), \tag {11}
$$

where  $U_{\mathrm{total}}$  represents the total strain energy, and  $U_{ij}$  denotes the strain energy component corresponding to the stress component  $\sigma_{ij}$ , such as

$$
U _ {i j} = \frac {1}{2} \sum_ {k = 1} ^ {n} S _ {i j} E _ {i j} V _ {i j}, \tag {12}
$$

where  $k$  represents the element index of 3D-ECM,  $n$  denotes the total number of elements, and  $ij$  corresponds to the material orientations, including six different values: 11, 22, 33, 12, 13, and 23;  $S$ ,  $E$ , and  $V$  represent elemental stress, strain, and volume, respectively.

Fig. 11 compares the distribution of strain energy components under uniaxial compression, as predicted by different models. Specifically,  $SE_{11}$ ,  $SE_{22}$ , and  $SE_{33}$  correspond to compressive deformation components in the orthogonal directions:  $x$ -direction denoted by 11,  $y$ -direction by 22, and  $z$ -direction by 33. Similarly,  $SE_{12}$ ,  $SE_{13}$ , and  $SE_{23}$  represent shear stress/strain components on different planes—12 on the  $x-y$  plane, 13 on the  $x-z$  plane, and 23 on the  $y-z$  plane. The results reveal that  $SE_{22}$  accounts for  $23.59\%$ , signifying its primary role as the major compressive direction and indicating substantial strain energy accumulation. Despite not being the highest percentage, this value implies significant deformation in the 2-direction. Conversely,  $SE_{11}$

represents  $17.34\%$  , indicating considerable strain energy accumulation in the 1-direction. This suggests that 2-directional compression  $(SE_{22})$  results in significant transverse contraction, leading to notable strain energy accumulation. On the other hand,  $SE_{33}$  comprises only  $0.8\%$  indicating minimal deformation in the 3-direction and limited strain energy accumulation in that dimension--this is a common characteristic of metamaterials designed to exhibit greater stiffness in the 3-direction.

The proportions of  $SE_{13}$  and  $SE_{23}$  are less than  $0.1\%$ , indicating minimal shear deformation in the 1-3 and 2-3 planes. In contrast,  $SE_{12}$  significantly dominates the shear strain energy in the 1-2 plane, peaking at  $58.16\%$ , highlighting the pivotal role of shear deformation in enhancing the energy absorption capacity. This is consistent with the auxetic effect (negative Poisson's ratio) of the butterfly MHS, where significant transverse contraction occurs during compression, inducing shear strain energy. It also reflects the advantage of the 3D-EDM in addressing complex geometries and shear-bending coupling effects, eliminating the need for detailed calculations of the forces and deformations of each individual bar.

# 4.5. Computational efficiency

Effective equivalent models should accurately predict the mechanical response while maintaining high computational efficiency to streamline calculations, minimize costs, and enhance computational capacity within the same time-frame. Table 6 provides an efficiency comparison between 3D-FEM and 3D-ECM in compressive behavior analysis. Despite both models utilizing the same solid element, C3D10, the 3D-ECM requires significantly fewer elements - reducing the element count by  $93.67\%$  compared to 3D-FEM - resulting in lower computational costs. During compressive simulations of the butterfly MHS, the 3D-FEM takes approximately  $380~s$  to complete, whereas the 3D-ECM finishes the calculations in just  $12~s$ . This demonstrates a remarkable 7.4-fold increase in computational efficiency with 3D-ECM over 3D-FEM, which is crucial for engineering applications that involve extensive data and complex models.

# 5. Parameter influence analysis

This section investigates the influence of different parameters on the compressive displacement, specific moduli, and Poisson's ratio of the butterfly MHS under elastic compression. Given the deformation mechanism of the butterfly MHS, it is recognized that critical parameters affecting its mechanical properties include the arc radius, cell height, and strut thickness. Consequently, this section primarily focuses on their impact on the elastic compressive behavior. To address the need for structural lightweighting, the concept of specific modulus is introduced, defined as the ratio of elastic modulus to equivalent density, which helps mitigate the effects of mass variations on compressive behavior.


Table 6 Comparison of computational efficiency between 3D-ECM and 3D-FEM in compressive behavior analysis of butterfly MSH.


<table><tr><td>Models</td><td>3D-FEM</td><td>3D-ECM</td><td>Reduction in elements /Efficiency improvement</td></tr><tr><td>Element type</td><td>C3D10</td><td>C3D10</td><td>/</td></tr><tr><td>Number of element</td><td>104,664</td><td>6,624</td><td>93.67%</td></tr><tr><td>Computation time</td><td>380 s</td><td>12 s</td><td>7.4 times</td></tr></table>


(a)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/228f4d8c0467539b763b5d87e4106136b5e3570d3c82883f4e8af301bda4df63.jpg)



(b)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/f02f528b237fe3e6d28b0cbe20f6f27e90ac3997780827a1efa17525d23dc816.jpg)



(c)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/5eb01748f22268d5de6d7bb241065b2cfd19ddc65b5ab436d3e358a2300c9cf9.jpg)



(d)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/396459a6d2e45cad388b792908a8e43781bbfc29725270f6dd4b74592599f0c5.jpg)



Fig. 12. Effect of arc radius  $R$  on (a) specific elastic modulus  $E_{i} / \rho^{*}$ , (b) specific shear modulus  $G_{ij} / \rho^{*}$ , (c) compressive displacement  $u_{i}$ , and (d) Poisson's ratio  $\nu_{12}$  of the butterfly MHS.


# 5.1. Arc radius

Fig. 12(a) and (b) illustrate the influence of arc radius  $(R = 2.7 - 3.3\mathrm{mm})$  on the specific elastic moduli of the butterfly MHS while keeping other parameters constant. The specific moduli  $E_{1} / \rho^{*}$ ,  $E_{2} / \rho^{*}$ ,  $G_{12} / \rho^{*}$ , and  $G_{13} / \rho^{*}$  show an increasing trend, though they also exhibit fluctuations as the radius increases. These variations are attributed to the supportive function of the honeycomb inclined struts at the ends of the connecting ties, enhancing the structure's ability to resist deformation. In contrast, the changes in  $E_{3} / \rho^{*}$  and  $G_{23} / \rho^{*}$  are less pronounced, indicating a lower sensitivity to radius variations in the 3-direction. Even though the variation in radius is independent of the thickness direction, the gradual increase in overall mass results in a slight reduction in specific moduli.

Fig. 12(c) illustrates a gradual decrease in compressive displacement with an increasing radius. This phenomenon arises from the overall increase in specific modulus as the radius increases, which enhances displacement resistance in all directions. Fig. 12(d) illustrates a more pronounced auxetic effect as the radius increases. The cellular structure achieves its peak elastic modulus at a radius of  $R = 3.1 \mathrm{~mm}$ , while

maintaining stable auxeticity within the arc radius range from 2.9 to  $3.1\mathrm{mm}$ .

The radius size significantly impacts the specific elastic modulus and strength of the butterfly MHS. A larger arc radius allows for increased deformation space, enhancing the effective dispersion and absorption of energy during compression, which in turn improves elastic compressive behavior. However, excessively large arc radius can lead to localized buckling under compressive loads, compromising the overall structural integrity. Therefore, it is crucial to determine an appropriate arc radius to optimize the trade-off between energy absorption capacity and the prevention of local buckling.

# 5.2. Cell height

Fig. 13(a) and (b) illustrate the impact of cell height  $(a = 4.1 - 5.9\mathrm{mm})$  on the specific elastic moduli, with other parameters held constant. Unlike the effects observed with arc radius variations, all specific elastic moduli — except for the 3-directional Young's modulus — decrease as cell height increases. This decline can be attributed to the increased spacing between honeycomb cells that transmit compressive stress,

![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/744ca051cb15f03e98969bbef8f4039eca29bce128e0422623dae6e341e43cab.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/cdd522ed4cf803256aa545b0be0544043c591d7ed16ae663a051ba4b79d7df81.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/4df0a2b595920dc815b03914ac825dadd5c2b44beebd968a186ec0f6ae7ca59a.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/2d564d3215bccef5ee86afe1dcaeced553bcfd3f2807a1aca850fa2e3e9fafc4.jpg)



Fig. 13. Effect of cell height  $a$  on (a) specific elastic modulus  $E_{i} / \rho^{*}$ , (b) specific shear modulus  $G_{ij} / \rho^{*}$ , (c) compressive displacement  $U_{i}$ , and (d) Poisson's ratio  $\nu_{12}$  of the butterfly MHS.


resulting in greater deformation of the cellular structure under uniform compressive loading. Fig. 13(c) and (d) reveal that both compressive displacement and Poisson's ratio of the butterfly MHS increase with cell height, indicating that cell height plays a crucial role in regulating the extent of structural deformation.

The variation in the cell height can significantly influence the specific elastic moduli and strength of the butterfly MHS. A higher honeycomb cell offers a larger support area, enhancing bending resistance under compressive loads. Additionally, the energy absorption capacity prior to plastic deformation increases with greater cell height. However, excessive cell height may lead to local buckling. Therefore, optimal height design is crucial for amplifying the auxetic effect, resulting in more pronounced lateral contraction during compression.

# 5.3. Strut thickness

Fig. 14(a) and (b) illustrate the effect of strut thickness  $(t = 0.08 - 0.32$  mm) on the specific elastic moduli of the butterfly MHS, while keeping other parameters constant. All specific moduli exhibit an increasing trend with greater strut thickness, indicating that heightened strut thickness enhances the specific elastic and load-bearing capacity of the butterfly MHS. Fig. 14(c) demonstrates that as strut thickness increases, the elastic compressive displacement of butterfly MHS decreases, promoting greater structural stability. Moreover, Fig. 14(d) displays a decreasing trend in Poisson's ratio with increasing strut thickness, signifying that thicker struts help reduce lateral contraction during compressive loading.

Greater strut thickness implies a higher load-bearing capacity per unit area, allowing to withstand increased compressive load. Increasing the strut thickness helps enhance the specific elastic moduli and stability of MHS configurations, mitigating the risks of buckling and instability during compression. However, greater strut thickness also adds to the overall weight of the cellular structure, which can conflict with the lightweight design. Therefore, it is crucial to strike a balance between enhancing specific elastic moduli and maintaining structural lightweight. Thicker struts may require more materials and complex manufacturing processes, resulting in increased production costs. Consequently, factors such as manufacturing capabilities and costs should also be considered when selecting strut thickness. The fluctuations in Figs. 12-14, attributed to local stress concentrations at critical junctions, can be mitigated by mesh refinement in these areas. The overall trends remain consistent, aligning with the structure's expected compressive behavior under varying parameters.

# 5.4. Summary of parameter analysis

Fig. 15 illustrates the effects of varying parameters on the elastic compressive behavior of butterfly MHS. Increasing the arc radius  $(R)$  significantly enhances its specific elastic modulus  $(E_{1})$ , specific shear modulus  $(G_{13})$ , and auxetic effect. Notably, a  $100\%$  increase in  $R$  leads to a  $220\%$  increase in  $E_{1}$ , a  $266\%$  increase in  $G_{13}$ , and a  $112\%$  increase in Poisson's ratio. This increase in specific elastic modulus corresponds to a reduction in compressive displacement of butterfly MHS.


(a)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/33481fd9844cbf42a5ea2584c42982545a04ab3947a679dfbe3712ae71ad8307.jpg)



(b)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/2b8183a14c10cee7a534f3c31bf69811c4862cc4d983af949ba08c9579f70371.jpg)



(c)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/83ceeed41154193ca03ca685e6efe299ad8cf2516d898d507cfe6eb758d83a5c.jpg)



(d)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/37c71a0285d1efdaa7b2e6d4886a26becd202fe033c1def922b4119f8c583efb.jpg)



Fig. 14. Effect of strut thickness  $t$  on (a) specific elastic modulus  $E_{i} / \rho^{*}$ , (b) specific shear modulus  $G_{ij} / \rho^{*}$ , (c) compressive displacement  $U_{i}$ , and (d) Poisson's ratio  $\nu_{12}$  of the butterfly MHS.


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/218f176398bc11854a8abeccd00c066c3cd0e93c822f4be11646e013ddf069c5.jpg)



Fig. 15. Effects of different parameters on equivalent properties and compressive displacements of butterfly MHS under uni-axial compression.



(a)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/7fb6a26b4f09ba367e28bffbbbf9914a281832406d9fa70658ff02dd475c9908.jpg)



(b)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/f7e76d636754ca0a63a2e32fa2e2cdf20696af198f88948ee4bbffb804478f5a.jpg)



Fig. 16. Geometries of (a) hexagonal MHS and (b) re-entrant MHS and their unit cell.



(a)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/e7f2bac44b292293ca7c149f2f0316d35e74c7c001cee88121de97f318e8bf72.jpg)



(b)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/45e87ef992f35f1fb6c73a9c080d65130a23ccc225e031878c68d8983dba7fc8.jpg)



Fig. 17. Comparison of (a) specific elastic moduli and (b) specific shear moduli for three MHS configurations.


Conversely, increasing the cell height  $(a)$  results in a decrease in the specific elastic moduli of butterfly MHS, reducing its deformation-resistance. The compressive displacement  $(u_{2})$  shows the most significant increase within this range. Additionally, while increasing strut thickness  $(t)$  has a notable impact on the specific elastic modulus  $(E_{2})$  and specific shear modulus  $(G_{12})$ , its effect on the compressive displacement of butterfly MHS is minimal. This is due to the minimal influence of strut thickness on the overall geometry of butterfly MHS, in contrast to the more pronounced effects of radius and cell height, which result in substantial changes to the stress state.

# 6. Comparison of different MHS configurations

The design of the butterfly-shaped honeycomb originates from the re-entrant auxetic honeycomb, which itself evolved from traditional hexagonal honeycombs. This section primarily examines the differences in elastic compression performance between butterfly MHS, re-entrant

MHS, and non-auxetic hexagonal MHS. The dimensions of the two MHS configurations are illustrated in Fig. 16, with  $l_{2}$ ,  $t_{c}$ , and  $\theta$  set to  $10\mathrm{mm}$ ,  $1\mathrm{mm}$ , and  $30^{\circ}$ , respectively. To ensure a fair comparison, the hexagonal MHS is set to a length of  $l_{1} = 10\mathrm{mm}$ , while the re-entrant MHS configured with a length of  $l_{1} = 20\mathrm{mm}$ .

# 6.1. Specific modulus

Fig. 17 compares the specific elastic moduli of three MHS configurations. Fig. 17(a), shows that the specific elastic modulus  $E_{3} / \rho^{*}$  for three MHS configurations is roughly equal due to their similar dimensions, with differences occurring primarily in the 1- and 2-directions, leading to comparable Young's modulus values in the 3-direction. Both the  $E_{1} / \rho^{*}$  and  $E_{2} / \rho^{*}$  values for the re-entrant MHS and butterfly MHS are greater than those for the hexagonal MHS, indicating that the auxetic configurations exhibit enhanced resistance to uniaxial compressive loads in these directions. Furthermore, the  $E_{1} / \rho^{*}$  and  $E_{2} / \rho^{*}$  values for

![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/cec6c963b251fc5121a768b9ead88d622cebb43bd6e32dbb7e43d048c55e9d11.jpg)



Fig. 18. Comparison of compressive displacement and Poisson's ratio of different MHS configurations at their elastic limit.


the butterfly MHS surpass those of the re-entrant MHS, demonstrating that the proposed MHS outperforms the re-entrant MHS in terms of elastic compressive behavior.

Fig. 17(b) illustrates that, with the exception of  $G_{23} / \rho^{*}$  remaining consistent, both  $G_{12} / \rho^{*}$  and  $G_{13} / \rho^{*}$  of butterfly and re-entrant MHS are lower than those of hexagonal MHS, which may arise from the structural anisotropy and the auxetic deformation mode of auxetic MHS. The lower specific shear modulus, particularly in the 1-2 and 1-3 planes, indicates localized weaknesses that could exacerbate shear deformation under critical loading conditions. However, the butterfly MHS demonstrates higher specific shear modulus compared to the re-entrant MHS, showcasing improved shear resistance among auxetic configurations. To mitigate the risk of failure, increasing strut thickness and optimizing the arc radius are recommended.

# 6.2. Compressive displacement and Poisson's ratio

Fig. 18 compares the compressive displacement and Poisson's ratio of different MHS configurations at their elastic limit. The results indicate that both re-entrant MHS and butterfly MHS exhibit larger deformations compared to hexagonal MHS, demonstrating that the auxetic multi-cellular structures can absorb and dissipate more energy

under compressive loads. Furthermore, the auxetic effect facilitates energy dispersion, allowing for greater displacements that help distribute compressive energy more effectively, thereby preventing localized failures and reducing the risk of stress concentration. As a result, the auxetic MHS showcases superior compressive behavior compared to the non-auxetic configuration. Additionally, the butterfly MHS experiences greater compressive displacement than the re-entrant MHS, suggesting enhanced compressive behavior. Notably, the lower Poisson's ratio of butterfly MHS compared to re-entrant MHS indicates reduced transverse deformation under applied compression, suggesting a weaker anisotropic response to external loading.

# 6.3. Strain energy

Fig. 19 shows the strain energy and equivalent strain energy  $(\mathrm{SE} / \mathrm{m})$  of three MHS configurations, as well as the proportions of specific strain energy components  $(SE_{11}, SE_{22}, SE_{12})$ . Fig. 19(a) illustrates that auxetic MHS (re-entrant and butterfly MHS) exhibit a notable advantage in energy absorption over non-auxetic MHS (hexagonal MHS), aligning with previously analyzed energy-absorbing characteristics of auxetic structures. Compared to hexagonal MHS, the total strain energy of the butterfly MHS increased by  $61.1\%$ , indicating the superior compressive energy absorption of auxetic MHS. In addition, the total strain energy of butterfly MHS increased by  $16.9\%$  over hexagonal MHS, indicating that the butterfly-shaped inclined strut configuration enhances elastic compressive behavior. The equivalent strain energy of re-entrant MHS is  $3.77\%$  higher than that of hexagonal MHS, while the equivalent strain energy of butterfly MHS is  $31.9\%$  higher than that of re-entrant MHS. This significant improvement in equivalent strain energy highlights the butterfly MHS as an optimized auxetic structure that combines lightweight design with high strength.

Fig. 19(b) illustrates that the strain energy components of the butterfly MHS surpass those of the other MHS configurations. The balanced proportion of  $SE_{11}$  in butterfly MHS indicates its strong capacity to limit lateral expansion under compression, thus reducing structural instability risks. Furthermore, the butterfly MHS has a moderate  $SE_{11}$  proportion with higher absolute values than the re-entrant MHS, showcasing its enhanced energy absorption efficiency and distinctive energy dissipation characteristics. In addition, the butterfly MHS exhibits a higher proportion of  $SE_{22}$ , indicating an enhanced energy absorption capacity in the loading direction and underscoring its superior compressive behavior.

![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/67032c04eff009ce56fe759730fc8b1e0039adc9dcb4c0d7ec1b5878214bfd72.jpg)


![](file://D:/MinerU/转换结果/153.pdf-37f09c58-c9ab-4946-96e9-b83888e9bc04/images/50367539bffd6e3f8a1b93e1b3d81c62daffe86429ee0d4bc560ea96ce65c3a0.jpg)



Fig. 19. Comparison of (a) strain energy and equivalent strain energy, and (b) strain energy component and their proportions, for three MHS configurations.


# 7. Conclusions

This study develops an equivalent Cauchy model (3D-ECM) for a butterfly-shaped multi-cellular honeycomb structure (butterfly MHS) using the variational asymptotic method. By comparing the elastic compression behavior, strain energy, and local field distribution obtained from 3D finite element analysis, the model's accuracy is confirmed. In addition, uniaxial compressive tests on 3D-printed specimens validate the model experimentally. Parametric studies elucidate the influence of arc radius, cell height, and strut thickness on specific elastic moduli, compressive displacement, and Poisson's ratio. Furthermore, the elastic compressive behaviors of different MHS configurations are compared. The following conclusions can be drawn:

The equivalent model demonstrates reliable accuracy in predicting the compressive displacement mode, total strain energy, and individual strain energy components of butterfly MHS. The compressive modes predicted by 3D-ECM and 3D-FEM are basically consistent, with a relative error in compression displacement of less than  $5\%$ . Furthermore, the equivalent model effectively captures detailed local stresses, strains, and displacements within the unit cell, maintaining errors within  $8.67\%$ . The analysis of strain energy components shows that SE22 is the primary contributor to significant transverse contraction, while SE12 reflects notable auxetic deformation in the 1-2 plane. Notably, the 3D-ECM significantly reduces the number of elements and model complexity, enhancing computational efficiency without compromising accuracy.

Increasing the arc radius in the butterfly MHS enhances the auxetic effect, which improves the structure's overall compressive behavior. Similarly, increasing the cell height raises the porosity of the butterfly MHS, further amplifying the auxetic effect and increasing structural displacement; however, this change may reduce the specific moduli of the honeycomb structure. In contrast, variations in strut thickness strongly influence specific moduli, with thicker struts improving the structure's load-bearing capacity. Compared to hexagonal and re-entrant MHS, the butterfly MHS exhibits superior specific moduli, compressive displacement capacity, Poisson's ratio, and strain energy, underscoring its optimized structural and mechanical performance.

This study primarily focuses on the quasi-static compressive behavior of butterfly MHS to establish baseline insights into their energy absorption and elastic deformation characteristics. Future work should include dynamic testing and simulations to assess the effects of impact velocity, deformation rate, and inertial forces. Moreover, future studies could examine the buckling and post-buckling behavior of butterfly MHS under combined compressive and shear loading.

# CRediT authorship contribution statement

Zhong Yifeng: Methodology, Investigation. Liu Rong: Validation, Software. Poh Leong Hien: Supervision, Resources. Liu Xiaoquan: Writing - original draft, Validation. Tang Yuxin: Resources, Methodology.

# Declaration of competing interest

The authors declare that they have no known competing financial interests or personal relationships that could have appeared to influence the work reported in this paper.

# Acknowledgments

The work described in this paper is financially supported by the National Natural Science Foundation of China (52073036).

# Appendix A. Supplementary data

Supplementary material related to this article can be found online at https://doi.org/10.1016/j.istruc.2025.108765.

# References



[1] Zhang X, Tian R, Zhang Z, et al. In-plane elasticity of a novel vertical strut combined re-entrant honeycomb structure with negative Poisson's ratio. Thin-Walled Struct 2021;163:107634.





[2] Qin S, Deng X, Yang F, et al. Energy absorption characteristics and negative Poisson's ratio effect of axisymmetric tetrachiral honeycombs under in-plane impact. Compos Struct 2023;323:117493.





[3] Shukla S, Behera BK. Auxetic fibrous structures and their composites: A review. Compos Struct 2022;290:115530.





[4] Tian L, Yang J, You X, et al. Tailoring centripetal metamaterial with superelasticity and negative Poisson's ratio for organic solvents adsorption. Sci Adv 2022;8(39):1014.





[5] Zhang M, Hu H, Kamrul H, et al. Three-dimensional composites with nearly isotropic negative Poisson's ratio by random inclusions: Experiments and finite element simulation. Compos Sci Technol 2022;218:109195.





[6] Li D, Shen G. Study on mechanical properties of an isotropic negative Poisson's ratio voronoi foam and its foam-filled tube. Smart Mater Struct 2022;31(6):065017.





[7] Li Y, Li Z, Wang Q, et al. 3D-printed magnetic porous structures with different Poisson's ratios and their mechanelectrical conversion capabilities. Addit Manuf 2023;69:103542.





[8] Harinarayana V, Shin YC. Design and evaluation of three-dimensional axisymmetric mechanical metamaterial exhibiting negative Poisson's ratio. J Mater Res Technol 2022;19:1390-406.





[9] Zhao Y, Deng X, Zheng S, et al. Study on quasi-static axial compression performances and energy absorption of four-star double arrow honeycomb. Compos Struct 2023;311:116816.





[10] Zhang T, Huang Z, Li Y, et al. Compressive mechanical behaviors of PPR and NPR chiral compression-twist coupling lattice structures under quasi-static and dynamic loads. Thin-Walled Struct 2023;182:110234.





[11] Li T, Chen Y, Hu X, et al. Exploiting negative Poisson's ratio to design 3D-printed composites with enhanced mechanical properties. Mater Des 2018;142:247-58.





[12] Wang Z. Recent advances in novel metallic honeycomb structure. Compos Part B: Eng 2019;166:731-41.





[13] Xu F, Yu K, Hua L. In-plane dynamic response and multi-objective optimization of negative Poisson's ratio (NPR) honeycomb structures with sinusoidal curve. Compos Struct 2021;269:114018.





[14] Govindaraman LT, Arjunan A, Baroutaji A, et al. Metamaterials for energy harvesting. Encycl Smart Mater 2022;2:522-34.





[15] Le DH, Novak N, Arjunan A, et al. Crashworthiness of bio-inspired multi-stage nested multi-cell structures with foam core. Thin-Walled Struct 2023;182:110245.





[16] Deng X, Qin S. In-plane energy absorption characteristics and mechanical properties of novel re-entrant honeycombs. Compos Struct 2023;313:116951.





[17] Xue X, Lin C, Wu F, et al. Lattice structures with negative Poisson's ratio: A review. Mater Today Commun 2023;34:105132.





[18] Fu MH, Xu OT, Hu LL, et al. Nonlinear shear modulus of re-entrant hexagonal honeycombs under large deformation. Int J Solids Struct 2016;80:284-96.





[19] Li X, Li Z, Guo Z, et al. A novel star-shaped honeycomb with enhanced energy absorption. Compos Struct 2023;309:116716.





[20] Gao Q, Wang L, Zhou Z, et al. Theoretical, numerical and experimental analysis of three-dimensional double-v honeycomb. Mater Des 2018;139:380-91.





[21] Bohara RP, Linforth S, Nguyen T, et al. Anti-blast and-impact performances of auxetic structures: A review of structures, materials, methods, and fabrications. Eng Struct 2023;276:115377.





[22] Momoh EO, Jayasinghe A, Hajsadeghi M, et al. A state-of-the-art review on the application of auxetic materials in cementitious composites. Thin-Walled Struct 2024;196:111447.





[23] Alomarah A, Masood SH, Ruan D. Out-of-plane and in-plane compression of additively manufactured auxetic structures. Aerosp Sci Technol 2020;106:106107.





[24] Zhang X, Hao H, Tian R, et al. Quasi-static compression and dynamic crushing behaviors of novel hybrid re-entrant auxetic metamaterials with enhanced energy-absorption. Compos Struct 2022;288:115399.





[25] Wang H, Lu Z, Yang Z, et al. A novel re-entrant auxetic honeycomb with enhanced in-plane impact resistance. Compos Struct 2019;208:758-70.





[26] Wang H, Lu Z, Yang Z, et al. In-plane dynamic crushing behaviors of a novel auxetic honeycomb with two plateau stress regions. Int J Mech Sci 2019;151:746-59.





[27] Xu M, Liu D, Wang P, et al. In-plane compression behavior of hybrid honeycomb metastructures: Theoretical and experimental studies. Aerosp Sci Technol 2020;106:106081.





[28] Peng XL, Bargmann S. A novel hybrid-honeycomb structure: Enhanced stiffness, tunable auxeticity and negative thermal expansion. Int J Mech Sci 2021;190:106021.





[29] Pan J, Zhang Q, Li M, et al. A novel misplaced reinforced honeycomb with in-plane bidirectional enhancement. Int J Mech Sci 2024;270:109088.





[30] Zhang S, Yang F, Li P, et al. A topologically gradient body centered lattice design with enhanced stiffness and energy absorption properties. Eng Struct 2022;263:114384.





[31] Suzuki M, Nagasawa H. Mollusk shell structures and their formation mechanism. Can J Zool 2013;91(6):349-66.





[32] Gilbert SF, Loredo GA, Brukman A, et al. Morphogenesis of the turtle shell: the development of a novel structure in tetrapod evolution. Evol Dev 2001;3(2):47-58.





[33] Wu Y, Liu Q, Fu J, et al. Dynamic crash responses of bio-inspired aluminum honeycomb sandwich structures with CFRP panels. Compos Part B: Eng 2017;121:122-33.





[34] Qi C, Jiang F, Yang S. Advanced honeycomb designs for improving mechanical properties: A review. Compos Part B: Eng 2021;227:109393.





[35] Ha NSan, Pham TM, Tran TT, et al. Mechanical properties and energy absorption of bio-inspired hierarchical circular honeycomb. Compos Part B: Eng 2022;236:109818.





[36] Wang M, Wu H, Yang L, et al. Structure design of arc-shaped auxetic metamaterials with tunable Poisson's ratio. Mech Adv Mater Struct 2023;30(7):1426-36.





[37] Sindelic V, Nikolic A, Minak G, et al. An improved 2D arc-star-shaped structure with negative Poisson's ratio: In-plane analysis. Mater Today Commun 2023;37:107593.





[38] Shen J, Ge J, Gao J, et al. In-plane impact dynamics of honeycomb structure containing curved reentrant sides with negative Poisson's ratio effect. Mech Adv Mater Struct 2022;29(10):1489-97.





[39] Qi C, Jiang F, Yang S, et al. Dynamic crushing response of novel re-entrant circular auxetic honeycombs: Numerical simulation and theoretical analysis. Aerosp Sci Technol 2022;124:107548.





[40] Qi C, Jiang F, Yang S, et al. Multi-scale characterization of novel re-entrant circular auxetic honeycombs under quasi-static crushing. Thin-Walled Struct 2021;169:108314.





[41] Zhang X, An C, Shen Z, et al. Dynamic crushing responses of bio-inspired re-entrant auxetic honeycombs under in-plane impact loading. Mater Today Commun 2020;23:100918.





[42] Yan ZG, Wang BL, Wang KF, et al. A novel cellular substrate for flexible electronics with negative Poisson ratios under large stretching. Int J Mech Sci 2019;151:314-21.





[43] Tatlier MS, Öztürk M, Baran T. Linear and non-linear in-plane behaviour of a modified re-entrant core cell. Eng Struct 2021;234:111984.





[44] Chen C, Airoldi A, Caporale AM, et al. Impact response of composite energy absorbers based on foam-filled metallic and polymeric auxetic frames. Compos Struct 2024;331:117916.





[45] Qi C, Jiang F, Remennikov A, et al. Quasi-static crushing behavior of novel re-entrant circular auxetic honeycombs. Compos Part B: Eng 2020;197:108117.





[46] Zhu D, Wei Y, Shen X, et al. A novel elliptical annular re-entrant auxetic honeycomb with enhanced stiffness. Int J Mech Sci 2024;262:108732.





[47] Xu F, Yu K, Hua L. In-plane dynamic response and multi-objective optimization of negative Poisson's ratio (NPR) cellular honeycombs with sinusoidal curve. Compos Struct 2021;269:114018.





[48] Usta F, Scarpa F, Turkmen HS. Edgewise compression of novel hexagonal hierarchical and asymmetric unit cells honeycomb metamaterials. Mater Today Commun 2020;24:101102.





[49] Wang S, Deng C, Ojo O, et al. Design and modeling of a novel three dimensional auxetic reentrant honeycomb structure for energy absorption. Compos Struct 2022;280:114882.





[50] Du J, Hao P, Li L. Finite element analysis of energy absorption characteristics for biomimetic thin-walled multi-cellular structure inspired by horsetails. Mech Adv Mater Struct 2022;29(27):6982-93.





[51] Tejavibulya N, Youssef J, Bao B, et al. Directed self-assembly of large scaffold-free multi-cellular honeycombs. Biofabrication 2011;3(3):034110.





[52] Jewell E, Allen MS, Zare I, et al. Application of quasi-static modal analysis to a finite element model and experimental correlation. J Sound Vib 2020;479:115376.





[53] Xue Z, Hutchinson JW. Constitutive model for quasi-static deformation of metallic sandwich cores. Internat J Numer Methods Engrg 2004;61(13):2205-38.





[54] Ashab ASM, Ruan D, Lu G, et al. Experimental investigation of the mechanical behavior of aluminum honeycombs under quasi-static and dynamic indentation. Mater Des 2015;74:138-49.





[55] Sun G, Huo X, Chen D, et al. Experimental and numerical study on honeycomb sandwich panels under bending and in-panel compression. Mater Des 2017;133:154-68.





[56] Zhao C, Goh KL, Lee HP, et al. Experimental study and finite element analysis on energy absorption of carbon fiber reinforced composite auxetic structures filled with aluminum foam. Compos Struct 2023;303:116319.





[57] Wang S, Deng C, Ojo O, et al. Design and modeling of a novel three dimensional auxetic reentrant honeycomb structure for energy absorption. Compos Struct 2022;280:114882.





[58] Chen S, Tan X, Hu J, et al. A novel gradient negative stiffness honeycomb for recoverable energy absorption. Compos Part B: Eng 2021;215:108745.





[59] Rong L, Yifeng Z, Siqi M, et al. Dynamic characteristics of sandwich panels with novel improved star-shaped honeycomb. Int J Mech Sci 2023;260:108641.





[60] Xinyi L, Yifeng Z, Rong L, et al. Static and global buckling analysis of sandwich panels with improved star-shaped honeycomb using VAM-based downscaling model. Compos Struct 2023;323:117458.





[61] Yu W, Volovoi VV, Hodges DH, et al. Validation of the variational asymptotic beam sectional analysis. AIAA J 2002;40(10):2105-12.





[62] Srivastava C, Mahesh V, Pitchai P, et al. Effective mechanical properties of auxetic materials: Numerical predictions using variational asymptotic method based homogenization. J Appl Mech 2023;90(11):111001.





[63] Zhang L, Yu W. Variational asymptotic homogenization of elastoplastic composites. Compos Struct 2015;133:947-58.





[64] Shi Z, Zhong Y, Yi Q, et al. High efficiency analysis model for composite honeycomb sandwich plate by using variational asymptotic method. Thin-Walled Struct 2021;163:107709.





[65] Yuheng C, Chunyu Z, Biao W. A new high-order deformation theory and solution procedure based on homogenized strain energy density. Internat J Engrg Sci 2024;195:103990.





[66] Pagani A, Zappino E, Bracaglia F, et al. Thermal stress analysis of variable angle tow composite plates through high-order structural models. Compos Struct 2024;327:117668.





[67] Zhang Y, Si J. A model for laminated composite beams based on a novel zig-zag theory. Mech Adv Mater Struct 2024;1-11.





[68] Zoghipour P, Kefal A, Yildiz M. Structural analysis of sandwich plates with variable stiffness composite skins and functionally graded cores using refined zig-zag theory. Mech Adv Mater Struct 2024;1-25.





[69] Boisse P, Hamila N, Madeo A. The difficulties in modeling the mechanical behavior of textile composite reinforcements with standard continuum mechanics of Cauchy. Some possible remedies. Int J Solids Struct 2018;154:55-65.





[70] Hütter G. Homogenization of a Cauchy continuum towards a micromorphic continuum. J Mech Phys Solids 2017;99:394-408.





[71] Zhang ZW, Tian RL, Zhang XL, et al. A novel butterfly-shaped auxetic structure with negative Poisson's ratio and enhanced stiffness. J Mater Sci 2021;56(25):14139-56.





[72] Rao E, Fu T. Acoustic radiation response of functionally graded sandwich plates cored by butterfly-shaped honeycombs with negative Poisson's ratio. J Mech Sci Technol 2024;1-13.

