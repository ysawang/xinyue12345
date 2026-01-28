# On the design and crashworthiness of a novel auxetic self-locking energy absorption system

![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/dd91ad9068f645ace937449424eaa7de81151932227ececd30ce877761c14ff8.jpg)


Yilin Zhu $^{a,b,*}$ , Ye Fu $^{a}$ , Xue Rui $^{c,d,**}$ , Chao He $^{b}$ , Qingyuan Wang $^{b}$ , Chuanzeng Zhang $^{e,f}$

$^{a}$  School of Civil Engineering and Geomatics, Southwest Petroleum University, Chengdu 610500, Sichuan, China

$^{b}$  Failure Mechanics and Engineering Disaster Prevention, Key Laboratory of Sichuan Province, Sichuan University, 610065 Chengdu, China

$^{c}$  Institute of Launch Dynamics, Nanjing University of Science and Technology, Nanjing 210094, PR China

$^{\mathrm{d}}$  National Key Laboratory of Complex Multibody System Dynamics, Nanjing 210094, PR China

$^{e}$  Center for Mechanics Plus under Extreme Environments, Ningbo University, Ningbo 315211, PR China

f Chair of Structural Mechanics, Department of Civil Engineering, University of Siegen, Paul-Bonatz-Straße 9-11, D-57076 Siegen, Germany

# ARTICLEINFO

Keywords:

Auxetics

Self-locking system

Energy absorption

Meta-structure

Negative Poisson's ratio

# ABSTRACT

Auxetic honeycombs and self-locking energy absorption systems/structures are promising candidates for protective applications. In the present work, a novel auxetic self-locking energy absorption system (ASLEAS) was proposed to utilize the superior properties brought by both the NPR effect and self-locking principle. The proposed ASLEAS consists of thin-walled tubes featuring an I-shaped cross-section which were arranged in a crisscross pattern to analogy to conventional anti-tetra-missing rib auxetic honeycomb. Structural discretization allows the system to be fabricated through cost-effective traditional manufacturing methods, a notable advantage over most auxetic meta-structures that often require expensive additive manufacturing (AM) technology. The proposed system can be conveniently assembled and disassembled to meet the requirement for flexible and responsive impact protection. The protective properties of the proposed system were then comprehensively investigated through numerical analysis under dynamic loading conditions. Results show that the proposed design exhibits evident NPR effects, outstanding self-locking stability and excellent energy absorption capacity as expected. Compared to existing integrated structures, including its integrated variant, it can more effectively reduces stress fluctuations and prevent the transfer of load to the protected object. Moreover, compared to many existing typical nonauxetic self-locking energy absorption systems, it has higher plateau stress and specific energy absorption (SEA). Based on the revealed underlying deformation mechanism, a theoretical model of the collapse stress under quasi-static, low-velocity, and high-velocity impacts were further developed. The present work paves a novel avenue to design protective devices with high performance and low-cost.

# 1. Introduction

Impact accidents are prevalent in various fields such as transportation, civil engineering, mechanical engineering, petroleum engineering and military. Impact loads pose significant safety concerns, threatening both human life and property safety while also potentially causing ecological damage (Eliopoulou et al., 2023; Manohar et al., 2020; Yang et al., 2020; Zhang et al., 2022b; Zhu et al., 2019). Energy absorption structures are critical protective devices against impact loads by absorbing the majority of impact energy typically through plastic

deformation. Metallic single-cell thin-walled tubes or multi-cell thin-walled structures are two kinds of typical energy absorption devices for protective applications.

Metallic single-cell thin-walled tubular structures have garnered attention as early as in the 1960 s (Florence and Vaughan, 1968) due to their potential convenience and superior energy absorption capacity and have played an important role in impact resistance and protection fields ever since. However, single-cell thin-walled tubular structures require external constraints or internal connections to mitigate splashing and second damage upon impact, thereby complicating their application

![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/a26824578c01014bac02f765ba707a0d251870255b186fcb49642faa56afb2fc.jpg)



Fig. 1. Some classical self-locking systems.


intensively. Over the past few years, scholars have proposed several kinds of self-locking energy absorption structures which are capable of withstanding external impacts without additional constraints or internal connections.

The concept of self-locking mechanism is probably dated back to the pioneering work by Chen and her co-workers (Chen et al., 2016; Yang et al., 2018a), who proposed a self-locking energy absorption system composed of dumbbell-shaped thin-walled tubes and investigated the deformation mode and energy absorption capacity of the structure numerically, experimentally and theoretically. Such a self-locking energy absorption system is convenient to be assembled and disassembled, features arbitrary cross-sectional expansion and addresses the issue of splashing under lateral impact loads for traditional metallic tubes, and hence has attracted widespread attention since its inception (Fig. 1).

Subsequently, Chen and her co-workers further advanced their work by modifying the shape the cross-section of the tubular component (Chen et al., 2016), introducing inner tubes (Yang et al., 2017) and proposing composite structure with foam inclusions (Pan et al., 2022) to further improve the energy absorption capacity of the dumbbell-shaped self-locking energy absorption system. Inspired by the dumbbell-shaped self-locking energy absorption system, Chen et al. (2022) developed a self-locking energy absorption structure composed of serially connected diamond-shaped tubes (also known as corrugated tubes), which can also feature simple assembly/disassembly and arbitrary cross-sectional expansion. Recently, Li et al. (2024) proposed a bio-inspired self-locking energy absorption system based on the microstructure of the diabolical ironclad beetle's wings. Unfortunately, the dumbbell-shaped and serially connected diamond-shaped self-locking energy absorption systems can only achieve unidirectional self-locking and hence cannot cope with complex impact loads, which limits their application scenarios

significantly. Therefore, several improved designs have been developed to further achieve planar multi-directional self-locking effect. Inspired by windmill, Liu et al. (2020) proposed a novel omnidirectional self-locking system consisting of thin-walled tubes with windmill-liked cross section. It is also revealed that their new design exhibits higher energy absorption efficiency than that of the round tubular structure and dumbbell-shaped self-locking system. By introducing specific variations in the cross-section of the dumbbell-shaped tube, Zhao et al. (2019; 2023; 2020) designed bidirectional self-locking energy absorbing systems and investigated the quasi-static compressive mechanical properties systematically. Liu et al. (2023) proposed a design strategy that utilizes concave and convex features to achieve periodic self-locking in desired directions. By modifying the dumbbell-shaped tube as a bident-shaped tube, the authors (WANG et al., 2023a) developed a novel self-locking energy absorption system, which is capable of achieving multi-directional self-locking property as well and exhibits excellent energy absorption performance. To achieve spatial expandability, several works also have been conducted by Yang et al. (2023a; 2024; 2023c) and Chen et al. (2024) more recently to propose spatial self-locking energy absorption systems.

Auxetic honeycombs exhibiting negative Poisson's' ratio (NPR) are another kind of promising candidates for protective applications due to their superior energy absorption capacity and regular and scalable microstructures (Balan et al., 2022; Li et al., 2020; Li et al., 2023a; Li et al., 2023d; Lu et al., 2025; Lu et al., 2024; Montgomery-Liljeroth et al., 2023; Qi et al., 2021; Qi et al., 2023; Ren et al., 2018; Shen et al., 2021; Su et al., 2024; Wang et al., 2023b; Wu et al., 2019; Zhang et al., 2023c). The rapid advancement of technical capabilities, particularly additive manufacturing (AM), in recent years has significantly expanded the freedom in designing and manufacturing structures with complex


(a)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/ad153049e559883bdd23c801c766cfff6fb9ba9f70953eeb4f0d431df422b668.jpg)



(b)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/2ccc209530da89dbd77bb8fedd4864f23d1505eaf130973a3f49808f1c755b80.jpg)



(c)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/522f3e1b09761969b1433e1f12732513553830742c38e4b4517ab3631b6d20ba.jpg)



(d)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/5e802cde77a10f18e4346ccf01df3439492247d951f0460b59815dadbb93b9b4.jpg)



Fig. 2. Design methodology: (a) RMCTWS, (b) NSLEAS, (c) ASLEAS and (d) the integrated anti-tetra-missing rib auxetic honeycomb.


configurations (Joseph et al., 2021; Mehrpouya et al., 2019; Xu et al., 2023; Yang et al., 2019a; Zeng et al., 2024; Zhang et al., 2024c). Therefore, auxetic honeycombs have drawn considerable attentions recently and a variety of auxetic honeycombs with different microstructural geometries have been designed and fabricated. Among the numerous types of auxetic honeycomb structures, the anti-tetra-chiral type auxetic honeycombs are particularly worthy of investigation, as they process both chirality and axial symmetry. Up to now, several anti-tetra-chiral type auxetic structures have been designed, such as the conventional anti-tetra-chiral honeycomb which is composed of central rings and tangential ligaments (Bacigalupo and De Bellis, 2015; Bacigalupo and Lepidi, 2016; Chen et al., 2013a; Chen et al., 2013b; Tabacu et al., 2020; Zhang et al., 2023b), anti-tetra-missing rib honeycomb which is obtained by replacing the central ring of the conventional anti-tetra-chiral honeycomb into a central truss (Deng and Lu, 2024; Gaspar et al., 2005; Smith et al., 2000; Zhang et al., 2024d), anti-tetra-missing rib honeycomb with wavy ligaments (Chen et al., 2017; Clausen et al., 2015; Yang et al., 2023b), enhanced anti-tetra-missing rib honeycomb proposed by introducing polygonal enhancement into the central truss (Zhang et al., 2024d; Zhu et al., 2022a), anti-tetra-chiral design inspired from auxetic perforated structure (Han et al., 2023; Hao et al., 2022), hierarchical designs with self-similar principle (Gatt et al., 2015; Wu et al., 2017; Zhang et al., 2023a) and hybrid designs by combining both chiral and re-entrant deformation modes (Chen et al., 2023; Zhang et al., 2021).

