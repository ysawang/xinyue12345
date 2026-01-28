# A novel 3D printed self-similar hierarchical re-entrant honeycomb with enhanced energy absorption and shape recoverability

![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/9849953fa808aaa7259a212c8bf40c4609df349ee115057f7662b65f9c3ee7f5.jpg)


Pengxu Lu a, Jin Zhou a,\*, Hui Liu a, Chunqi Liu a, Hui Li b,\*, Yue Xing c, Xiubing Liang c, Zhongwei Guan a,d, b, Wesley J. Cantwell e

$^{a}$  State Key Laboratory for Manufacturing Systems Engineering, School of Mechanical Engineering, Xi'an Jiaotong University, Xi'an 710049, China

$^{b}$  School of Mechanical Engineering and Automation, Northeastern University, Shenyang 110819, China

$^{c}$  National Innovation Institute of Defence Technology, Academy of Military Sciences, Beijing 100071, China

$^{d}$  School of Mechanical Engineering, Chengdu University, Chengdu 610106, China

$^{e}$  Department of Aerospace Engineering, Khalifa University of Science and Technology, Abu Dhabi, UAE

# ARTICLEINFO

# Keywords:

Hierarchical re-entrant honeycombs

Negative Poisson's ratio

Lattice filling density

In-plane crushing

Energy absorption

Shape recoverability

# ABSTRACT

This paper introduces a self-similar hierarchical design and lattice filling density process for regular re-entrant (R-Re) honeycombs. Two categories of honeycomb are considered, one with a low lattice filling density (L-Re) and the other with a high one (H-Re). Here, the stress response and energy absorption responses of re-entrant honeycombs are obtained by conducting a series of quasi-static compression tests. The mechanical behavior is subsequently predicted by the finite element simulations. The results show that the stress, specific energy absorption and mean crushing force values of the H-Re honeycombs are two to six times higher than those of their L-Re and R-Re counterparts. In particular, the H-Re honeycomb exhibits pronounced structural recoverability after testing. Following unloading, the H-Re structure can rapidly recover up to  $75\%$  of its original height, and its original height after 6 hours under room temperature conditions. In addition, parametric analyses have been developed to study the effect of lattice filling density on energy absorption, as well as the influence of the representative volume element distribution and relative density on the crashworthiness and failure modes. The results of this study can be used to identify the factors that affect the energy-absorbing characteristics of re-entrant honeycombs and facilitate the design of the next generation of complex hierarchical structures.

# 1. Introduction

Honeycomb structures have been widely used in the defense, aerospace, civil engineering and energy-generating industries, as well as other engineering fields, due to their light weight, high specific stiffness/ strength, exceptionally high energy absorption as well as superior fracture toughness [1-3]. In recent decades, extensive research has been undertaken on investigating the crashworthiness of honeycomb structures. Wierzbicki [4] proposed theoretical models to describe energy absorption in hexagonal honeycombs subjected to out-of-plane loading and found that the crashworthiness of a honeycomb is strongly dependent on the cell-wall thickness. Based on their experiments and analyses, Papka and Kyriakides [5] investigated the load-displacement response of hexagonal honeycombs and the deformation behavior during the in-plane compression. Wu and Jiang [6] performed quasi-static and dynamic experiments on six types of hexagonal honeycomb structure to

study their crashworthiness over a range of strain-rates. Ruan et al. [7] and Aktay et al. [8] undertook numerical simulations to study the in-plane compressive behavior of hexagonal honeycomb structures.

Following Gibson et al. [9] and Lakes' [10] work on designing and manufacturing negative Poisson's ratio structures, researchers began to focus on honeycombs exhibiting negative Poisson's ratio characteristics, such as the auxetic re-entrant honeycombs [11]. Liu et al. [12] studied the in-plane dynamic crushing behavior of re-entrant honeycombs by the finite element analysis (FEA). Their results showed that the incident impact velocity significantly affected the energy-absorbing capacity of the re-entrant honeycombs. Xiao et al. [13] and Dong et al. [14] investigated the quasi-static compression behavior of re-entrant honeycombs based on different cell-wall thicknesses, and elucidated the effect of cell-wall thickness on collapse modes through both experiments and simulations. Zhang and Lu [15] compared the energy-absorbing processes of re-entrant honeycombs during tension and compression,

finding that the advantages of re-entrant honeycombs can be fully leveraged in energy-dissipating applications dominated by tensile forces. Li et al. [16] proposed a ribbed star-shaped diamond honeycomb structure, which exhibited a  $136\%$  and  $75\%$  increase in specific energy absorption compared to re-entrant and star-shaped honeycomb structures, respectively. This indicates that the introduction of ribs effectively enhances both load-bearing capacity and energy-absorbing performance. Etemadi et al. [17] combined re-entrant honeycombs with S-shaped, star-shaped and petal-shaped auxiliary structures, enriching the innovative design of negative Poisson's ratio honeycombs. Through testing and finite element validation, the petal-shaped re-entrant honeycomb demonstrated the highest energy-absorbing efficiency.

In recent years, with the greater interest in light-weight materials and cellular structures, hierarchical structures have attracted significant attention for use in energy-absorbing honeycomb structures [18,19]. Chen and Pugno [20] derived the buckling stress - strain response of hierarchical honeycombs with different filling levels in the lattice cell wall, and found that increasing the filling level decreases the energy density and increases the specific energy absorption. Based on Euler beam theory, Sun et al. [21,22] analyzed the influence of negative Poisson's ratio sub-structures on the in-plane stiffness of multifunctional hierarchical honeycombs. Qiao and Chen [23] derived analytical expressions of the quasi-static compressive stress for hierarchical honeycombs by employing a two-scale method. Zhang et al. [24] conducted numerical simulations on the out-of-plane dynamic crushing response of self-similar regular hexagonal hierarchical honeycombs and showed that increasing the hierarchical order significantly enhanced their crashworthiness characteristics. Chen et al. [25] and Yin et al. [26] developed a set of hierarchical honeycomb structures by substituting the cell walls of regular honeycombs with hexagonal, Kagome and triangular lattices. Following analytical and numerical analyses, they confirmed that hierarchical honeycombs based on Kagome and triangular lattices exhibited superior in-plane crushing energy absorption characteristics compared to their hexagonal counterparts. Based on a simplified super folding element method, Fang et al. [27] derived theoretical expressions for the mean force and plateau stress of hierarchical honeycombs subjected to out-of-plane crushing. Chen et al. [28] introduced triangular lattices into the cell walls of regular honeycombs, and investigated their in-plane crushing behavior. It was found that slender lattices can significantly enhance both the energy absorption and the overall recoverability. Liu et al. [29] developed a novel graded hierarchical honeycomb by varying the sub-cell into different layers, and analyzed the deformation mode and crashworthiness performance of positively and negatively graded hierarchical honeycombs. Tan et al. [30] studied the in-plane crushing behavior of re-entrant hierarchical honeycombs, and concluded that such honeycombs exhibited superior crashworthiness characteristics compared to regular re-entrant honeycombs. Tan et al. [31] developed re-entrant hierarchical honeycomb sandwich panels with different orientations and investigated how such designs impacted the energy-absorbing behavior of these panels. Xue et al. [32] used a non-dominated sorting genetic algorithm-II (NSGA-II) to design the optimal configuration and enhance the energy absorption of re-entrant hierarchical honeycomb sandwich beams. Zhan et al. [33] identified the relationship between the observed deformation mode and the relative density of re-entrant hierarchical honeycombs through a combination of DIC analysis and numerical simulations. Tan et al. [34] proposed a novel re-entrant hierarchical crash absorber and subsequently compared its crashworthiness against both aluminum foam-filled and traditional crash box structures. Their results showed that the energy absorption capability of the re-entrant hierarchical crash box was superior to that of its conventional counterpart. Usta et al. [35] presented a novel hierarchical configuration based on hexachiral auxetic cells. Experimental results showed that the proposed structure offered a higher specific energy absorption and specific compressive strength.