Despite significant advancements in the design and manufacturing of auxetic honeycombs and the evolution of additive manufacturing (AM) technology, structures produced through AM still encounter challenges such as internal defects, rough surface finishes, microstructural inconsistencies, and residual stresses, all of which limit their broader application (Mostafaei et al., 2022; Wang et al., 2015; Yao et al., 2022). Additionally, AM technology continues to lag behind traditional manufacturing techniques in terms of maturity, and the associated production costs are often considerably higher than those of conventional methods. Moreover, the majority of current auxetic honeycombs are typically integrated structures with limited flexibility to meet urgent engineering demands (Zhang et al., 2022a; Zhu et al., 2024; Zhu et al., 2022b), and the benefits brought by the self-locking effect have surprisingly been underutilized thus far.

Fortunately, scholars have preliminarily begun exploring the combination of self-locking and negative Poisson's ratio in recently years, though they may have used other terms to express the concept of self-locking in their papers. Zhang et al. (2022a) developed a method to produce an assembled anti-chiral-type auxetic honeycomb by interlocking slotted wavy plates in a crisscrossing pattern. Li et al. (2023b) and Wang et al. (2022) then conducted follow-up works with this method to propose interlocking assembled grid structures. It should be noted that this method is only suitable for structures with simple

configurations and the slot will reduce the strength and load-bearing capacity of the structure. More recently, pioneeringly utilizing the mortise and tenon principle, the authors (Zhu et al., 2024) proposed a novel prefabricated anti-tetra-missing rib honeycomb, which is capable of adopting traditional manufacturing method and maintaining structural stability and as well as load-bearing capacity under severe loading conditions. At about the same time, Li et al. (2024) developed an interlocking energy absorption structure based on the mortise and tenon principle, with its microstructural geometry inspired by the superior compression resistance of the diabolical ironclad beetle. Based on such an principle, Deng et al. (2024) and Yan et al. (2025) subsequently designed self-locking metamaterials with different configurations. Noteworthy, the self-locking structures based on the mortise and tenon principle, however, sacrifice some assembly flexibility in exchange for ensuring the stability of self-locking mechanisms. These set the drawback of the present work. In this work, an auxetic self-locking energy absorption structure (shorted as ASLEAS to simplify the presentation) was proposed to utilize the superior properties brought by both the NPR effect and self-locking property. Most importantly, the proposed design achieves a good balance among manufacturing cost, self-locking stability, mechanical properties and assembly flexibility. The paper is organized as follows. The design methodology of the proposed structure was first elaborated in Section 2. The crashworthiness along with the underlying deformation mechanisms of the proposed design under quasi-static and dynamic impacts, were further presented in Section 3. Theoretical models for the dual energy-absorbing plateau stress were subsequently established in Section 4 and validated numerically in Section 5 to provide guidance of the optimization and application of the proposed structure. Section 6 further emphasizes the advancement of the proposed design in comparison to existing non-auxetic self-locking energy absorption systems. Conclusions and prospects were finally given in Section 7.

# 2. Design methodology

As mentioned previously, the proposed ASLEAS consists of thin-walled tubes featuring an I-shaped cross-section. The design methodology is illustrated in Fig. 2 and elaborated in the following. The rectangular thin-walled tube is the building block of the rectangular multi-cell thin-walled structure (shorted as RMCTWS and depicted in Fig. 2a). No doubt that a system composed of simply stacked rectangular thin-walled tubes will experience splashing under impact loads. Modifying the rectangular tube into an I-shaped tube and stacking it in one direction will create an energy absorption system allowing unidirectional self-locking (Fig. 2b), which is similar as the self-locking system proposed by Chen and her co-workers (Chen et al., 2016; Yang et al., 2018a). Such a system is clearly a non-auxetic self-locking energy absorption system, shorted as NSLEAS in the following. Further, if the I-shaped tubes are

![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/daadef5c0760e641b4cd4a77a88115da8f5539fe5ff1cbaa987d48649f481b3e.jpg)



Fig. 3. The assembly method for ASLEAS.


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/2c042cf2fb61e10f44015551ab63f41bfca08ae08f3a114d1ca00e57b5a9f30b.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/d9590463051f16306e92ba3e0530b2a8b624cf0c354bc5c0cee4d675c4233247.jpg)



Fig. 4. (a) Schematics for dynamic compression and (b) meshed single tubes with various geometrical parameters (the other geometrical parameters for ii) to vi) are identical to those for the standard set).


arranged in a crisscross pattern, a planar multi-directional self-locking energy absorption system (i.e., the proposed ASLEAS) can be achieved, as shown in Fig. 2c. Such an energy absorption structure can also be regard as a discrete variant of the classical anti-tetra-missing rib auxetic honeycomb (Fig. 2d). Noteworthy, for the sake of clarity in the presentation, the terms "system" and "structure" mentioned earlier are collectively referred to as "structure" in the following text.

The cross section of the I-shaped tube consists of two rectangular flanges connected with a rectangular web. The geometry of the I-shaped tube can be fully described by the length and width of the rectangular wing (denoted as  $l$  and  $w$ ), the height and width of the rectangular web (denoted as  $h$  and  $p$ ), the radius  $(r)$  of the smooth transitions introduced at the corners tube to facilitate the fabrication, the overall thickness  $(t)$  of the wall and the out-plane length  $(T)$ . Noted that the above-mentioned longitudinal parameters are all measured from the outer edge. Noted also that according to the geometric compatibility, we have the following geometrical relationships, i.e.,

$$
h = l, l = p + 2 w. \tag {1}
$$

Consequently, there are only five independent geometrical parameters of the I-shaped tube. For simplification, we choose  $l$ ,  $w$ ,  $r$ ,  $t$  and  $T$  as the basic set of geometrical parameters to describe the architecture of the I-

shaped tube.

The assembly method of the proposed ASLEAS is straightforward and user-friendly, which is illustrated in Fig. 3. First, the I-shaped tubular components are stacked alternately in both horizontal and vertical orientations to create a layer. Next, the ASLEAS is constructed through staggered stacking of these layers.

To facilitate the subsequent description of the deformation mechanism, we have defined several terms, such as "longer vertical thin-walled plates", "longer horizontal thin-walled plates", "shorter vertical thin-walled plates", and "shorter horizontal thin-walled plates" as depicted in Fig. 3.

# 3. Crashworthiness

In this section, the crashworthiness as well as the underlying deformation mechanisms of the proposed ASLEAS under both quasi-static and dynamic loads were investigated.

Considering that finite element (FE) analysis is now highly advanced and its effectiveness in simulating mechanical behavior of structures has been extensively validated by numerous scholars, FE simulations were conducted in this section to study the crashworthiness of the proposed design. The mechanical properties of the RMCTWS and NSLEAS were


Table 1 Material parameters of 201 stainless steel.


<table><tr><td>Elasticity modulus E/GPa</td><td>Poisson&#x27;s ratioν</td><td>Yield stress σs/MPa</td><td>Ultimate strength σu/MPa</td><td>Hardening modulus EP/GPa</td><td>Density ρs/(kg/m3)</td></tr><tr><td>191</td><td>0.26</td><td>322</td><td>772.8</td><td>1100</td><td>7830</td></tr></table>

also simulated here for comparison.

# 3.1. Setup for FE simulations

Finite element simulations were conducted using the commercial software Abaqus/Explicit. 3D geometrical models were utilized in this paper (Fig. 4a). As depicted in Fig. 4a, the three energy absorption structures/systems (referred to as systems hereafter to simplify the presentation) were positioned on a rigid supporting plate, where all degrees of freedom were constrained. The rigid loading plate was subjected to a constant velocity  $V$ , with only the vertical displacement allowed, while all other degrees of freedoms were constrained. S4R shell element was employed for the energy absorption structures, and C3D8R solid element was used for the loading and supporting plates. After conducting a convergence analysis (referring to Appendix A), an in-plane mesh size of  $1\mathrm{mm}$  and an out-of-plane mesh size of  $2\mathrm{mm}$  were selected for all the FE simulations. The mesh configurations of the six I-shaped single-tubes with different geometrical parameters for the selected mesh sizes are depicted in Fig. 4b, offering a more intuitive visualization of the meshing strategy. Noted that a set of geometrical parameters  $t: r: w: l: T = 1: 2: 10: 30: 100$  (unit: mm) was considered as a standard set to facilitate the subsequent presentation and discussion. Furthermore, general contact with penalty tangential behavior (friction coefficient  $f = 0.05$ ) and "hard contact" normal behavior were applied to prevent penetration between contact surfaces and accurately represent the interaction between the structures.

Noted that the friction coefficient was roughly considered as 0.05, which is referred to (Yang et al., 2018a). Considering the large amount of contact surfaces of the proposed energy absorption system, the mechanical response may be dependent on the assumed tangential contact behavior. Therefore, the effect of friction coefficient on the crashworthiness was also investigated and the results is given in Appendix B. Fortunately, the friction coefficient has little impact on the

crashworthiness of the structure.

Additionally, 201 stainless steel was utilized as the base material, the material properties were described of which is also referred to Yang et al. (2018a) and presented in Table 1.

A bilinear constitutive model was employed for the base material. Furthermore, the strain rate dependency was accounted for using the Cowper-Symonds model, which provides an effective framework for capturing the material's dynamic response. The Cowper-Symonds model is defined as following, i.e.,

$$
\bar {\varepsilon} _ {m} ^ {p l} = C \left(\frac {\bar {\sigma} _ {m}}{\sigma_ {s}} - 1\right) ^ {n}, \tag {2}
$$

where  $\overline{e}_m^{pl}$  is the equivalent plastic strain rate,  $\overline{\sigma}_{m}$  and  $\sigma_{s}$  are the effective stress and initial yield stress, respectively,  $C$  and  $n$  are dimensionless parameters with values of 40 and 5, respectively (Yang et al., 2018b).

# 3.2. Quasi-static mechanical properties of the ASLEAS

In this part, the quasi-static crashworthiness and the related deformation mechanism of the ASLEAS were simulated and discussed. The standard set of geometrical parameters was considered here.

The quasi-static macroscopic stress-strain  $(\Sigma -\Delta)$  response as well as corresponding deformation modes of the ASLEAS with a standard set of geometrical parameters are shown in Fig. 5. It is indicated from this figure that the quasi-static compressive deformation of the ASLEAS can be clearly divided into four distinct stages, i.e., elastic, plateau, second hardening and densification stages, akin to other energy absorption structures. Noteworthy, the evolution of energy absorption efficiency  $\eta$  is considered here to assist in determining plateau stage. According to (Zhang et al., 2024b; Zhou et al., 2020),  $\eta$  is defined as

$$
\eta = \frac {\int_ {0} ^ {\Delta} \Sigma (\Delta) d \Delta}{\Sigma (\Delta)}, \tag {3}
$$

where  $\Delta$  represents the strain at a specific time, and  $\Sigma (\Delta)$  denotes the stress related to  $\Delta$ . The onset of the plateau stage is marked by the first upward inflection point on the energy absorption efficiency curve, while the end is indicated by the first downward inflection point. Typically, the collapse stress is defined as the average stress between these two inflection points. Noted also that a loading velocity of  $1\mathrm{m / s}$  was adopted for the quasi-static compression simulation to reduce

![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/3cfd14c57c77c2776f6f0dba9eb30b96b9081eb10cea86d3e21c442e9ed129f0.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/bfed012006ff75c57329c3cbdc657b266fa4ba5745b97acf1dec6713d6c97e3d.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/b0a0ab5753834cbe59678843a0d6a6ec2bbb3276916082b8fffe4fc2cdcb15e2.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/1aac660648d37aaaa9ba9607380b49488acb481877d309318f9d519f52f2e65e.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/11f2386a45a4a63158b6d9257b12b83a6b6ad6e9ad3de07fa45670945308112a.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/d4f167087e04af6deeb0c6890f3f7b6b37a402f02e6bab020011d35cd1735b3d.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/a47a90742c5631745b2ac94574fa6b5143894d3316671cfd48456780b0886a1f.jpg)



Fig. 5. Mechanical response of ASLEAS under quasi-static compression. (a) stress-strain relation, (b) kinetic and internal energy evolution and (c) deformation modes.



(a)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/7c083faef4a420c24f176d6301fecc5a8f5cf2a912d24c99624a3f49a54002fe.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/9ea717e53fc7387137bb5784289d87fb9d0f2986ef327410cee46884d62637ca.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/5995013b3243f46df1fe50058b4171e872365001a5d075fa9f8c4370938d6351.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/1aad4c9de949d2a86ba54cf57122a94a224b48795cb9f4fbc35b74cf770eb369.jpg)



(c)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/56353de0fd555f469f81c30639976f80b9834abf4eeceda14d368aa848633377.jpg)



(d)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/ebedbb18da21b6f89c9742fba59e5ce4be374f0d71ce5eadbb50e130bbf54276.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/e6ca35928413705dd1bf2e5361865ae7710c57f9affe7635a8e87bc2686e2ada.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/aeee5ae1d982be576ed694463b0ec9d566c2a2c35477442bc3236708db565b7a.jpg)



Fig. 6. The macroscopic stress-strain responses of ASLEAS under impact loading conditions. (a) stress-strain relation  $(V = 10\mathrm{m / s})$  (b) deformation modes  $(V = 10$  m/s), (c) stress-strain relation  $(V = 70~\mathrm{m / s})$  and (d) deformation modes  $(V = 70~\mathrm{m / s})$


computational time. The kinetic and internal energy evolution of the ASLEAS throughout the entire compression process was shown in Fig. 5b. It is readily observed that the kinetic energy remains well below  $5\%$  of the internal energy, indicating that the simulation accurately represents the quasi-static compression process (Li et al., 2024; Yang et al., 2023a).

As further indicated from Fig. 5, the quasi-static compressive deformation of the ASLEAS can be roughly divided into four stages, i.e., the elastic, plateau, second hardening and densification stages, marked as stages-I, -II, -III and -IV, respectively. In the plateau stage, the bending of the longer vertical thin-walled plates dominates, while the longer horizontal thin-walled plates remain mostly horizontal, experiencing slight positional displacement in the horizontal direction. Additionally, such a deformation mode leads to an overall contraction of the structure under compressive load, exhibiting an evident NPR effect. Subsequently, the positional displacement between the pairs of longer horizontal thin-walled plates intensifies, leading to an evident overall shear collapse of the structure. The contact interactions occurring during the collapse further enhance the structural strength, resulting in a secondary stress hardening. Such a stage is hence termed as second hardening stage. Final, the structure tends to be densified in the densification stage.

# 3.3. Dynamic mechanical properties of the ASLEAS

The dynamic crashworthiness and the related deformation

mechanism of the ASLEAS were further investigated in this part.

Previous to conduct the FE simulations, the critical impact velocities (i.e., the first critical velocity  $V_{\mathrm{cr1}}$  and the second critical velocity  $V_{\mathrm{cr2}}$ ) need to be determined firstly, since the impact velocity is a crucial parameter that significantly influences the collapse behavior of the structures. In term of the impact velocity, three impact modes can be defined, i.e., quasi-static, low-velocity, and high-velocity impacts. Each impact mode generates different stress wave patterns at the impact end of the structure. When the impact velocity is lower than the first critical velocity, the structure primarily displays overall or global deformation. As the impact velocity falls between the first and second critical velocities, localized deformation becomes more pronounced. Beyond the second critical velocity, the structure undergoes significant collapse, progressing through a layer-by-layer failure mechanism(Zhang et al., 2024a).

Based on the studies conducted by Höönig and Stronge (2002) and Yang et al. (2019b), the first and second critical velocities of structures are influenced by the densities of both the base material and the structure (denoted as  $\rho_{\mathrm{s}}$  and  $\overline{\rho}$ , respectively), and can be derived using wave trapping theory. Using their approach, the first and second critical velocities for the ASLEAS, with a standard set of geometrical parameters defined in Section 3.2, are calculated as follows, i.e.,

$$
V _ {\mathrm {c r} 1} = 3. 7 \mathrm {m} / \mathrm {s}, V _ {\mathrm {c r} 2} = 3 8. 2 1 \mathrm {m} / \mathrm {s}. \tag {4}
$$

For clarity in the following discussion, impacts with loading velocities ranging from  $3.7\mathrm{m / s}$  to  $38.21\mathrm{m / s}$  are classified as low-velocity

![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/2c649f7876b7727dbf886a13ca87064a36bdc824321f0cb544d49643679980b1.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/7178da621ef4d6dd7d741918a366d49b701b6cda20c4e8d91048ba9d9346ccac.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/65aa07e4692c78b13ae610e807ab56b002aea0c58d21d77135845c625231c4bb.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/a9ef19142006fc0410432b7c3994af249e1e5f7022587f7080c700c705130bea.jpg)



Fig. 7. Comparison of the FE mechanical behavior of the three structures under quasi-static compression. (a) stress-strain relation of the energy absorption structures, (b) normalized reaction force of the support plates vs. the macroscopic strain of the energy absorption structures, (c) crush stress and (d) SEA.


impacts, while those exceeding  $38.21\mathrm{m / s}$  are considered high-velocity impacts. Noteworthy, although the first and second critical velocities depend on variations in structural dimensions and base materials, the relative density of the structures discussed does not vary so much, and the base material does not change. As a result, we can reasonably approximate that the relative critical speeds given in Eq. (4) correspond to the critical velocities for all the structures discussed here.

The deformation mechanism of the structures is the fundamental basis for the theoretical modeling of the collapse stress. The stress-strain relationships and corresponding deformation modes of the ASLEAS with a standard set of geometrical parameters as defined in Section 3.2 under low-velocity impact  $(V = 10\mathrm{m / s})$  and high-velocity impact  $(V = 70\mathrm{m / s})$  are hence presented in Fig. 6, where excellent self-locking stabilitiy can be observed.