To date, the published literature has largely focused on the crashworthiness of both auxetic structures and hierarchical honeycombs.

However, a systematic investigation of the effect of lattice distribution in hierarchical re-entrant honeycombs remains limited. In the present study, unique self-similar lattice fillings are introduced into hierarchical re-entrant honeycombs and subjected to compression testing in order to characterize their energy-absorbing characteristics. Finite element modelling is then undertaken to accurately simulate their elastoplastic and damage performance. The model is then used to undertake a parametric study to investigate the influence of lattice distribution parameters on crushing response. This research aims to propose design directions for a new generation of hierarchical auxetic energy-absorbing structures.

# 2. Materials and design

# 2.1. Design of geometric configuration

The hierarchical re-entrant honeycombs studied in this paper were designed by inserting self-similar lattices into the cell walls of regular re-entrant honeycombs (R-ReH), which consist of the horizontal cell wall  $(l_r)$  and the tilted cell wall  $(w_r)$  but do not contain any lattices. In the process of introducing self-similar lattices, the horizontal and inclined cell walls of each R-ReH adopt the same lattice filling method and maintain the same lattice filling density. Based on the lattice filling density, the hierarchical honeycombs are divided into two classes, these being low and high density hierarchical re-entrant honeycombs (L-ReH and H-ReH). Fig. 1(a) and (b) present the cross-section configurations of these honeycombs. Fig. 1(c) shows the specific construction of the horizontal cell walls with introduced self-similar lattices.

Three geometric parameters were investigated, these being the length of horizontal hierarchy framework ( $l_{l}$  and  $l_{h}$ ), the tilted hierarchy framework ( $w_{l}$  and  $w_{\mathrm{h}}$ ), and the lattice thickness ( $t_{l}$  and  $t_{h}$ ), as shown in Fig. 1(c). The angle between the horizontal and inclined lines in the ReHs was set to  $45^{\circ}$ , while that for the re-entrant lattices was fixed at  $75^{\circ}$ . The lattice filling density,  $R$ , represents the density of the re-entrant lattices filling within each cell wall, and is related to the aforementioned geometric parameters. For example, the geometric parameters for L-ReH ( $R = 1$ ) and H-ReH ( $R = 4$ ) have the following relationship:

$$
w _ {l} = 2 w _ {h} \tag {1}
$$

$$
l _ {l} = 2 l _ {h} \tag {2}
$$

The formulae shown above highlight that the size of the geometric parameters for the L-ReH structure is double that of the H-ReH structure. To maintain the rationality of the hierarchical structure, the heights of the framework  $(h_l$  and  $h_h)$  are maintained the same. With this in mind, it becomes clear that each re-entrant lattice (Cell #0) in L-ReH is replaced by four scaled-down re-entrant lattices (Cells #1 to #4) in H-ReH. It is worth noting that, upon the introduction of Cells #1 to #4, a re-entrant space (highlighted in pink) was automatically generated. This re-entrant space was formed by the cell walls of Cells #1 to #4, without the inclusion of any additional design elements. The formation of this space was strongly dependent on the presence of Cells #1 to #4 and was regarded as an additional component of the design. As a result, the lattice filling density of L-ReH is 1, whereas that of H-ReH is 4.

As a porous structure, ReHs features relative density as a crucial structural parameter for controlling its mass distribution. The relative density is calculated by the ratio of the actual volume of ReH to the total volume of the space it occupies [36]. To ensure accurate comparisons between the different configurations, it is important that the structures possess the same relative density. The expressions for the relative densities are as follows:

$$
\bar {\rho} _ {\mathrm {R} - \mathrm {R e H}} = \frac {\left(4 w _ {r} + 2 l _ {r} - \frac {2 t _ {r}}{\sin 4 5 ^ {\circ}} - \frac {t _ {r}}{\tan 4 5 ^ {\circ}}\right) t _ {r}}{\left(2 l _ {r} - 2 w _ {r} \cos 4 5 ^ {\circ} - \frac {3 t _ {r}}{\sin 4 5 ^ {\circ}}\right) \times \left(2 w _ {r} \sin 4 5 ^ {\circ} + t _ {r}\right)} \tag {3}
$$


(a)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/e5fcaeac5d622cfde3b2a9e280dc4b988a9f63781847c641f7028e49d07b42ad.jpg)



(b)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/4dc8c754f65ff5973e68c5ad2dcf4a5618cf5e6d1aeb73015e72dd32106415df.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/d74e19ed202c08de2afbff94100019915026dbdf4adc0a4634f3d5e497f4fa0c.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/4afd36a25423e7d0452d7896fc3ceaabfbaaf2042724e0aa557049c7987a69da.jpg)



(c)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/0ac1c57eaec46a1629614052daadb76dafcf2b1c1cf89f4eac0d85ff3e5ac9ff.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/c7298fc4a55ba42fd41bf88ea384b967f8e1dc3b05d8d18d9c7827d4da684d9d.jpg)



Fig. 1. The geometric illustrations and configurations of hierarchical ReHs. (a) R-ReH, L-ReH and H-ReH. (b) Representative volume elements of each ReH. (c) Cellular structures of each ReH cell wall.


$$
\bar {\rho} _ {\mathrm {L} - \mathrm {R e H}} = \frac {\left(9 2 w _ {l} + 1 6 0 l _ {l} - \frac {1 6 0 t _ {l}}{\sin 7 5 ^ {\circ}}\right) t _ {l}}{\left(2 2 l _ {l} - 2 4 w _ {l} \cos 7 5 ^ {\circ}\right) \times \left(1 4 w _ {l} \sin 7 5 ^ {\circ} + t _ {l}\right)} \tag {4}
$$

$$
\bar {\rho} _ {\mathrm {H} - \mathrm {R e H}} = \frac {\left(2 5 2 w _ {h} + 6 4 0 l _ {h} - \frac {6 4 0 t _ {h}}{\sin 7 5 ^ {\circ}}\right) t _ {h}}{\left(4 8 l _ {h} - 4 8 w _ {h} \cos 7 5 ^ {\circ}\right) \times \left(2 8 w _ {h} \sin 7 5 ^ {\circ} - t _ {h}\right)} \tag {5}
$$

where  $\overline{\rho}_{\mathrm{R - ReH}},\overline{\rho}_{\mathrm{L - ReH}}$  and  $\overline{\rho}_{\mathrm{H - ReH}}$  are the relative densities of the R-ReH, L-ReH and H-ReH, respectively.