As indicated in Fig. 6a, the deformation of the ASLEAS under low-velocity impact can be divided into six stages, i.e., the elastic, first plateau, second hardening, second plateau, third hardening and densification stages. The deformation mechanism observed in Fig. 6b is elaborated in the following. Similar as the quasi-static compression, in the first plateau stage (stage-II), all the longer vertical thin-walled plates bend and come into contact with each other, while the shorter vertical thin-walled plates remain roughly vertical without local deformation. In contract, all the short horizontal thin-walled plates bend, while the longer horizontal thin-walled plates remain roughly horizontal. Such a deformation mode also leads to an overall contraction of the structure under compressive load, exhibiting an evident NPR effect. Then, the bending of the shorter vertical thin-walled plates at the loaded and supported parts of the structure intensifies, and the flanges of the vertically arranged I-shaped tubes undergo distortion, causing the edge of the shorter horizontal thin-wall plates to come into contact with the longer horizontal plates of the flanges. This effect undoubtedly increases the structural strength, pushing the deformation into the second hardening stage (stage-III). Subsequently, the distortion of the flanges gradually propagates from both ends toward the center, and the structure quickly enters the second plateau stage (stage-IV). In the second

plateau stage, localized shear deformation of the structure can already be observed. In stage-V, the shear deformation becomes more pronounced, further increasing the contact between components, thereby enhancing the strength of the structure and resulting in a third hardening. Finally, the structure tends to be densified, and such a stage is termed as densification stage (stage-VI).

For high-velocity impact, only one plateau stage can be observed, and the deformation of the ASLEAS under high-velocity impact is divided into three stages, i.e., the elastic, plateau and densification stages (Fig. 6c). In the plateau stage under high-velocity impact, the structure undergoes significant localized deformation characterized by progressive crushing across multiple layers (Fig. 6d). At this stage, the structure's behavior transitions, and it no longer exhibits the NPR effect typically seen under quasi-static loading conditions and low-velocity impacts, as dynamic effects dominate and alter its mechanical response.

# 3.4. Comparison with existing energy absorption structures

To highlight the superiority of the proposed structure in energy absorption and protection, a comprehensive comparison of the crashworthiness between the proposed design and two existing structures (i.e., the nonauxetic RMCTWS and NSLEAS as depicted in Section 2) was firstly conducted in this part. To ensure a fair comparison, the relative densities of the three structures were kept identical  $(\overline{\rho} = 0.18)$  and the overall dimensions of all the energy absorption structures were carefully maintained with minimal differences. The standard set of geometrical parameters defined in Section 3.2 was considered for the single tube of the ASLEAS. The NSLEAS consists of 63 I-shaped tubes and a set of geometrical parameters  $t: r: w: l: T = 1: 2: 22.5: 20: 100$  (unit: mm) was adopted for the single tube of the NSLEAS. Noted that all the symbols mentioned above carry the same meaning as those for the ASLEAS since they share the same microstructural configuration. The RMCTWS is composed of an array of 10 rectangular units in the horizontal direction and 16 units in the vertical direction. The length and width of each rectangular unit are  $29\mathrm{mm}$  and  $18\mathrm{mm}$ , respectively.

![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/9cc6b43916bcbdd2614f416485534d9c40a2e320773999971d12c487bc4170d0.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/b25a9526195770ced1d91bbeabc17d36f7a4527f6e156ccef31c7a44e5c9ecc6.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/2dea4ad32f251959261b2b51436e41e99361520cf771ff9b0557e3ded77ec440.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/a659003e2058b7b5b588929118fa4f5cb7e356e162e692b6e3db1561d7c27e14.jpg)



Fig. 8. Comparison of the FE mechanical behavior of the three structures under low-velocity impact  $(V = 30\mathrm{m / s})$  (a) stress-strain relation of the energy absorption structures, (b) normalized reaction force of the support plates vs. the macroscopic strain of the energy absorption structures, (c) crush stress and (d) SEA.


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/917e3d9e036faba9d64c1958e7dbbc7c4764e35e209c6096c771cae2b6157bf0.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/970796950802405e0f826df1c2828c25c843389621d91de8a406dc288dbe9e69.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/93d903467b01f9d089b59a93dd188ebc315297b35a90e66ff2fa29c7ecfda2aa.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/7c1038c0f1733d49de6fae143dd3ef522ef944b9ecddb9c04d8cedb2c5ad1a10.jpg)



Fig. 9. Comparison of the FE mechanical behavior of the three structures under high-velocity impact  $(V = 70\mathrm{m / s})$  (a) stress-strain relation of the energy absorption structures, (b) normalized reaction force of the support plates vs. the macroscopic strain of the energy absorption structures, (c) crush stress and (d) SEA.


The mechanical properties of the three structures under quasi-static compression, low and high-velocity impact were depicted in Figs. 7-9. To offer a thorough comparison, these figures present a detailed analysis of the stress-strain response of the structures, the evolution of the

reaction force (normalized by the area of the cross section of the structures, denoted as  $\Sigma_{\mathrm{f}}$ ) of the supporting plate, the crush stress (defined as the first peak stress of the structures) and the specific energy absorption (SEA).

![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/1914073315cae2822a36f3c944f4f57ae217d25e7da55d870183e1db22701b19.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/7438f8c9004eea457393184f1f68fedf65e72de08f5772f427b29df888910601.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/65e30e26173b87e3743fe2a76eaf6160ddef90f33064e685acd17ef2a1f3edc4.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/9c919150890eb2f71a8f7a232d4cffc4bb9e39a9d275453edb577600e9ce0d9f.jpg)



Fig. 10. Comparison of the FE mechanical behavior of the proposed ASLEAS and integrated anti-tetra-missing rib auxetic honeycomb: (a) stress-strain response  $(V = 30\mathrm{m / s})$ , (b) normalized reaction force of the support plates  $(V = 30\mathrm{m / s})$ , (c) stress-strain response  $(V = 70\mathrm{m / s})$ , (d) normalized reaction force of the support plates  $(V = 70\mathrm{m / s})$ .


The specific energy absorption (SEA) is a common indicator used to evaluate the energy absorption capacity of structures (Gao and Liao, 2021; Li et al., 2023c), which is defined as

$$
S E A = \frac {\int_ {0} ^ {\mu_ {\max }} F (u) \mathrm {d} u}{m _ {\mathrm {T}}}, \tag {5}
$$

where  $F$  and  $u$  are the reaction force and displacement of the loading plate, respectively,  $u_{\mathrm{max}}$  is the displacement of the loading plate at the point when the structure reaches densification, and  $m_{\mathrm{T}}$  is the total mass of the structure.

As indicated from Figs. 7-9, overall, the assembled structures (i.e., NSLEAS and ASLEAS) significantly reduces stress fluctuations compared to the integrated structure (i.e., the RMCTWS), while greatly lowers the initial crush stress as well. With the introduction of more flexibility, the assembled structure can more effectively prevent the transfer of external load to the protected object (supporting plate), leading to a significantly lower reaction force on the protected object, as shown in Fig. 7b, 8b and 9b. Moreover, the assembled structures also exhibit higher specific energy absorption.

Further comparison of the two assembled energy absorption structures reveals that, compared to the nonauxetic assembled structure, the auxetic assembled structure proposed in this paper process lower reaction force on the supporting plate, smoother stress evolution and comparable specific energy absorption. Considering that both two assembled structures share similar constituent components, with the only difference being the NPR effect introduced in the structure proposed in this paper, it can hence be concluded that the NPR effect imparts better protective characteristics to the energy absorption structures.

Since the proposed ASLEAS is a variant of the integrated anti-tetramissing rib auxetic honeycomb, we therefore also compared the crash-

worthiness of these two structures numerically. Low- and high-velocity impacts were considered with  $V = 30 \, \mathrm{m/s}$  and  $V = 70 \, \mathrm{m/s}$ , respectively. The standard set of geometrical parameters defined in Section 3.2 was also considered for the single tube of the ASLEAS. To ensure a fair comparison, both structures were designed with identical unit cell sizes and macroscopic dimensions. Additionally, the overall thickness of the integrated anti-tetra-missing rib auxetic honeycomb was set to twice that of the single-tube structure in ASLEAS. Consequently, the relative density of the integrated anti-tetra-missing rib auxetic honeycomb is  $22\%$ , which is slightly higher than that of ASLEAS ( $\overline{\rho} = 0.18$ ) due to the absence of some single tubes at the edges of the ASLEAS.

The stress-strain responses of the two structures, along with the evolution of the reaction force on the supporting plates, are presented in Fig. 10. The figure illustrates that, due to its enhanced flexibility, the proposed design sacrifices some collapse stress but significantly minimizes stress fluctuations and effectively delays the transmission of external loads to the protected object.

# 4. Theoretical modeling of the collapse stress

The collapse stress of the plateau stage is an important indicator for evaluating the energy absorption capacity of structures. Therefore, we derived the theoretical models for the collapse stress of the proposed ASLEAS structure under quasi-static compression, low- and high-velocity impacts, providing theoretical guidance for its engineering applications.

# 4.1. Quasi-static compression

Considering the geometrical symmetry, a smallest repeatable unit (SRU) as depicted in Fig. 10 was picked out here for the theoretical

![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/4c16ca8c351bd9ccc8fefa2d8f457f97ecc988e368d7f3c6f16d34a11eecd721.jpg)



Fig. 11. Free body diagram of the ASLEAS under quasi-static compression.


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/804dc0d331c4993db46d00b8682f9838f2d5dab6649f15995f7f9503efacbb23.jpg)



Fig. 12. Deformation modes the ASLEAS at certain deformation levels during low-velocity impacts.


analysis. Since there is no external horizontal load subjected to the structure, all the cut edges of the SRU must be free of any horizontal force. Moreover, the cut edges of the outer vertical plates must be free of any vertical force since no shear force acts on these edges due to the axial symmetry of the whole structure. Consequently, these edges experience equal magnitudes of vertical forces (denoted as  $F / 2$ ) that are opposite in direction. Recall in Section 3.2 that, in the plateau stage of quasi-static compression, the bending of the outer vertical plates dominates, and the horizontal outer plates remain mostly horizontal. Again, considering the symmetry of the structure, only cut edges of the outer vertical plates undergo moment (denoted as  $M / 2$ ). The free body diagram (FBD) of SRU is hence obtained and detailed illustrated in Fig. 11.

According to the moment equilibrium, we have

$$
F = \frac {M}{w}. \tag {6}
$$

In the plateau stage of quasi-static compression, all the cut edges of the SUR can be assumed as plastic hinge lines. We hence have

$$
M = \frac {1}{2} t ^ {2} T \sigma_ {0}, \tag {7}
$$

where  $\sigma_0$  is the yield stress of materials exhibiting elastic-perfect plastic property. To account for the fact that most materials are not truly ideal plastic materials, Wen et al. (2022) and Yang et al. (2018a) proposed a correction for the yield stress as follows

$$
\sigma_ {0} = \frac {\sigma_ {\mathrm {s}} + \sigma_ {\mathrm {u}}}{2}, \tag {8}
$$

where  $\sigma_{\mathrm{s}}$  and  $\sigma_{\mathrm{u}}$  are the initial yield and ultimate stresses of the material.  $M$  is hence rewritten as

$$
M = \frac {1}{4} t ^ {2} T \left(\sigma_ {\mathrm {s}} + \sigma_ {\mathrm {u}}\right). \tag {9}
$$

Considering the force balance of each layer of the structure in the direction of the external load, we have

$$
\sigma_ {Q} = \frac {n F}{n l T} = \frac {F}{l T}, \tag {10}
$$

where  $\sigma_{Q}$  is the quasi-static collapse stress of the structure and  $n$  is the number of SRU of each layer.

In view of Eqs. (6), 9, 10), the quasi-static collapse stress  $\sigma_{Q}$  is obtained as,

$$
\sigma_ {Q} = \frac {t ^ {2} \left(\sigma_ {\mathrm {s}} + \sigma_ {\mathrm {u}}\right)}{4 l T}. \tag {11}
$$

Once the theoretical formula for collapse stress under quasi-static compression is established, inertia effects can be subsequently considered to derive the theoretical expression for the plateau stress under dynamic impact. The derivation of the theoretical model of the collapse stress under low- and high-velocity impacts are further elaborated in the following sub-sections.

# 4.2. Low-velocity impact

Recall that two plateau stages were observed during the low-velocity impact of the proposed structure, with the deformation mechanism in the first plateau stage being similar to that of quasi-static compression. Therefore, the theoretical expression of the collapse stress (denoted as  $\sigma_{L - I}$ ) of the first plateau stage under low-velocity impact can be readily obtained by analyzing the relationship among the change of momentum and the increment in collapse stress relative to the quasi-static loading condition.

To better observe the changes in deformation of the ASLEAS at typical moments, the deformation modes of two vertically connected unit-cells (the upper and lower unit-cells are termed as  $\alpha$ - and  $\beta$ - unit-cells, respectively) at the initial moment (denoted as  $t_1$ ) and the moment when the first plateau stage ends (denoted as  $t_2$ ) were depicted in Fig. 11. The height of the two vertically connected unit-cells at the moments  $t_1$  and  $t_2$  are readily obtained as

![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/a99ccb9ce2226d64e2f171eb4d3ec07e4d87e0899d7749438113ce186b2464d2.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/ee21bfc16e0f72dbaaddb5bbc802d1a9d26d8d637fd631ed25bacc1fa106dc46.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/446532a1d91a5b357afc8d9f52570b4fde9be42aeb6d10abce43820b017e19ce.jpg)



Fig. 13. Deformations of the ASLEAS at (a) the beginning and (b) the end of the second plateau stage. (c) the schematic diagram of the supposed typical deformation of each unit-cell.


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/9761fedc116819521a2fb83b42e9b26f32eb3ef771b1f47cd03fb6bb3002b565.jpg)



Fig. 14. Deformation modes the ASLEAS at certain deformation levels during high-velocity impacts.


$$
H _ {1} = 4 w + 2 h + p, H _ {2} = 2 l \sin \theta + 4 w - 4 t, \tag {12}
$$

where  $\theta = \frac{l / 2}{l / 2} = 1$ , which can be readily obtained from Fig. 12.

From the initial moment  $t_1 = 0$  to moment  $t_2$ , the change of momentum  $(\Delta p)$  is readily obtained as

$$
\Delta p = p _ {2} ^ {\alpha} + p _ {2} ^ {\beta} - p _ {1} ^ {\alpha} - p _ {1} ^ {\beta}, \tag {13}
$$

where  $p_i^\alpha$  and  $p_i^\beta$  are the momentum of the  $\alpha$ - and  $\beta$ -unit-cells at the moment  $t_i (i = 1,2)$ . Undoubtedly,  $p_i^\alpha$  and  $p_i^\beta$  are all identical to zero at the initial moment. Moreover, according to the study by Qiao and Chen (2015), the velocity of the upper unit-cell at the moment  $t_2$  is assumed to be equal to the loaded impact velocity, while the velocity of the lower unit-cell is nearly zero. We can readily have

$$
\Delta p = p _ {2} ^ {a} = m V = t T (4 l + 2 h + 4 w - 2 p - 2 4 r + 6 \pi r - \pi t) \rho_ {s} V. \tag {14}
$$

where  $m$  is the mass of one unit-cell.

Based on the conservation of momentum, the change in momentum can also be expressed as

$$
\Delta p = 2 l T \int_ {t _ {1}} ^ {t _ {2}} \left(\sigma_ {L - I} - \sigma_ {Q}\right) d t. \tag {15}
$$

Additionally, according to the kinematic relationship, we have

$$
\left(t _ {2} - t _ {1}\right) V = H _ {1} - H _ {2}. \tag {16}
$$

Solving Eqs. (14-16) simultaneously, the collapse stress  $\sigma_{L - I}$  is derived as

$$
\sigma_ {L - 1} = \sigma_ {Q} + \frac {2 t \rho_ {s} V ^ {2} (4 l + 2 h + 4 w - 2 p - 2 4 r + 6 \pi r - \pi t)}{l (2 h + p - 2 l \sin \theta + 4 t)}. \tag {17}
$$

Revisiting Section 3.2 once again, the deformation mechanism changes since the second hardening stage. The deformation profiles of the structure at the beginning and end of the second plateau stages were further given in Fig. 13, with the moments denoted as  $t_3$  and  $t_4$ , respectively. As illustrated in this figure, each unit-cell now includes 16 additional plastic hinge lines. The plastic work done by these additional plastic hinge lines will contribute to the collapse stress of the second plateau stage (denoted as  $\sigma_{L - \mathrm{II}}$ ) under low-velocity impact. We readily obtained that

$$
\sigma_ {L - \mathrm {I I}} = \sigma_ {L - \mathrm {I}} + \Delta \sigma , \tag {18}
$$

where  $\Delta \sigma$  denotes the contribution of the additional plastic hinge lines to the  $\sigma_{L - \mathrm{II}}$ .

During the second plateau stage, the structure undergoes relatively complex deformation. Based on the observed deformation mechanism, the typical deformation mode of each unit-cell was supposed as the schematic diagram as shown in Fig. 13c. Noted that each pair of adjacent thin-walled plates in the deformation schematic shown in Fig. 13c was combined into a single plate for simplification. According to the geometrical relations, the height of the unit-cell at the moments  $t_3$  and  $t_4$  (denoted as  $H_{u1}$  and  $H_{u2}$ ) and the ration angle of each plastic hinge line (denoted as  $\varphi$ ) can be expressed as

$$
H _ {u 1} = l \sin \theta + 2 w - 2 t, H _ {u 2} = l \sin \theta + 2 t, \tag {19}
$$

![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/7199fd02251fda1417ef33ba6b0c9dc5e2172948168dea0948350bafbc575087.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/f63c64c17a509e893bcc74973d59a4792d9fb31d6d4befc332010b7902f5ce31.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/617a96dea269663db456c248224402b9cfec5a98268b96adcfa96c19ff804ac3.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/79f0c2e35390cc9652aef85d3b459005e78830a4296c3deb8d850361c31b99bd.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/d2a631c4103f818869f49bace9e107f33251ccb2b1448a5809582c2c4e50dbe4.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/7300195651c68ae3e27704cdf688e93ef3e7fe314834d4f678585656289072f4.jpg)



Fig. 15. The FE simulation predicted impact collapse stresses in terms of macroscopic stress-strain response for the proposed ASLEAS with different loading conditions. (a) Quasi-static, (b)  $V = 10 \, \mathrm{m/s}$ , (c)  $V = 20 \, \mathrm{m/s}$ , (d)  $V = 30 \, \mathrm{m/s}$ , (e)  $V = 70 \, \mathrm{m/s}$ , (f)  $V = 90 \, \mathrm{m/s}$ .


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/66bcea90eca9f31bb3823db509d85aa6cd5dc2a92a20b27c8d3fa9fefbd6e6be.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/d40752a7d3926b3c49857e7debc12eb4ed873f459b2e494964e752d65a98ae57.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/00b29eca1fb7abdde8118016573aa4acf5dbcd3b06b306266e36cc9d407c67b6.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/849725b59af7cd100ea13774001e845efe202be607555e6dd0ccd7cc8aaa3e44.jpg)