# 2.2. Materials and sample preparation

All samples were printed using a Lite600HD 3D printer (Ningbo Zhechuang Technology Co., Ltd), with a positing precisions and layer resolution of  $0.05\mathrm{mm}$ . Samples were printed at a speed of  $20\mathrm{mm/s}$  with a layer height of  $0.1\mathrm{mm}$ . The polymer R4600 (an ABS-like resin), as shown in Fig. 2(e), was used for printing. After printing, the samples were washed in  $90\%$  isopropanol alcohol for approximately 10 minutes, dried, and subsequently post-cured using the Form Cure device. Finally, the support structures were removed, and the sample surfaces were polished to achieve the desired finish. As can be seen in Fig. 1(a), the ReH samples consist of  $2 \times 3$  representative volume elements (RVEs) with overall dimensions of  $160 \times 95 \times 40\mathrm{mm}$  (width  $\times$  height  $\times$  thickness). The samples were fabricated with the same printing orientation to ensure the same mechanical properties. In order to have a uniform compressive strain during testing, an additional connecting plate was printed on the upper and lower surfaces of the samples. All samples were printed with sufficiently thick walls to avoid out-of-plane buckling during the compressive tests. At least three test samples for each design were prepared and stored at room temperature for five days after printing to ensure the material being completely cured.

# 2.3. Mechanical testing

The mechanical properties of the R4600 material were obtained using a universal testing machine (WDM-100E, Jinan Chenda, Co., Ltd.)

by conducting uniaxial tensile tests (ASTM D638-14), uniaxial compressive tests (ASTM D695-15) and V-notched shear tests (ASTM D5379-12). The average stress-strain responses of the samples shown in Fig. 2(a)-(c) were calculated based on the relevant load-displacement data from three repeated tests, with the geometric dimensions of the samples being given in Fig. 2(d). It can be seen that the tensile and shear strengths of the material are significantly lower than the compressive strength.

# 3. Experimental testing and crashworthiness criteria

# 3.1. Quasi-static compressive tests

Quasi-static compression tests on the ReH samples were conducted by the WDM-100E universal testing machine and the crosshead displacement rate was set to  $1.5\mathrm{mm / min}$  [37]. The load-displacement data were measured to calculate the stress level and crashworthiness of the ReHs. The samples were subjected to uniaxial compression testing in the X- and Y-directions, as shown in Fig. 3. It is worth noting that samples tested in the Y-direction consist of  $3\times 2$  RVEs to avoid out-of-plane buckling. They have the same mass as the test samples loaded in the X-direction

# 3.2. Crashworthiness criteria

The initial peak stress corresponds to the initial compressive strength of the structure and is regarded as the onset of plastic deformation. Due to the excellent energy absorption characteristics, the initial peak stress of an auxetic structures is low [38]. Following the linear elastic deformation regime, continuous compressive loading will result in plastic deformation within the structures and show a plateau phase before final densification.

The energy absorption (EA) term employed here represents the total amount of energy absorbed during loading before final densification, which can be expressed as [39]:

$$
E A (x) = \int_ {0} ^ {l} F (x) d x \tag {6}
$$

![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/9dc8899c84efb7aacbd421e9a160aafa2303a81aa17606934bab12da3f2162cf.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/e986a9fe84b5daeaa88e02c911076ae2a3fdcb16db0ec2d50135dac7e3b4a47a.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/8d209d0f35a15744ac3878d0a5171b6647dc9de5363aa60295227c9dfb31bedb.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/050f4f3a4efea3d021e597b2bf8ecf9ece1d5165eef40aed137c5102109413f3.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/e7dc325e50de5d2f9b308d1c7960a68b555eaad6f38cd64fb55ac89a74608342.jpg)



Fig. 2. Stress-strain responses of R4600 material: (a) uniaxial tensile test, (b) uniaxial compressive test and (c) V-notched shear test; (d) geometric dimensions of tensile, compressive, and shear samples; (e) R4600 ABS-like resin.


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/f9150b79d7e276db79681ea9f91dae3d9db5bef65b35bb209bdc7c4f20342ca1.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/a89bc9b8b5e8ea2c9d9de2c83b137eb304162d2e56b29ff0fe59d1bb9fb00c69.jpg)



Fig. 3. Experimental loading in the (a) X-direction and (b) Y-direction for L-ReH as an example.


In Eq. (6), 1 denotes the total compressive displacement. The variable  $x$  indicates the compressive displacement, and  $F(x)$  is the corresponding compressive load. It is worth noting that a higher value of EA corresponds to a superior energy absorption capacity, while the specific energy absorption (SEA) can more reliably reflect the crashworthiness, which defines the energy absorption per unit mass and is given by [36]:

$$
S E A (x) = \frac {E A (x)}{m} \tag {7}
$$

where  $m$  is the mass of the structure.

The mean crushing force (MCF), which reflects the efficiency and stability of energy absorption, is defined as the average impact load

during the energy absorption process, and can be written as [40]:

$$
M C F (x) = \frac {E A (x)}{x} \tag {8}
$$

# 4. Numerical modelling and results discussion

# 4.1. Finite element modelling

The finite element (FE) models of the ReHs under quasi-static uniaxial compression were developed using Abaqus/CAE 2020. Compression samples were modeled between two rigid compression platens to represent the actual experimental conditions, shown in Fig. 4(a). The

![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/ed641191495a6cbe7e17bd4c3f4ad78377d19ec19694d2e35337ce46ad0988d5.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/8d048a6343d339e9449688713392c3f08f4b6cdce418f073ff4839c96719afb8.jpg)



Fig. 4. Loading and boundary conditions of ReH FE model: (a) X-direction compression of L-ReH and (b) L-ReH model meshed using C3D10M elements.


yield behavior of the R4600 polymer exhibits significantly differences in tension and compression, Fig. 2, thus the material constitutive behavior is described by a pressure-dependent plasticity model. The elastic and plastic behavior of the R4600 polymer was modeled by using an isotropic elasticity model and a linear Drucker-Prager plasticity model, respectively. The ductile damage model was selected for modelling material failure. The material properties used in the FE analysis are shown in Tables 1 and 2. These values were obtained from the mechanical tests shown in Fig. 2.

General contact and self-contact were considered in the FE modelling. Here, contact between rigid platens and the surfaces of ReHs was modelled as a general contact interaction, and self-contact is applied throughout the modelling. In addition, hard contact was employed in the normal direction, whilst in the tangential direction a friction coefficient of 0.2 [41] was used. Explicit dynamic analysis is adopted to avoid convergence issues [42], but inertia effects cannot be ignored in this case. Therefore, the selection of displacement rate must maintain a balance between computational efficiency and inertial effects. While a higher displacement rate can enhance computational efficiency, it is crucial to ensure that the ratio of kinetic energy to internal energy remains below  $5\%$ , as shown in Fig. 5. Under these conditions, inertial effects become negligible, allowing the compression process to be approximated as quasi-static. Therefore, the crosshead displacement rate adopted the FE analysis was set to  $0.9~\mathrm{m / s}$ .

Here, 10-noded tetrahedral (C3D10M) elements with a  $0.5\mathrm{mm}$  mesh size were used to mesh ReHs, with the mesh sensitivity analysis being shown in Fig. 6. The top and bottom rigid platens were meshed using 4-noded linear quadrilateral (R3D4) elements with a  $0.5\mathrm{mm}$  mesh size. The resulting force and displacement data were used to describe the compression deformation and energy absorption capacity of the structures. It is worth noting that the dimensions of ReHs used in the FE analysis are consistent with the printed samples, as described in Section 2.2.

# 4.2. Uniaxial compression in the  $X$  -direction

The in-plane deformation of the R-ReH, L-ReH and H-ReH structures subjected to compression in the X-direction are shown in Figs. 7 to 9, and the compression strains  $\varepsilon$  (ratio of compression displacement to original height) at each deformation stage are also provided in the figures. It can be seen that the ReH structures contracts inwards in the Y-direction during the compression process, which reflects its auxetic


Table 1 The elastic and plastic material parameters for the R4600 polymer.


<table><tr><td>Young&#x27;s modulus (MPa)</td><td>Poisson&#x27;s ratio</td><td>Density (g/cm3)</td><td>Angle of friction (°)</td><td>Flow Stress Ratio</td><td>Dilation Angle (°)</td></tr><tr><td>2640</td><td>0.42</td><td>1.13</td><td>12</td><td>0.8216</td><td>12</td></tr></table>


Table 2 Ductile damage model parameters for R4600 polymer under compressive and tensile loading.


<table><tr><td></td><td>Fracture strain</td><td>Stress triaxiality</td><td>Strain rate (1/s)</td><td>Fracture energy (N/mm)</td></tr><tr><td>Compression</td><td>0.538</td><td>-0.33</td><td>0.00133</td><td>5</td></tr><tr><td>Tension</td><td>0.028</td><td>0.33</td><td>0.00133</td><td>5</td></tr></table>

![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/f21b1f6ddf2cf5c9e1733af93739616723c80a5a191ed8a0eab6f3736bd3de2b.jpg)



Fig. 5. Kinetic energy (KE) of the structure during compression of different loading speeds.


characteristics. It can be seen from Fig. 7 that R-ReH exhibits brittle fracture of the cell walls during the quasi-static compression process, with fracture occurring preferentially at certain corners where stress concentrations are present. The fracture bands transition towards to the bottom of the sample during the impact process, followed by densification of the whole structure. However, when a hierarchical structure is adopted, the failure process in ReHs changes from brittle fracture to progressive plastic collapse, as shown in Figs. 8 and 9. It is worth noting that when H-ReH enters the densification phase as shown in Fig. 9, it is not completely crushed in a manner similar to other hierarchical ReH structures, which retain the topology of H-ReH and break locally in the lattice.

It can also be observed that cracks in different ReHs initiate at different compressive strains, with R-ReH initiating the crack at a strain of 0.2, and L-ReH/H-ReH at a strain of 0.3. This variation is attributed to the different deformation mechanisms of their structures. When R-ReH is subjected to compression, its horizontal and inclined cell walls undergo bending-shear coupling deformations, caused by rotations at the

![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/8567f591823358454492fdf5c483c99faf359b1f170ed3264bb441f3becf2c8f.jpg)



Fig. 6. Force-displacement curves of R-ReH at different mesh element sizes.


joints [43]. In contrast, for L-ReH and H-ReH, the strain field within the hierarchical lattices is more uniformly distributed under compression [33]. The horizontal and inclined cell walls of the lattices primarily carry axial loads, undergoing tensile and compressive deformations, with no rotations at joints [44]. For R-ReH, the bending-shear coupling deformation mechanism generates severe stress concentrations at the joints during buckling, leading to early-stage cracks. Conversely, the buckling of L-ReH and H-ReH primarily results in densification of the hierarchical lattices [28,33]. As the densification progresses, stress concentrations gradually develop near the joints, eventually resulting in cracks, which occurs significantly later than the cracks induced by bending-shear coupling in R-ReH. Additionally, with increasing lattice filling density, the influence of bending-shear coupling on the cell walls diminishes, and the densification effect becomes more pronounced. This explains the delayed cracks observed in H-ReH compared to L-ReH.

Fig. 10(a)-(b) show the geometrical changes in the H-ReH sample after compression, i.e. during the unloading process and six hours after unloading. If the compression process is stopped and followed by a slow unloading process, deformation in H-ReH is recoverable. With slow

unloading, H-ReH can eventually recover to  $75\%$  of its original height. Indeed, it can be restored to its original height after six hours at room temperature, as shown in Fig. 10. However, L-ReH structure does not significantly recover its deformation after being compressed to the same strain level. Here, instead, the sample enters the densification phase resulting in permanent failure. This unusual mechanical response is attributed to the lattice deformation which changes from the tensile-shear coupling deformation to in-plane compression-dominant deformation mode as the lattice filling density increases. The R4600 polymer exhibits significant plasticity when subjected to tensile and compressive loading, and brittleness when it is subjected to shear loading, Fig. 2. As a result, the structural deformation mode evolves into a progressive plastic collapse mode. To clearly illustrate the shape recovery history of H-ReH, Fig. 10(c) gives the records of the shape recovery ratio and shape recovery rate within 10 minutes after unloading. The expressions of shape recovery ratio and shape recovery rate are as follows [45]:

$$
\text {S h a p e r e c o v e r y r a t i o} = \frac {h _ {r}}{h _ {c}} \tag {9}
$$

$$
\text {S h a p e r e c o v e r y r a t e} = \frac {\Delta h}{\Delta t} \tag {10}
$$

where  $h_r$  and  $h_c$  represent the recovered height at a specific recovery time and the total compressive height of H-ReH, respectively.  $\Delta t$  represents the unit time interval, while  $\Delta h$  denotes the recovered height within the corresponding time period.

It can be observed that H-ReH recovers  $83.2\%$  of the compressive strain within 10 minutes after unloading. The shape recovery rate exhibits an initial increasing trend, reaching its peak value of  $0.26~\mathrm{mm / s}$  at  $216~s$ , and then enters a decreasing phase. It is worth noting that although the shape recovery rate becomes relatively small after 5 minutes, it does not drop to zero. H-ReH continues to recover at an extremely low rate and gradually returns to its original height over 6 hours.

Based on the experimental data and the FE analysis, the reaction forces of R-ReH, L-ReH and H-ReH can be obtained. Fig. 11 shows the stress-strain curves, of which the stresses are obtained from the ratio of reaction forces to the compression cross-sectional area of ReHs and the strains by the ratio of compressive height to original height.

Figs. 7 to 9 compare the experimental and the predicted failure modes in the honeycombs and Fig. 11 compares the associated stress-

![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/62c9234f24df3fb461d1a097d9f0d154556add10374487357ef4d9013b1a4359.jpg)



Fig. 7. Deformation process of R-ReH under quasi-static compression along the X-direction.



Experiment


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/bb886ce5b5678104cea76b7fb94a96cfd1ed2b4259267bec52afa213818a3ea0.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/421077682a0229864793f5939708c7faf0ca4af33c4e96121fa813bbd0bde841.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/5e58865a26a11691bd08239a15026fd295d3307c10f1efd2f5b061295f28381f.jpg)