Fig. 16. Theoretical and FE simulation results of the collapse stress of the ASLEAS. The effect of (a) impact velocity, (b) wing length  $l$  (mm), (c) wing width  $w$  (mm) and (d) overall thickness  $t$  (mm) on the collapse stress.



(a)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/51fe0adca0f9d2539b1efb0cb0447389f38b94c21f97c51ccf5e27849e40701e.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/4e8ec1c3ed9a692ae195aac310d9e15ca9b3bcffe23c520639761208386af5c2.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/87e7e80719fee09be8250fed820e020e6c12960cc66d9068776eaca5b20c9cce.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/1fc0836cff01d04d3abd43158efd65c1172351bede2e450c926e3e78afd98bd7.jpg)



(b) 9


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/f44d387ba7a3bcd493511cc85302fde7346b6d1bf786819632c2ea4ec3761e5d.jpg)



(c)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/34b9dc16ca40300b0b90511ef5f064607ad0c7d21550c6180dad140a1a246858.jpg)



Fig. 17. Comparison of the proposed structure with existing nonauxetic self-locking energy absorption structures. (a) geometrical configurations of four reported self-locking energy absorption structures, (b) collapse stress and (c) SEA.


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/e763ef076bedd65be86ee01ef87a943fa8e58a3cc1959cf7063e5948c1b40f86.jpg)



Fig. A1. Mesh convergence study of the FE model, with the geometrical parameters of the standard set.


$$
\varphi = \arctan \frac {2 w}{l - (l \sin \theta + 2 t) \tan \frac {\theta^ {\prime}}{2}} \tag {20}
$$

Apparently, the internal plastic work  $(W_{p})$  done by the additional plastic hinge lines and the external work acted on the unit-cell  $(W_{e})$  from the moment  $t_3$  to  $t_4$  can be defined as

$$
W _ {p} = 1 6 \times \frac {M}{2} \times \varphi = 8 \text {M a r c t a n} \frac {2 w}{l - (l \sin \theta + 2 t) \tan \frac {\theta}{2}} \tag {21}
$$

$$
W _ {e} = \Delta \sigma L _ {1} T \left(H _ {u 1} - H _ {u 2}\right), \tag {22}
$$

with  $L_{1} = 2l - 4t$

According to the principle of energy conservation, the internal plastic work must equal the work done by external forces, i.e.,

$$
W _ {p} = W _ {e}. \tag {23}
$$

Combining the Eqs. (9), 18-23), the second plateau stress is obtained as

$$
\sigma_ {L - \Pi} = \sigma_ {L - I} + \frac {\arctan \frac {2 w}{l - (l \sin \theta + 2 t) \tan \frac {2}{2}} t ^ {2} \left(\sigma_ {\mathrm {s}} + \sigma_ {\mathrm {u}}\right)}{2 (l - 2 t) (w - 2 t)} \tag {24}
$$

# 4.3. High-velocity impact

The procedure for deriving the theoretical formulation of collapse stress under high-velocity impact (denoted as  $\sigma_{H}$ ) closely resembles that used for low-velocity impact. Therefore, only a brief overview of the derivation process is provided here.

The only difference is the expression of the height of the two vertically connected unit-cells at moment  $t_2$  as depicted in Fig. 14, where the deformation modes were given for the initial moment  $(t_1)$  and the moment when the  $\alpha$ -unit-cell was fully collapsed  $(t_2)$ . According to the observed deformation mechanism, the height  $H_2$  is expressed as

$$
H _ {2} = h + 4 w + 4 t. \tag {25}
$$

![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/7fe0a386931e1e03225193984340df1390233dfd701c4eb0d282292f707ae1c7.jpg)