Simulation


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/fc84874ab8e6362bfb176508ae56ae47b229cb091bafa9ede2bdce07278c0fb3.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/fe3abc5ed1ba560e1e3dd0f0d5e32240b9836eefc078e1ed03e2b2e5477481e7.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/097851fb09ca62a63fa65bc40584c2cef61fe49d8377079241c1ac9c37518bc9.jpg)



$\varepsilon = 0.3$



$\varepsilon = 0.4$



$\varepsilon = 0.6$



Simulation Experiment


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/db93c342db3b120daf7d98d58ac5170b61502af635398d80dcc9fa7390a4f568.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/658697b8e6c784e19b272ba4dcb4b9f4d08ba70d74c48a1930ae1384f1d6237a.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/4e9a79c91dfab605cb9cbbedccb6bf32140ff7520e48cc012938f5e836f698cf.jpg)



Fig. 8. Deformation process of L-ReH under quasi-static compression along the X-direction.


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/8a06b3c13068a265d9a3ecc1c6d4e9a5a86ab55f36d3c8a2196b92d0bcffad34.jpg)



Fig. 9. Deformation process of H-ReH under quasi-static compression along the X-direction.


strain relationships from the FE analysis and the experimental tests. Therefore, the validated FE models can provide reliable predictions of the quasi-static compressive behavior of the ReH structures.

The curves in Fig. 11 show that all ReH structures exhibit common characteristics, i.e. a small initial peak stress occurs at the beginning of the test, followed by a stress plateau phase, and finally a rapid stress increase as the sample enters the densification phase. The smaller initial peak force makes the acceleration of the structure relatively low, avoiding a large instantaneous impact on the protected target. In the stress plateau phase, the stress levels in the different ReH structures are basically consistent but at different levels. When the plateau phase is over, before entering the densification phase, the order of stress levels under the same strain is H-ReH, L-ReH and R-ReH.

For an energy-absorbing structure, it is important to describe the crashworthiness using parameters such as the SEA and the MCF. The effective energy absorption criteria (e.g., SEA and MCF) of structures subjected to compression is generally calculated up to the densification

point. A compressive strain of 0.65, i.e. beyond the densification point was used to calculate and compare their energy absorption capacity. As shown in Fig. 12(a), before the strain reaches 0.4, the SEA values of different ReHs are very similar. However, as the strain increases further, the SEA of H-ReH increases rapidly and far exceeds L-ReH and R-ReH. Specifically, when the strain reaches 0.65, the SEA value of H-ReH is  $130\%$  greater than that of L-ReH and  $620\%$  greater than that of R-ReH. Comparing the SEA values between the strains of 0.4 and 0.65, the SEA values of R-ReH, L-ReH and H-ReH increase by 72, 458 and  $1065\%$ , respectively. Clearly, the adoption of a hierarchical structure can enhance the energy-absorbing capacity, and increasing the lattice filling density of the hierarchical structure can further enhance energy absorption. Fig. 12(b) shows the MCF of ReHs, from which it can be seen that the MCF of R-ReH is approximately horizontal but is higher than that of L-ReH and H-ReH before the strain reaches 0.4. When the strain reaches this value, the upward trend in the MCF is similar to that for the SEA. The MCF value of H-ReH is  $130\%$  greater than that of the L-ReH

![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/6485b5e5ffdaefafa426c859c4aa2a40958e448a82fee210bf732371c7d82986.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/77db834dfc7ad34eb443abfb64c6c0848200d64a9f850a601ec958b04e08bd21.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/b561e3b7059316ec269238ba9676e2fd76dd9da07290d4a3682935bf121621b1.jpg)



Fig. 10. Recoverable deformation of H-ReH after (a) unloading and (b) 6 hours at room temperature; (c) recovery history of H-ReH.


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/03a6dc51b73880029cad5c5b932993dd9fda2bad699e8b6735210dd899e2dc4f.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/6706f972ed68d6ce99c95191272baf160cc55995cb8db81d1ad6a16b8072f284.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/231782e32b796d1562649638fe40ad7b9b956767c576ccd43f6ad8e99397fc99.jpg)



Fig. 11. Comparisons of the stress-strain curves of (a) R-ReH, (b) L-ReH and (c) H-ReH in the X-direction obtained from the experiments and finite element analysis.


and  $640\%$  greater than that of R-ReH when the strain is 0.65. The MCF values of the R-ReH, L-ReH and H-ReH at a strain of 0.4 are increased by 6, 200 and  $620\%$ , respectively.

When the strain reaches 0.65, the R-ReH and L-ReH are considered to be completely densified. As shown in Fig. 10, H-ReH is not completely densified and still has an energy absorption potential. Therefore, the energy absorption capacity of H-ReH is not only superior to that of L-ReH and R-ReH at the same strain, but also can have a superior energy absorption capability than R-ReH and L-ReH.

# 4.3. Uniaxial compression in the  $Y$  direction

Fig. 13 shows the in-plane deformation responses of R-ReH, L-ReH and H-ReH under the compression in the Y-direction. In contrast to the deformation modes shown in Figs. 7-9, all ReHs exhibit deformation in the diagonal direction. At the beginning of the compression process, the deformation modes in the upper and lower parts of the structure are essentially symmetrical. With increasing strain, deformation gradually develops in the diagonal direction. During the compression process in

![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/0329de872f4950e9d22d1208892bba46a1f604fca0936d7fb7f3489c0af93458.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/555e78602a46ec7f5098f49b868a3b86ee2e81441372281e4fe3e01bf2b4c951.jpg)



Fig. 12. (a) SEA-strain curves and (b) MCF-strain curves of R-ReH, L-ReH and H-ReH along the X-direction.


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/c373f498f2ac643816ef8d05d947423077b21259a4fecc8f02299088b857d8c6.jpg)



Fig. 13. Deformation process of (a) R-ReH, (b) L-ReH and (c) H-ReH under quasi-static compression along the Y-direction.


the Y-direction, all ReH samples exhibit a similar failure mode, i.e. local fracture of the cell wall, leading to global densification. This is because the vertical cell walls of both the ReHs and the hierarchical lattices undergo bending-shear coupling deformations and severe buckling, leading to structural instability [46]. As buckling progresses, the ReH structures form multiple collapse bands sequentially [30]. In each collapse band, the cell walls experience self-contact, causing interlocking and eventually forming several diamond enclosed cavities [47]. The above behavior results in brittle fracture and local collapse of the cell walls, further destabilizing the structures. Therefore, during compression along the Y-direction, all three types of ReHs experience instability due to the same underlying mechanism and exhibit the same failure mode. Meanwhile, H-ReH does not exhibit unique recoverable deformation, which is attributed to the failure of progressive plastic collapse of the hierarchical lattices due to cell wall buckling. However, under the compression in the X-direction, the lattices collapse progressively without forming large enclosed cavities, which ensures that the structures remain stable throughout the compression process. These findings indicate that the introduction of hierarchical lattices has minimal effect on the deformation mode of ReHs in the Y-direction.

Fig. 14 (a) shows the stress-strain curves for the ReHs. As can be seen, the different ReHs exhibit an almost identical stress response during the compression process along the Y-direction, and the hierarchical structure does not significantly improve the stiffness of the structure in that direction.

Fig. 14 (b) and (c) present the SEA and MCF of the REHs. Below a strain of 0.6, the SEA of the R-ReH is higher than that of L-ReH and H-ReH. However, when the strain increases above 0.6, the SEA of the H-ReH rises rapidly, exceeding those of the L-ReH and R-ReH. Specifically,

when the strain reaches 0.7, the SEA value of H-ReH is  $13\%$  higher than that of L-ReH and  $28\%$  higher than that of the R-ReH. Similarly, the MCF of the ReHs exhibits a similar trend to the SEA. The MCF value of the H-ReH is  $9\%$  higher than L-ReH and  $18\%$  higher than R-ReH when strain is 0.7.

# 5. Parametric studies of hierarchical re-entrant honeycombs

Based on the validated FE models, the FE analysis was used to investigate the influence of lattice filling density on the crashworthiness, and to study the influence of the RVE distribution and the relative density of the hierarchical ReH structures on energy absorption.

# 5.1. Effects of lattice filling density

In Section 4, the energy absorption capacity of the ReHs with lattice filling densities  $R = 1$  (L-ReH) and  $R = 4$  (H-ReH) were compared experimentally. Further study was carried out to investigate the effect of lattice filling density using finite element modelling. Here higher filling densities of ReH with  $R = 9$  were modelled using the FE analysis and compared to the H-ReH. It can be seen from Fig. 15 that the ReH structure with  $R = 9$  exhibits the same deformation mechanisms as its H-ReH counterpart, these being local buckling and occasional fracture of the lattices, ultimately leading to plastic collapse of the structure. Fig. 16 (a) shows the stress-strain curves from where it can be seen that when the lattice filling density is further increased, the densification phase (from strain 0.4 to strain 0.6) of the stress-strain curve is clearly extended. Further, at the end of the plateau phase, the stress increases more rapidly when the high lattice filling density is higher. Fig. 16(b)

![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/7b48de9e7c7b416b90d061ac7d03cf438af3f1131962dec540e0da4ba6b83b8e.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/09d7f5a1f16c59af75db587a14c11461b2311ab265d42ccc5e72befb67e0b961.jpg)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/57f7f80f53cdd7b59f4d8e195742b7104c866f6858d1aceb8d5d1225f12fc69d.jpg)



Fig. 14. The (a) stress-strain curves, (b) SEA-strain curves and (c) MCF-strain curves of R-ReH, L-ReH and H-ReH along the Y-direction.


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/c0c9f74a162f9865c9d6adf2ec5c74fd6ce1d97e9b1e551a3c3e17a66b4ba1ae.jpg)



Fig. 15. Deformation process of hierarchical ReH structure with  $R = 9$ .



(a)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/16cff51f05b23d173844896fbae76692777c4d8902ca7a02aae2a227d61ef65a.jpg)



(b)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/e9b6489e59dfe11365d547985e67e894caab99da344759ffe38d54cfe2b80ba9.jpg)



(c)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/9496d8f00d91c289bee88b7219db6e55e50b29fa5c9dbc269700e3adac9e6b90.jpg)



Fig. 16. The (a) stress-strain, (b) SEA-strain and (c) MCF-strain curves of H-ReHs with different lattice filling densities.


and (c) show the crashworthiness characteristics of the different lattice filling densities. At the beginning of the energy absorption process, the SEA and MCF values for the  $R = 4$  sample are slightly higher than those for  $R = 9$ . After entering the densification phase, the SEA and MCF values for  $R = 9$  increase rapidly, exceeding the former. Interestingly, the ReH structures with high lattice filling densities ( $R = 4$  and  $R = 9$ ), do not exhibit overall brittle fracture during the densification phase. Clearly, they still exhibit an energy-absorbing ability during this densification phase. Coupled with the information from the SEA and MCF curves, it can be concluded that for cases of significant deformation, a high lattice filling density can further enhance the energy absorption capacity of the structure.

# 5.2. Effects of RVE distribution

In order to study the influence of the number of RVEs in the transverse and longitudinal directions on the energy absorption and deformation modes observed in the structures, the ratio of the number of transverse RVEs to longitudinal RVEs,  $r_{\mathrm{tl}}$ , was taken as a key indicator. Using H-ReH as an example, FE analyses of structures with the ratios  $r_{\mathrm{tl}} = 1.5$ ,  $r_{\mathrm{tl}} = 1$  and  $r_{\mathrm{tl}} = 0.75$  were conducted.

Fig. 17 compares the deformation modes of the H-ReH structures based on different ratios. It can be seen that when the ratio is greater than or equal to unity, the H-ReH structure exhibits an X-shape deformation mode, which reflects the auxetic characteristics of the ReH structures. However, when the ratio is less than unity, the deformation mode is no longer the X-shaped, but the double-V-shape deformation

![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/7cdb8dd70c734578e2fe5d9a5695daa966e1bb3d4960143f31923d0b288d1b40.jpg)



Fig. 17. Deformation modes of H-ReHs with different ratios: (a)  $r_{\mathrm{tl}} = 1.5$ , (b)  $r_{\mathrm{tl}} = 1$ , (c)  $r_{\mathrm{tl}} = 0.75$ . (Top ones are pre-deformation structures).


with one side protruding is observed. The double-V-shape deformation mode renders the structure unstable and easy to buckle.

Fig. 18 shows the stress-strain, SEA-strain and MCF-strain curves for the H-ReH structures. Here, the stress-strain curves for the  $r_{\mathrm{tl}} = 1.5$  and  $r_{\mathrm{tl}} = 1$  structures are relatively close to each other. When the strain is in the range between 0.3 and 0.5, the stress of the H-ReH sample, when  $r_{\mathrm{tl}} = 1$ , fluctuates and is slightly lower than that of the H-ReH based on  $r_{\mathrm{tl}} = 1.5$ . However, the stress level for the H-ReH with  $r_{\mathrm{tl}} = 0.75$  is much lower since the occurrence of buckling leads to a decrease in the measured force. The SEA and MCF values for the H-ReH structures with  $r_{\mathrm{tl}} = 1.5$  and  $r_{\mathrm{tl}} = 1$  are very similar, but higher than those of the H-ReH

with  $r_{\mathrm{tl}} = 0.75$ . Specifically, when the strain reaches 0.5, the SEA value of the H-ReH with  $r_{\mathrm{tl}} = 1.5$  is  $53\%$  higher than that of the H-ReH with  $r_{\mathrm{tl}} = 0.75$ , and the MCF value is  $49\%$  higher.

# 5.3. Effect of relative density

In order to study the effect of relative density on energy absorption, two different densities of H-ReH were considered in the FE analysis. The specific parameters corresponding to these two designs are listed in Table 3. The deformation responses of the lattices based on these two relative densities are displayed in Fig. 19. Failure in the sample based on


(a)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/2c1d1726326761c8ff3753183bdb6c2bb1cf0825829d88a75017ae7771382df5.jpg)



(b)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/d4b741ddad32e1c687a0746f97c40d914229bec575a828a7cf3b46806159aa25.jpg)



(c)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/fda0bebcc232b8a431f8d593834bfcc3281ec71dc21a4b5b3ed0a407b2a142d7.jpg)