![](file://D:/MinerU/转换结果/160.pdf-7c4cfbd0-7611-445f-b6f8-47643b482c0e/images/cc92401c2b3f12bac6ef388692cde6fa1cd6614c2ea846cd476d5d263ff5be56.jpg)



Fig. B1. Effect of friction properties on the energy absorption characteristics. (a) Stress-strain response for different friction coefficients, (b) collapse stress (the geometrical parameters is identical to the standard set).


Adopting similar derivation process,  $\sigma_{H}$  is derived as

$$
\sigma_ {H} = \sigma_ {Q} + \frac {2 t \rho_ {s} V ^ {2} (4 l + 2 h + 4 w - 2 p - 2 4 r + 6 \pi r - \pi t)}{l (h + p - 4 t)}. \tag {26}
$$

# 5. Validations and discussions

The validity of the theoretical models for collapse stresses derived in the previous section is numerically verified in this section.

Firstly, Fig. 15 shows the FE predicted impact collapse stresses (dash lines) in terms of macroscopic stress-strain response (solid lines) for the proposed ASLEAS with different loading velocities. This figure clearly demonstrates that the theoretically predicted collapse stresses closely align with the collapse response calculated by the FE simulations, which verifies the validity of the theoretical formulas.

A more comprehensive comparison of the dynamic collapse stress obtained from the theoretical formula and FE simulations are further given in Fig. 16. Both the effects of impact velocity and the geometrical parameters on the dynamic mechanical response were investigated here. The variation of three key geometrical parameters, i.e.,  $l$ ,  $w$ , and  $t$  were considered. The numerical and theoretical results align closely, as shown in Fig. 16, demonstrating the high predictive accuracy of the theoretical model proposed in this study.

As further observed in Fig. 16, the dynamic collapse stress of the ASLEAS increases with loading velocity, the decrement of rectangular wing length  $l$  and the increment of rectangular wing width  $w$  the overall thickness  $t$ . These findings can provide guidance for the application of ASLEAS as energy absorbing protective devices.

# 6. Comparison with reported self-locking energy absorption structures

To further reveal the advantages and innovation of the proposed auxetic self-locking energy absorption structure, it is worthwhile to compare it with previously published nonauxetic self-locking energy absorption structures. Considering the proposed design is a two-dimensional structure, four reported two-dimensional self-locking energy absorption structures were considered for comparison, i.e., the traditional dumbbell-shaped self-locking energy absorption structure, shorted as DSSLEAS (Yang et al., 2018a), windmill-shaped self-locking energy absorption structure, shorted as WSSLEAS (Liu et al., 2020), the corrugated self-locking energy absorption structure, shorted as CSLEAS (Chen et al., 2022) and the self-locking energy absorption structure with tubes inspired by diabolical ironclad beetle, shorted as SLEASDIB (Li et al., 2024). These structures have distinct microstructural configurations (as shown in Fig. 17a), making it challenging to provide a fair comparison of their mechanical properties. Given that the lightweight characteristic is a key performance indicator, Fig. 17b and 17c illustrate

the evolution of collapse stress and SEA for five different structures, showing how they vary with relative density under different geometrical parameters.

As shown in Fig. 17b and 17c, the auxetic self-locking energy absorption structure we developed generally exhibits better crashworthiness compared to nonauxetic energy absorption structures, confirming the superiority of combining negative Poisson's ratio with self-locking principle.

# 7. Conclusions

By utilizing the superior properties brought by both the NPR effect and self-locking principle, a novel auxetic self-locking energy absorption structure was proposed in this work. The quasi-static and dynamic mechanical properties of the proposed design were then systematically investigated numerically and theoretically. The major findings from this study can be summarized as follows:

(1) Structural discretization enables the proposed energy absorption structure to be manufactured using cost-effective traditional methods, while offering exceptional flexibility for protective applications.

(2) Compared to integrated honeycombs (both auxetic and nonauxetic), the proposed design more effectively minimizes the stress fluctuations and delays the transfer of external loads to the protected object, resulting in a significantly lower reaction force.

(3) Compared to existing non-auxetic self-locking energy absorption structures, the proposed design demonstrates enhanced crashworthiness, including superior collapse stress and specific energy absorption.

(4) The theoretical formulas derived for the proposed design accurately describe how collapse stress evolves with changes in geometry and loading velocity, providing useful insights for tailoring mechanical properties to specific targets.

Noted that the elastic constants of the structure, such as the effective Poisson's ratio and elastic modulus, also warrant further investigation. We plan to address this aspect in a future work by deriving theoretical formulas for elastic constants of the proposed structure and validating them through both numerical simulations and experimental tests.

# CRediT authorship contribution statement

Yilin Zhu: Writing - review & editing, Supervision, Methodology, Funding acquisition, Conceptualization. Ye Fu: Writing - original draft, Visualization, Software, Formal analysis, Data curation. Xue Rui: Writing - review & editing, Supervision, Project administration,

Investigation. Chao He: Visualization, Resources. Qingyuan Wang: Writing - review & editing, Project administration. Chuanzeng Zhang: Writing - review & editing, Supervision.

# Declaration of competing interest

The authors declare that they have no known competing financial interests or personal relationships that could have appeared to influence the work reported in this paper.

# Acknowledgements

The financial supports from the National Natural Science Foundation of China (12372143), Sichuan Science and Technology Program (2025ZNSFSC0092) and 2024 Open Project of Failure Mechanics and Engineering Disaster Prevention, Key Lab of Sichuan Province (No. FMEDP202405) are gratefully acknowledged.

The numerical calculations in this paper have been done on the supercomputing system in the High Performance Computing Center of Southwest Petroleum University.

# Appendix A. Mesh convergence analysis

Fig. A1..

# Appendix B. The effect of friction coefficient on crashworthiness

Fig. B1..

# Data availability

Data will be made available on request.

# References



Bacigalupo, A., De Bellis, M.L., 2015. Auxetic anti-tetrachiral materials: equivalent elastic properties and frequency band-gaps. Composite Structures 131, 530-544.





Bacigalupo, A., Lepidi, M., 2016. High-frequency parametric approximation of the Floquet-Bloch spectrum for anti-tetrachiral materials. International Journal of Solids and Structures 97-98, 575-592.





Balan, M., Mertens, J., Bahubalandruni, M.R., 2022. Auxetic Mechanical Metamaterials and their Futuristic Developments: A state-of-art Review. Materials Today. Communications 105285.





Chen, Y., Scarpa, F., Liu, Y., Leng, J., 2013. Elasticity of anti-tetrachiral anisotropic lattices. International Journal of Solids and Structures 50, 996-1004.





Chen, Y., Qiao, C., Qiu, X., Zhao, S., Zhen, C., Liu, B., 2016. A novel self-locked energy absorbing system. Journal of the Mechanics and Physics of Solids 87, 130-149.





Chen, Y., Li, T., Scarpa, F., Wang, L., 2017. Lattice metamaterials with mechanically tunable Poisson's ratio for vibration control. Physical Review Applied 7, 024012.





Chen, Z., Wu, Q., Yang, H., Yang, L., Xiong, J., 2022. A periodic dissipative system with self-locking capacity. International Journal of Impact Engineering 166, 104233.





Chen, Z., Wei, X., Yang, L., Xiong, J., 2024. Origami-based bidirectional self-locking system for energy absorption. Journal of the Mechanics and Physics of Solids 188.





Chen, M., Zhong, R., Wang, Y., Wu, H., Fu, M., 2023. Mechanical properties of re-entrant chiral anisotropic honeycomb. Engineering Structures 291, 116431.





Clausen, A., Wang, F., Jensen, J.S., Sigmund, O., Lewis, J.A., 2015. Topology optimized architectures with programmable Poisson's ratio over large deformations. Adv. Mater 27, 5523-5527.





Deng, X., Lu, Q., 2024. Crushing performance of a novel tetra-missing rib honeycomb: Experimental and numerical studies. Journal of the Mechanical Behavior of Biomedical Materials 151, 106410.





Deng, J., Zhao, W., Wang, J., Li, J., Wu, B., Li, X., Liu, X., Chen, L., Liu, T., Zhu, S., 2024. A novel design of an I-shape self-locked thin-walled system with mortise and tenon joints. Thin-Walled Structures 201, 111966.





Eliopoulou, E., Alissafaki, A., Papanikolaou, A., 2023. Statistical analysis of accidents and review of safety level of passenger ships. Journal of Marine Science and Engineering 11, 410.





Florence, A., Vaughan, H., 1968. Dynamic plastic flow buckling of short cylindrical shells due to impulsive loading. International Journal of Solids and Structures 4, 741-756.





Gao, Q., Liao, W.-H., 2021. Energy absorption of thin walled tube filled with gradient auxetic structures-theory and simulation. International Journal of Mechanical Sciences 201, 106475.





Gaspar, N., Ren, X.J., Smith, C.W., Grima, J.N., Evans, K.E., 2005. Novel honeycombs with auxetic behaviour. Acta Materialia 53, 2439-2445.





Gatt, R., Mizzi, L., Azzopardi, J.I., Azzopardi, K.M., Attard, D., Casha, A., Briffa, J., Grima, J.N., 2015. Hierarchical Auxetic Mechanical Metamaterials. Scientific Reports 5, 8395.





Han, D., Zhang, Y., Zhang, X.Y., Xie, Y.M., Ren, X., 2023. Lightweight auxetic tubular metamaterials: Design and mechanical characteristics. Composite Structures 311, 116849.





Hao, J., Han, D., Zhang, X.G., Zhang, Y., Jiang, W., Teng, X.C., Lang, J.P., Pan, Y., Ni, X. H., Zhang, X.Y., 2022. Novel dual-platform lightweight metamaterials with auxeticity. Engineering Structures 270, 114891.





Hönig, A., Stronge, W.J., 2002. In-plane dynamic crushing of honeycomb - Part I: crush band initiation and wave trapping. International Journal of Mechanical Sciences 44, 1665-1696.





Joseph, A., Mahesh, V., Harursampath, D., 2021. On the application of additive manufacturing methods for auxetic structures: A review. Advances in Manufacturing 9, 342-368.





Li, D., Gao, R., Dong, L., Lam, W.-K., Zhang, F., 2020. A novel 3D re-entrant unit cell structure with negative Poisson's ratio and tunable stiffness. Smart Materials and Structures 29, 045015.





Li, G.-F., Liu, H.-T., Wang, Y.-B., Cai, G.-B., 2023a. Mechanical properties of 3D auxetic structure: Emergence of transverse isotropy. International Journal of Mechanical Sciences 250, 108285.





Li, N., Liu, S.Z., Wu, X.N., Wang, J.Y., Han, Y.S., Zhang, X.C., 2023c. Mechanical characteristics of a novel rotating star-rhombic auxetic structure with multi-plateau stages. Thin-Walled Structures 191, 111081.





Li, X., Peng, W., Wu, W., Xiong, J., Lu, Y., 2023d. Auxetic mechanical metamaterials: from soft to stiff. International Journal of Extreme Manufacturing 5, 042003.





Li, J.F., Qin, Q.H., Zhang, W., Wang, Q., Peng, J.X., 2023b. On Quasi-Static and Dynamic Compressive Behaviors of Interlocked Composite Kagome Lattice Structures. Journal of Applied Mechanics-Transactions of the Asme 90, 1-23.





Li, J., Sui, C., Sang, Y., Zhou, Y., Zang, Z., Zhao, Y., He, X., Wang, C., 2024. A flexible, reusable and adjustable high-performance energy absorption system inspired by interlocking suture structures. International Journal of Solids and Structures 296, 112839.





Liu, H., Qiao, C., Ma, Y., Pan, F., Chen, Y., 2023. A concave-convex design strategy for periodic self-locked energy-absorbing systems. International Journal of Impact Engineering 175, 104539.





Liu, Y., Xiong, F., Yang, K., Chen, Y., 2020. A novel omnidirectional self-locked energy absorption system inspired by windmill. Journal of Applied Mechanics 87, 085001.





Lu, F., Wei, T., Zhang, C., Huang, Y., Zhu, Y., Rui, X., 2024. A novel 3D tetra-missing rib auxetic meta-structure with tension/compression-twisting coupling effect. Thin-Walled Structures 199, 111764.





Lu, F., Mo, W., Wei, T., Huang, Y.H., Zhou, S.Z., Zhu, Y., 2025. A novel 3D auxetic metastructure based on enhanced hexa-missing rib honeycomb. Engineering Structures 326, 119597.





Manohar, T., Suribabu, C., Murali, G., Salaimanimagudam, M., 2020. A novel steel-PAFRC composite fender for bridge pier protection under low velocity vessel impacts. Structures. Elsevier 765-777.





Mehrpouya, M., Dehghanghadikolaei, A., Fotovati, B., Vosooghnia, A., Emamian, S.S., Gisario, A., 2019. The potential of additive manufacturing in the smart factory industrial 4.0: A review. Applied Sciences 9, 3865.





Montgomery-Liljeroth, E., Schievano, S., Burriesci, G., 2023. Elastic properties of 2D auxetic honeycomb structures-a review. Applied Materials Today 30, 101722.





Mostafaei, A., Zhao, C., He, Y., Ghibaasian, S.R., Shi, B., Shao, S., Shamsaei, N., Wu, Z., Kouraytem, N., Sun, T., Pauza, J., Gordon, J., V, Webler, B., Parab, N.D., Asherloo, M.D., Guo, Q., Chen, L., Rollett, A., 2022. Defects and anomalies in powder bed fusion metal additive manufacturing. Current Opinion in Solid State & Materials Science 26.





Pan, J., Zhu, W., Yang, K., Hu, L., Chen, Y., 2022. Energy absorption of discretely assembled composite self-locked systems. Composite Structures 292, 115686.





Qi, C., Jiang, F., Yang, S., 2021. Advanced honeycomb designs for improving mechanical properties: A review. Composites Part B: Engineering 227, 109393.





Qi, C., Pei, L.-Z., Remennikov, A., Yang, S., Jiang, F., 2023. Numerical and theoretical analysis of crushing strength of 3D re-entrant honeycomb. Thin-Walled Structures 182, 110140.





Qiao, J., Chen, C.Q., 2015. Analyses on the In-Plane Impact Resistance of Auxetic Double Arrowhead Honeycombs. Journal of Applied Mechanics 82, 1-9.





Ren, X., Das, R., Phuong, T., Tuan, D., Ngo, X., 2018. Auxetic metamaterials and structures: a review. Smart Materials & Structures 27, 023001.





Shen, L., Wang, Z., Wang, X., Wei, K., 2021. Negative Poisson's ratio and effective Young's modulus of a vertex-based hierarchical re-entrant honeycomb structure. International Journal of Mechanical Sciences 206, 106611.





Smith, C.W., Grima, J., Evans, K., 2000. A novel mechanism for generating auxetic behaviour in reticulated foams: missing rib foam model. Acta Materialia 48, 4349-4356.





Su, B., Zhou, Z., Qiu, J., Yao, X., Li, Z., Wang, Z., Shu, X., 2024. Multiaxial yield behavior of 2D re-entrant auxetic cellular materials. Engineering Structures 311, 118216.





Tabacu, S., Negrea, R.F., Negrea, D., 2020. Experimental, numerical and analytical investigation of 2D tetra-anti-chiral structure under compressive loads. Thin-Walled Structures 155, 106929.





Wang, Z.P., Li, J.F., Li, H.B., Wei, B.F., Qin, Q.H., 2022. Mechanical properties and damage failure of carbon fiber reinforced polymer composite sandwich structure with square honeycomb core using the interlocking method. Acta Materiae Compositae Sinica 39, 1778.





Wang, X., Lu, F., Wang, H., Cui, H., Tang, X., Wu, Y., 2015. Mechanical constraint intensity effects on solidification cracking during laser welding of aluminum alloys (Article). Journal of Materials Processing Technology 218, 62-70.





Wang, W.-J., Zhang, W.-M., Guo, M.-F., Yang, J.-S., Ma, L., 2023b. Energy absorption characteristics of a lightweight auxetic honeycomb under low-velocity impact loading. Thin-Walled Structures 185, 110577.





Wang, K.-W., Zhu, Y.-L., Zhao, X., Yu, C., Shao, Y.-B., 2023a. Design and energy absorption capacity study on bident-shaped spatial self-locked energy absorbing system. Engineering Mechanics 41 (12), 57-66.





Wen, W., Lei, M., Tao, Y., Lian, Y., 2022. Out-of-plane crashworthiness of bio-inspired hierarchical diamond honeycombs with variable cell wall thickness. Thin-Walled Structures 176.





Wu, W., Tao, Y., Xia, Y., Chen, J., Lei, H., Sun, L., Fang, D., 2017. Mechanical properties of hierarchical anti-tetrachiral metastructures. Extreme Mechanics Letters 16, 18-32.





Wu, W., Hu, W., Qian, G., Liao, H., Xu, X., Berto, F., 2019. Mechanical design and multifunctional applications of chiral mechanical metamaterials: A review. Materials & Design 180, 107950.





Xu, R., Chen, C., Sun, J., He, Y., Li, X., Lu, M., Chen, Y., 2023. The design, manufacture and application of multistable mechanical metamaterials-a state-of-the-art review. International Journal of Extreme Manufacturing 5 (4), 042013.





Yan, H., Xie, S., Zhang, F., Jing, K., He, L., 2025. Sound absorption performance of honeycomb metamaterials Inspired by Mortise-and-Tenon structures. Applied Acoustics 228, 110292.





Yang, K., Chen, Y., Liu, S., Qiao, C., Yang, J., 2017. Internally nested self-locked tube system for energy absorption. Thin-Walled Structures 119, 371-384.





Yang, K.J., Chen, Y.L., Zhang, L., Xiong, F., Hu, X., Qiao, C., 2019b. Shape and geometry design for self-locked energy absorption systems. International Journal of Mechanical Sciences 156, 312-328.





Yang, K., Hu, X., Pan, F., Qiao, C., Ding, B., Hu, L., Hu, X., He, Z., Chen, Y., 2023a. An on-demand tunable energy absorption system to resolve multi-directional impacts. International Journal of Solids and Structures 271, 112257.





Yang, K., Li, Z., Ge, D., 2023b. Quasi-static and dynamic out-of-plane crashworthiness of 3D curved-walled mixed-phase honeycombs. Thin-Walled Structures 182, 110305.





Yang, K., Li, Z., Huang, P., Lin, Y., Huang, L., 2024. Mechanical and failure characteristics of novel tailorable architected metamaterials against crash impact. Engineering Failure Analysis 159, 108141.





Yang, X., Ma, J., Wen, D., Yang, J., 2020. Crashworthy design and energy absorption mechanisms for helicopter structures: A systematic literature review. Progress in Aerospace Sciences 114, 100618.





Yang, K., Qin, Q., Zhai, Z., Qiao, C., Chen, Y., Yang, J., 2018. Dynamic response of selflocked energy absorption system under impact loadings. International Journal of Impact Engineering 122, 209-227.





Yang, K., Rao, L., Hu, L., Pan, F., Yin, Q., Chen, Y., 2023c. Flexible, efficient and adaptive modular impact-resistant metamaterials. International Journal of Mechanical Sciences 239, 107893.





Yang, H., Wang, B., Ma, L., 2019a. Mechanical properties of 3D double-U auxetic structures. International Journal of Solids and Structures 180, 13-29.





Yao, X., Wang, J., Yang, Y., Zhang, X., Cheng, X., Zhang, S., 2022. Review on Defect Formation Mechanisms and Control Methods of Metallic Components During Laser Additive Manufacturing. Zhongguo Jiguang/chinese Journal of Lasers 49.





Zeng, Z., Gao, S., Pokkalla, D.K., Zhang, S., Han, C., Liu, F., Xiao, Z., Kandukuri, S.Y., Liu, Y., Zhou, K., 2024. Additive manufacturing of metallic metamaterials with enhanced mechanical properties enabled by microstructural and structural design. International Journal of Machine Tools and Manufacture 199, 104172.





Zhang, C., Ba, S., Zhao, Z., Li, L., Tang, H., Wang, X., 2023a. Energy absorption characteristics of novel bio-inspired hierarchical anti-tetrachiral structures. Composite Structures 313, 116860.





Zhang, X., Han, Y., Zhu, M., Chu, Y., Li, W., Zhang, Y., Zhang, Y., Luo, J., Tao, R., Qi, J., 2024c. Bio-inspired 4D printed intelligent lattice metamaterials with tunable mechanical property. International Journal of Mechanical Sciences 272, 109198.





Zhang, X.-C., Liu, N.-N., An, C.-C., Wu, H.-X., Li, N., Hao, K.-M., 2023c. Dynamic crushing behaviors and enhanced energy absorption of bio-inspired hierarchical honeycombs with different topologies. Defence Technology 22, 99-111.





Zhang, C., Lu, F., Wu, J., Liu, X., Zhu, Y., 2023b. Theoretical modeling and optimization of the plateau force of tubular anti-tetrachiral structures. Smart Materials and Structures 32, 075004.





Zhang, C., Lu, F., Lin, B., Ling, X., Zhu, Y., 2024a. Analysis on the collapse stress of auxetic tubular anti-tetrachiral structures. European Journal of Mechanics - A/solids 103, 105167.





Zhang, C., Lu, F., Wei, T., Huang, Y., He, Y., Zhu, Y., 2024b. A novel windmill-shaped auxetic structure with energy absorption enhancement. International Journal of Mechanical Sciences 280, 109635.





Zhang, Y., Ren, X., Jiang, W., Han, D., Zhang, X.Y., Pan, Y., Xie, Y.M., 2022a. In-plane compressive properties of assembled auxetic chiral honeycomb composed of slotted wave plate. Materials & Design 221, 110956.





Zhang, Y., Wang, G., Zhang, Y., Ye, J., Zeng, T., Zhao, K., Zheng, Z., Wan, R., 2022b. Crashworthiness design of car threshold based on aluminium foam sandwich structure. International Journal of Crashworthiness 27, 1167-1178.





Zhang, Y., Ma, L.-H., Xu, H.-Q., Zhou, W., 2024d. A novel anti-missing-rib lozenge lattice metamaterial with enhanced mechanical properties. Materials Today Communications 38, 108151.





Zhang, W., Zhao, S., Scarpa, F., Wang, J., Sun, R., 2021. In-plane mechanical behavior of novel auxetic hybrid metamaterials. Thin-Walled Structures 159, 107191.





Zhao, Y., Chen, L., Du, B., Liu, H., Chen, B., Peng, S., Guo, Y., Chen, L., Li, W., Fang, D., 2019. Bidirectional self-locked energy absorbing system: Design and quasi-static compression properties. Thin-Walled Structures 144, 106366.





Zhao, Y., Chen, L., Wu, Z., Du, B., Chen, L., Li, W., Fang, D., 2020. Lateral crushing behavior of novel carbon fiber/epoxy composite bidirectional self-locked thin-walled tubular structure and system. Thin-Walled Structures 157, 107063.





Zhao, Y., Chen, L., Li, W., Wu, Q., Wu, L., 2023. Improving energy absorption of bidirectional self-locked structures and systems inspired by origami crease. European Journal of Mechanics-A/solids 100, 104977.





Zhou, H., Zhao, M., Ma, Z., Zhang, D.Z., Fu, G., 2020. Sheet and network based functionally graded lattice structures manufactured by selective laser melting: Design, mechanical properties, and simulation. International Journal of Mechanical Sciences 175, 105480.





Zhu, Y., Jiang, S., Lu, F., Ren, X., 2022a. A novel enhanced anti-tetra-missing rib auxetic structure with tailorable in-plane mechanical properties. Engineering Structures 262, 114399.





Zhu, Y., Gao, D., Shao, Y., Chen, H., Yu, C., Wang, Q., 2024. A novel prefabricated auxetic honeycomb meta-structure based on mortise and tenon principle. Composite Structures 329, 117782.





Zhu, L., Liu, W., Fang, H., Chen, J., Zhuang, Y., Han, J., 2019. Design and simulation of innovative foam-filled Lattice Composite Bumper System for bridge protection in ship collisions. Composites Part B: Engineering 157, 24-35.





Zhu, Y., Luo, Y., Gao, D., Yu, C., Ren, X., Zhang, C., 2022b. In-plane elastic properties of a novel re-entrant auxetic honeycomb with zigzag inclined ligaments. Engineering Structures 268, 114788.