Fig. 18. The (a) stress-strain, (b) SEA-strain and (c) MCF-strain curves of H-ReHs with different ratios.



Table 3 Design parameters of H-ReHs at different relative densities.


<table><tr><td>Relative density</td><td>Cell wall thickness (mm)</td><td>Mass(kg)</td></tr><tr><td>0.26</td><td>0.50</td><td>0.116</td></tr><tr><td>0.34</td><td>0.75</td><td>0.147</td></tr></table>

the higher relative density is in a brittle failure mode. As can be seen from Fig. 20, the stress, SEA and MCF values all increase with increasing relative density. It is worth noting that varying the relative density has greater influence on the MCF than on the SEA. For example, when the strain is approximately 0.5, the SEA increases by  $9\%$ , but MCF increases by  $38\%$ .

# 6. Conclusions

In this study, the in-plane crashworthiness, deformation modes and energy absorption characteristics of re-entrant hierarchical honeycombs

subjected to compression have been investigated. In addition, parametric studies investigating the effect of lattice filling density, RVE distribution, relative density and crashworthiness are presented. Based on the findings of this study, the following conclusions can be drawn:

(1) The FE analysis results are in good agreement with the experimental results, with the deformation mode and energy absorption of the ReHs being accurately predicted. During quasi-static compression testing in the X-direction, the ReHs with a high lattice filling density exhibit a superior energy absorption. The SEA and MCF values for the H-ReH are  $132\%$  and  $638\%$  higher than those for the L-ReH, respectively. The SEA and MCF values of the L-ReH structures are  $243\%$  and  $617\%$  greater than those of the R-ReH. This is attributed to the increase in lattice filling density. The failure modes observed in the ReH structures progresses from a brittle fracture failure to the progressive plastic collapse.


(a)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/b40d48444e74db4f74507ea6eeee8b8d6c1ca966eb6e9cb46c371d33c9321a7f.jpg)



(b)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/509b6271d92ffd3289bb93ef36c5acbd7ce96680dfb8a3ef17bb07d2623da8ce.jpg)



Fig. 19. Deformation modes of H-ReHs at the same strain with (a)  $\bar{\rho}$  = 0.26 and (b)  $\bar{\rho}$  = 0.34.



(a)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/c085dfc7b48b3e3dc584afa24160a4a3d3060561bfa3a441b3b11db907df36bb.jpg)



(b)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/934dade6e83c438844063bf877512aa3a236b4b5c483e87a8693c28c80c17146.jpg)



(c)


![](file://D:/MinerU/转换结果/152.pdf-63caf981-79c2-4a53-946c-73add18d54b0/images/0c68fca56bdf77c0b5668e0d9423e0081b069fa206654bfc843280eacf4f7298.jpg)



Fig. 20. The (a) stress-strain, (b) SEA-strain and (c) MCF-strain curves of H-ReHs with different relative densities.




(2) The H-ReH structures exhibit significant recovery following quasi-static compression in the X-direction. With slow unloading, the H-ReH structure can recover to  $75\%$  of the original height, and then after 6 hours at room temperature, it can recover its original height. This is because the lattice deformation mode changes from the tensile-shear coupling one to in-plane compression-dominated deformation one, as the lattice filling density increases.





(3) The deformation and energy absorption characteristics of the various ReHs subjected to the quasi-static compression in the Y-direction are similar. This is attributed to the instability of these structures and results in lower energy-absorbing properties.





(4) With increasing lattice filling density, both SEA and MCF of REHs have been improved. The stress in the ReHs with a higher lattice filling density rises more rapidly at large strains and the ultimate stress level is higher than that associated with a lower lattice filling density. The RVE distribution and relative density of ReHs determines the deformation mode and energy-absorbing capacity. In order to improve the crashworthiness, it is recommended that the structure be designed with a greater number of RVEs distributed in the transverse direction. Finally, with the increase in relative density, the stress level and energy absorption capacity are improved, but the failure mode changes to brittle fracture from progressive plastic collapse.



Based on the conclusions drawn above, this study provides a reliable foundation for the design directions and guidelines of a new generation of hierarchical auxetic energy-absorbing structures. To achieve higher energy absorption capacity and efficiency, it is essential to increase the lattice filling density and the number of distributed RVEs while maintaining a relatively low relative density. Additionally, it is essential to ensure that larger contact surfaces bear the primary crushing forces during the energy-absorbing process.

In future work, cyclic energy-absorbing tests will be conducted to investigate the effects of lattice distribution parameters on the shape recoverability and reversible energy-absorbing capacity of hierarchical auxetic energy-absorbing structures, aiming to enhance their mechanical characteristics and reusability.

# CRediT authorship contribution statement

Zhou Jin: Writing - review & editing, Supervision, Resources, Project administration, Funding acquisition. Liu Hui: Data curation. Lu Pengxu: Writing - original draft, Validation, Methodology, Investigation, Conceptualization. Liu Chunqi: Data curation. Li Hui: Writing - review & editing, Supervision, Conceptualization. Xing Yue: Data curation. Cantwell Wesley J.: Writing - review & editing, Supervision. Liang Xiuning: Data curation. Guan Zhongwei: Writing - review & editing, Supervision.

# Declaration of Competing Interest

The authors declare that they have no known competing financial interests or personal relationships that could have appeared to influence the work reported in this paper.

# Acknowledgments

This work was supported by the National Natural Science Foundation of China [grant number 12002265] and the National Key R&D Program of China [grant number 2021YFF0500100].

# Data availability

Data will be made available on request.

# References



[1] Xu F, Zhang X, Zhang H. A review on functionally graded structures and materials for energy absorption. Eng Struct 2018;171:309-25.





[2] Wang Z. Recent advances in novel metallic honeycomb structure. Compos Part B: Eng 2019;166:731-41.





[3] Qi C, Jiang F, Yang S. Advanced honeycomb designs for improving mechanical properties: A review. Compos Part B: Eng 2021;227:109393.





[4] Wierzbicki T. Crushing analysis of metal honeycombs. Int J Impact Eng 1983;1(2): 157-74.





[5] Papka SD, Kyriakides S. In-plane compressive response and crushing of honeycomb. J Mech Phys Solids 1994;42(10):1499-532.





[6] Wu E, Jiang W-S. Axial crush of metallic honeycombs. Int J Impact Eng 1997;19(5-6):439-56.





[7] Ruan D, Lu G, Wang B, Yu TX. In-plane dynamic crushing of honeycombs—a finite element study. Int J Impact Eng 2003;28(2):161-82.





[8] Aktay L, Johnson AF, Kroplin B-H. Numerical modelling of honeycomb core crush behaviour. Eng Fract Mech 2008;75(9):2616-30.





[9] Gibson LJ, Ashby MF, Schajer GS, Robertson CI. The mechanics of two-dimensional cellular materials. P R Soc A-Math Phy 1997;382(1782):25-42.





[10] Lakes R. Foam Structures with a Negative Poisson's Ratio. Science 1987;235 (4792):1038-40.





[11] Zhang J, Lu G, You Z. Large deformation and energy absorption of additively manufactured auxetic materials and structures: a review. Compos Part B: Eng 2020;201:108340.





[12] Liu W, Wang N, Luo T, Lin Z. In-plane dynamic crushing of re-entrant auxetic cellular structure. Mater Des 2016;100:84-91.





[13] Xiao D, Dong Z, Li Y, Wu W, Fang D. Compression behavior of the graded metallic auxetic reentrant honeycomb: Experiment and finite element analysis. Mat Sci Eng A 2019;758:163-71.





[14] Dong Z, Li Y, Zhao T, Wu W, Xiao D, Liang J. Experimental and numerical studies on the compressive mechanical properties of the metallic auxetic reentrant honeycomb. Mater Des 2019;182:108036.





[15] Zhang J, Lu G. Energy absorption of re-entrant honeycombs in tension and compression. Eng Struct 2023;288:116237.





[16] Li L, Yang F, Zhang S, Guo Z, Wang L, Ren X, et al. A novel hybrid auxetic honeycomb with enhanced load-bearing and energy absorption properties. Eng Struct 2023;289:116335.





[17] Etemadi E, Hosseinabadi M, Taghizadeh M, Scarpa F, Hu H. Enhancing the energy absorption capability of auxetic metamaterials through auxetic cells within re-entrant circular units. Eng Struct 2024;315:118379.





[18] Li S, Liu Z, Shim VPW, Guo Y, Sun Z, Li X, et al. In-plane compression of 3D-printed self-similar hierarchical honeycombs - Static and dynamic analysis. Thin-Walled Struct 2020;157:106990.





[19] Zhang D, Fei Q, Jiang D, Li Y. Numerical and analytical investigation on crushing of fractal-like honeycombs with self-similar hierarchy. Compos Struct 2018;192: 289-99.





[20] Chen Q, Pugno NM. In-plane elastic buckling of hierarchical honeycomb materials. Eur J Mech A Solids 2012;34:120-9.





[21] Sun Y, Pugno NM. In plane stiffness of multifunctional hierarchical honeycombs with negative Poisson's ratio sub-structures. Compos Struct 2013;106:681-9.





[22] Sun Y, Wang B, Pugno N, Wang B, Ding Q. In-plane stiffness of the anisotropic multifunctional hierarchical honeycombs. Compos Struct 2015;131:616-24.





[23] Qiao J, Chen C. In-plane crushing of a hierarchical honeycomb. Int J Solids Struct 2016;85-86:57-66.





[24] Zhang Y, Lu M, Wang CH, Sun G, Li G. Out-of-plane crashworthiness of bio-inspired self-similar regular hierarchical honeycombs. Compos Struct 2016;144:1-13.





[25] Chen Y, Jia Z, Wang L. Hierarchical honeycomb lattice metamaterials with improved thermal resistance and mechanical properties. Compos Struct 2016;152: 395-402.





[26] Yin H, Huang X, Scarpa F, Wen G, Chen Y, Zhang C. In-plane crashworthiness of bio-inspired hierarchical honeycombs. Compos Struct 2018;192:516-27.





[27] Fang J, Sun G, Qiu N, Pang T, Li S, Li Q. On hierarchical honeycombs under out-of-plane crushing. Int J Solids Struct 2018;135:1-13.





[28] Chen Y, Li T, Jia Z, Scarpa F, Yao C-W, Wang L. 3D printed hierarchical honeycombs with shape integrity under large compressive deformations. Mater Des 2018;137:226-34.





[29] Liu H, Zhang ET, Wang G, Ng BF. In-plane crushing behavior and energy absorption of a novel graded honeycomb from hierarchical architecture. Int J Mech Sci 2022;221:107202.





[30] Tan HL, He ZC, Li KX, Li E, Cheng AG, Xu B. In-plane crashworthiness of re-entrant hierarchical honeycombs with negative Poisson's ratio. Compos Struct 2019;229: 111415.





[31] Tan HL, He ZC, Li E, Tan XW, Cheng AG, Li QQ. Energy absorption characteristics of three-layered sandwich panels with graded re-entrant hierarchical honeycombs cores. Aerosp Sci Technol 2020;106:106073.





[32] Xue HT, Tan HL, Chen T, He ZC, Li E, Li QQ, et al. Energy absorption characteristics and multi-objective optimization of a novel reentrant hierarchical honeycomb bumper system. Mech Adv Mater Struct 2022;30(19):3923-36.





[33] Zhan C, Li M, McCoy R, Zhao L, Lu W. 3D printed hierarchical re-entrant honeycombs: Enhanced mechanical properties and the underlying deformation mechanisms. Compos Struct 2022;290:115550.





[34] Tan H, He Z, Li E, Cheng A, Chen T, Tan X, et al. Crashworthiness design and multi-objective optimization of a novel auxetic hierarchical honeycomb crash box. Struct Multidiscip Optim 2021;64(4):2009-24.





[35] Usta F, Zhang Z, Jiang H, Chen Y. Harnessing structural hierarchy and multi-material approaches to improve crushing performance of re-entrant honeycombs. J Manuf Process 2023;92:75-88.





[36] Niknam H, Akbarzadeh AH. Graded lattice structures: Simultaneous enhancement in stiffness and energy absorption. Mater Des 2020;196:109129.





[37] Zou Z, Xu F, Niu X, Fang T, Jiang Z. In-plane crashing behavior and energy absorption of re-entrant honeycomb reinforced by arched ribs. Compos Struct 2023;325:117615.





[38] Sun Y, Li QM. Dynamic compressive behaviour of cellular materials: A review of phenomenon, mechanism and modelling. Int J Impact Eng 2018;112:74-115.





[39] Tang T, Zhang W, Yin H, Wang H. Crushing analysis of thin-walled beams with various section geometries under lateral impact. Thin-Walled Struct 2016;102: 43-57.





[40] Gao Z, Ruan D. Axial crushing of novel hierarchical multi-cell square tubes. Eng Struct 2023;286:116141.





[41] Lv W, Li D, Dong L. Study on mechanical properties of a hierarchical octet-truss structure. Compos Struct 2020;249:112640.





[42] Teng XC, Ren X, Zhang Y, Jiang W, Pan Y, Zhang XG, et al. A simple 3D re-entrant auxetic metamaterial with enhanced energy absorption. Int J Mech Sci 2022;229:107524.





[43] Deshpande VS, Ashby MF, Fleck NA. Foam topology: bending versus stretching dominated architectures. Acta Mater 2001;49(6):1035-40.





[44] Yang W, Mao S, Yang J, Shang T, Song H, Mabon J, et al. Large-deformation and high-strength amorphous porous carbon nanospheres. Sci Rep 2016;6:24187.





[45] Wang K, Sun G, Wang J, Yao S, Baghani M, Peng Y. Reversible energy absorbing behaviors of shape-memory thin-walled structures. Eng Struct 2023;279:115626.





[46] Zhou J, Liu H, Dear JP, Falcon BG, Kazanci Z. Comparison of different quasi-static loading conditions of additively manufactured composite hexagonal and auxetic cellular structures. Int J Mech Sci 2023;244:108054.





[47] Montazeri A, Saeedi A, Bahmanpour E, Mahnama M. Auxetic mechanical metamaterials with symmetry-broken Re-entrant units. Int J Mech Sci 2024;266: 108917.

