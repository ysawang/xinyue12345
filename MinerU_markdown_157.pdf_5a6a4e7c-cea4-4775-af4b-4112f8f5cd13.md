Full length article

# Efficient data driven optimization framework for designing B-spline honeycombs with excellent energy absorption

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/bdb12c658bd012396f1140ffb2ee4de2febbbe380e6bbc745c52de4dcc768251.jpg)


Sicong Zhou a, Kang Zhang a, Liuchao Jin a, Qiang Gao b, Wei-Hsin Liao a,c,*

$^{a}$  Department of Mechanical and Automation Engineering, The Chinese University of Hong Kong, Shatin, Hong Kong, China

b School of Mechanical Engineering, Southeast University, Nanjing, China

$^{c}$  Institute of Intelligent Design and Manufacturing, The Chinese University of Hong Kong, Shatin, Hong Kong, China

# ARTICLEINFO

# Keywords:

Honeycomb

Machine learning

Energy absorption

Optimization design

Empirical equation

# ABSTRACT

Designing honeycomb structures with exceptional energy absorption capabilities and a broad design space is crucial for meeting the increasing demands in the field of impact protection. In this study, innovative B-spline honeycombs (BSHs) were developed to represent a variety of polyline/curve hexagonal honeycombs. The energy absorption performance of the BSHs was assessed using the finite element method, validated by quasi-static compression experiments. The developed data-driven optimization design framework integrates deep neural network models and genetic algorithms, enabling the generation of novel BSHs that fulfill specific design criteria. Using this framework, the upper specific energy absorption boundary of BSHs was determined to identify configurations with the highest specific energy absorption across varying relative densities. Additionally, empirical equations to compute the maximum initial peaking compression force, mean compression force, and specific energy absorption of BSHs at specific relative densities were summarized. These optimized BSHs were categorized into bowl-shaped BSHs, 30-sided BSHs, 5-shaped BSHs, 2-shaped BSHs, M-shaped BSHs, and  $r$ -shaped BSHs based on their topological structures. The BSH with the highest specific energy absorption,  $13.4~\mathrm{J / g}$ , belonged to the 5-shaped BSHs category, with a corresponding relative density of  $9.15\%$ . The predominant deformation mode for these optimized BSHs, ensuring maximal material utilization, was identified as perfect folding mode. Compared to traditional hexagonal honeycomb and other polyline/curve hexagonal configurations at equivalent relative densities, the BSHs exhibited superior energy absorption capabilities. This study offers a systematic design approach for future endeavors aimed at developing high energy absorbing honeycombs with more intricate cross-sectional shapes.

# 1. Introduction

As typical cellular materials, honeycomb structures consist of unit cells that are arranged in a parallel stacking configuration along the in-plane direction, forming a periodic topology. This distinctive topology imparts honeycombs with a lower relative density compared to their constituent materials, consequently endowing them with exceptional specific mechanical properties such as specific elastic modulus, specific strength, and specific energy absorption. The advantageous properties of honeycombs make them highly desirable for lightweight structural applications in various industries, including aerospace [1-3], automotive [4,5], railway [6], marine [7], protective gear [8], wearable sensor [9], and packaging [10,11]. Moreover, by manipulating the unit cell configuration, honeycombs can be tailored to exhibit unique mechanical

properties, such as negative thermal expansion [12,13], negative stiffness [14-16], and negative Poisson's ratio [17-21]. The high mechanical freedom allows for the creation of honeycombs with customized characteristics to meet specific engineering requirements, including impact resistance [22-24], vibration reduction [25-27], heat insulation [28-30].

Honeycombs exhibit anisotropy with distinct mechanical properties in the in-plane and out-of-plane directions, resulting from variations in deformation mechanisms [31,32]. When subjected to in-plane loading, honeycomb cell walls primarily undergo bending deformation, with the plastic hinges forming perpendicular to the plane. Conversely, under out-of-plane loading, the primary deformation modes of honeycombs include cell wall buckling and membrane deformation, leading to a more intricate distribution of plastic hinges. Generally, honeycombs subjected

to out-of-plane loading demonstrate higher stress levels compared to those experiencing in-plane loading, thereby exhibiting improved energy absorption capacity. Out-of-plane compression of honeycombs entail three deformation modes: global buckling, transitional buckling, and full-fold collapse [33]. In the global buckling mode, honeycombs exhibit a single plastic hinge line, resulting in a lower plateau force. Conversely, the full-fold collapse mode entails the appearance of multiple plastic hinge lines on honeycombs, leading to numerous folds on the wall, thereby generating a larger and more stable plateau force. The transitional buckling mode serves as an intermediate deformation mode between the global buckling and full-fold collapse modes, where honeycombs transition from full-fold to global buckling after the formation of several folds.

Over the past two decades, there has been a significant proliferation of honeycomb designs aimed at achieving diverse objectives. Numerous strategies, such as curved design, hierarchical approaches, graded design, and hybrid strategy, have been employed as guiding principles to construct innovative honeycomb configurations. The presence of curved structures in nature has inspired the development of honeycombs with curved edges, which exhibit promising mechanical properties, such as vibration control capabilities [34], energy absorption performance [35, 36], and stiffness [37]. Hierarchical structures, including self-similar hierarchical structures [38] and non-self-similar structures [39], have also been extensively observed in biological materials, contributing to their exceptional mechanical performance. Common hierarchical honeycombs encompass vertex hierarchy [40-43], cell-wall hierarchy [44, 45], face hierarchy [46,47], and spiderweb hierarchy [48,49], which are determined based on the location of small-scale configurations. The gradient design methodology confers substantial advantages in the field of honeycomb structure design by facilitating the creation of customized material distributions. Through grading cell wall thickness [50-52] or cell configuration distribution [53-56], gradient honeycombs exhibit distinct stress-strain curves and deformation modes in comparison to their uniform counterparts. Hybrid design entails the integration of multiple unit cells with diverse topological configurations, resulting in a novel honeycomb structure that harnesses the mechanical advantages of these individual units [57-59]. Furthermore, the hybrid honeycomb enables the customization of geometric parameters, thereby expanding the design space for achieving desired performance characteristics [60], such as the ability to absorb greater energy with reduced structural mass [61]. Finally, it should be emphasized that these design strategies are not independent of each other, some honeycombs are proposed by combining them together, such as the combination of curved and gradient strategies [62,63], the combination of hierarchical and hybrid strategies [64] and the combination of gradient and hybrid strategies [65].

A forementioned strategies can be categorized as traditional design methods, which require designers to possess extensive experience in mechanical structure design. However, these methods face challenges in identifying the design boundaries of specific configurations due to the high costs associated with experiments or finite element analysis, resulting in limited design flexibility. Fortunately, the emergence of machine learning has opened new avenues for exploring the deformation mechanisms and mechanical performance of honeycombs with various configurations at a relatively lower cost. By employing machine learning techniques, it becomes possible to design honeycombs with distinct in-plane elastic modulus [66], negative Poisson's ratio [67-69], and semi-auxetic properties [70]. Moreover, machine learning methodologies facilitate the simultaneous optimization of multiple mechanical characteristics. For example, the utilization of a data-augmented deep autoencoder enables the design of Bézier curve honeycombs with programmable negative Poisson's ratio and thermal expansion performance [71]. The energy absorption behavior of honeycombs poses a highly nonlinear problem, particularly when dealing with a large number of design parameters, making the construction of surrogate models challenging. However, artificial neural networks exhibit

remarkable capabilities in capturing the nonlinear relationships between structural parameters and energy absorption properties. Manipulating gradient distribution parameters to modify deformation modes can significantly influence the impact resistance of honeycombs, and machine learning methods offer a cost-effective means to identify the optimal gradient distribution [22,72]. Furthermore, different types of neural networks have been employed for predicting deformation modes [73] and forecasting energy absorption performance based on deformed structure images [74].

In summary, existing polyline/curve honeycombs have limited design freedom to comprehensively represent the category of polyline/ curve honeycombs, leading to it is difficult to determine the realistic upper energy absorption design boundary of polyline/curve honeycombs. Therefore, this study proposes innovative B-spline honeycombs (BSHs), the honeycombs with B-spline shaped wall, to represent different polyline/curve honeycombs. However, traditional optimization methods for energy absorption structures, such as surrogate models [75], are difficult to optimize the structures with numerous design parameters. An efficient data-driven optimization design framework is developed to explore the energy absorption boundary of BSHs and investigate design principles for BSHs exhibiting exceptional energy absorption characteristics. Section 2 provides an overview of the data collection methods employed, including geometric modeling, quasi-static experiments, and finite element analysis. Subsequently, in Section 3, deep neural network (DNN) models are constructed and trained utilizing the initial dataset generated in Section 2 to predict the relative density, initial peak compression force (PCF), mean compression force (MCF), and specific energy absorption (SEA) of BSHs. Furthermore, an optimization design framework is established by integrating the DNN models with the genetic algorithm. Section 4 encompasses the upper design boundary of the PCF, MCF, and SEA for the BSHs at varying relative density, with the empirical equations for determining these boundaries succinctly presented. Furthermore, a thorough discussion is conducted on the geometric characteristics and deformation mechanisms of the optimized configurations. Finally, the broader design space and the exceptional energy absorption performance of BSHs in comparison to common energy absorption materials and structures signify significant potential applications in the field of impact resistance.

# 2. Data collection

This section presents the methodology employed to construct the energy absorption properties database of honeycombs, encompassing the procedures for building BSH and the numerical approach for gathering the associated mechanical properties.

# 2.1. Structural configuration of B-spline honeycomb

The unit cell of the traditional hexagonal honeycomb (THH) is a regular hexagon comprising 6 straight edges of equal length. By changing straight lines to polylines or curves, the diversity of honeycomb structures can be significantly improved, facilitating the identification of the honeycomb configurations with superior energy absorption properties. Sharp edges typically result in stress concentrations that are prone to structural failure. As a geometric representation standard, the B-spline curves are widely used in the computer aided design and fabrication due to fast calculation and numerically stable characteristics. Therefore, the B-spline curve is applied to model the smooth outside profile of the honeycomb for lower stress concentrations and fabrication conveniences, as illustrated in Fig. 1a, which can open flexible polyline/ curve honeycombs design space. The function of the B-spline curve with an order of  $p$  and  $n$  control points is expressed as

$$
\mathbf {S} (\xi) = \sum_ {i = 0} ^ {n - 1} \mathrm {P} _ {i} b _ {i p} (\xi) \tag {1}
$$


(a)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/5b8d7e44224b6016c433a500bf7b504e505a5c97d8e3d21a11d2b6cb9bb3dcaf.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/d75a500591a3e4761b18dfc62232a085f75a0168083c913a53fe4a8ccbb78f51.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/98c376b6a390c2608261cdf76de83fa74f2e8218378c8f58ae86ea7cc2c42392.jpg)



(b)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/f09399abec468dc8ace57d177f28e44bc98540aecafd94dcc77420371de3a374.jpg)



Fitting-A


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/7d3b2b8a5d1a901ee25ed8337014dbe3f354b669cb4c942191b50d59c5847754.jpg)



Fitting-B


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/589fb1f7020e55be97d53a1b30f057ba218891608fb5b5f868d3db36dc66739e.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/d8272a3f3f94c4b31dc819b876cf005a3254429502c5664192720372ea6a6b6b.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/73e6d2587f485fd2fd821f4c39c15a09d8f992da126c41bd6ea6eecb9dd3a40a.jpg)



Fig. 1. Configuration of the BSH: (a) The unit cell; (b) The array type.


where  $S(\xi)$  signifies the curve,  $P_{i}$  represents the control points, and  $\xi$  denotes the parametric coordinate. Besides, the expressions of the B-spline basis are given by

$$
b _ {i, 0} (\xi) = \left\{ \begin{array}{l} 1, \text {i f} \xi_ {i} \leq \xi <   \xi_ {i + 1} \\ 0, \text {o t h e r w i s e ,} \end{array} \right. \tag {2}
$$

$$
\boldsymbol {b} _ {i, p} (\xi) = \frac {\xi - \xi_ {i}}{\xi_ {i + p} - \xi_ {i}} \boldsymbol {b} _ {i, p - 1} (\xi) + \frac {\xi_ {i + p + 1} - \xi}{\xi_ {i + p + 1} - \xi_ {i + 1}} \boldsymbol {b} _ {i + 1, p - 1} (\xi) \quad \text {i f} \xi_ {i} \leq \xi <   \xi_ {i + 1}, \tag {3}
$$

following the convention  $0 / 0 = 0$ . In this work,  $p = 3$ ,  $n = 11$ , and the knot vector  $[\xi_0,\xi_1,\dots ,\xi_{n + p}] = [0.0,0.0,0.0,0.0,0.125,0.25,0.375,0.5, 0.625,0.75,0.875,1.0,1.0,1.0,1.0]$ . To facilitate the assembly of honeycomb unit cells into a honeycomb array, a centrally symmetric B-spline curve is adopted as the edge of the honeycomb unit cell. In addition, the range of the x-coordinate and y-coordinate for the B-spline curve is [0.0, 0.5] and [-0.5, 0.5], respectively. Due to the central symmetry and boundary constraints, only 4 control points are variable, while the coordinates of the  $1^{\mathrm{st}}$ ,  $6^{\mathrm{th}}$ , and  $11^{\mathrm{th}}$  control points are fixed at (0.0, 0.0), (0.5, 0.0), and (1.0, 0.0), respectively. Furthermore, this modeling method can be used to generate previous honeycomb structures such as the super hexagonal honeycomb (Target-A in Fig. 1a) [76] and the horseshoe inspired honeycomb (Target-B in Fig. 1a) [35], meaning BSHs have a strong universality. In this study, the basic-edge length  $l$  of the unit cell of the BSH is set as  $16.67~\mathrm{mm}$ , and the height  $h$  of the BSH is  $28~\mathrm{mm}$ . The unit cell can be arranged appropriately to form a honeycomb array structure for the research of its mechanical properties, as depicted in Fig. 1b. To construct an initial training dataset, 5,000 distinct B-spline curves are generated to represent 5,000 BSHs with varying cross-sections. It is important to note that when constructing geometric models of BSHs, the coordinates of the control points should be multiplied by  $l$ . Finally, the relative density of the BSH can be given by

$$
\bar {\rho} = \frac {\rho}{\rho_ {s}} \tag {4}
$$

where  $\rho$  and  $\rho_{s}$  are the density of BSH and the density of the constitute material, respectively.

# 2.2. Energy absorption properties

Several energy absorption indexes, including PCF, MCF, SEA, and compression force efficiency (CFE), are employed to evaluate the energy absorption capabilities of different BSHs. The energy absorption (EA) of the BSH is quantified by the area under the corresponding compression force-displacement curve (the gray region shown in Fig. 2), which expression is

$$
\mathrm {E A} = \int_ {0} ^ {\delta_ {\mathrm {D}}} F (\delta) \mathrm {d} \delta \tag {5}
$$

where  $\delta$  signifies the compression displacement,  $\delta_{\mathrm{D}}$  represents the densification displacement, and  $F(\delta)$  denotes the compression force. To determine the parameter  $\delta_{\mathrm{D}}$ , the energy absorption efficiency  $\eta$  is denoted as

$$
\eta (\delta) = \frac {\int_ {0} ^ {\delta} F (\delta) \mathrm {d} \delta}{F _ {\max } \cdot h} \tag {6}
$$

The parameter  $\delta_{\mathrm{D}}$  is defined as the displacement at which  $\eta$  reaches its maximum value. In addition,  $F_{\mathrm{max}}$  signifies the maximum force when the displacement ranges between 0 and  $\delta$ . SEA serves as a pivotal metric for evaluating energy absorption performance and is expressed as

$$
\mathrm {S E A} = \frac {\mathrm {E A}}{m} \tag {7}
$$

where  $m$  is the mass of the BSH. As depicted in Fig. 2, PCF correlates with the initial buckling force of the BSH, a critical factor to regulate to prevent subjecting the protected object to excessive acceleration. By imposing an upper limit on the compression force, energy absorbers ensure that protected objects undergo a safe level of initial acceleration. This constraint aids in upholding the integrity and safety of the protected object while optimizing the energy absorption process. MCF characterizes the average load intensity of the energy absorbing structure within the densification displacement, which can be expressed as

$$
\mathrm {M C F} = \frac {\mathrm {E A}}{\delta_ {\mathrm {D}}} \tag {8}
$$

Moreover, CFE can reflect the uniformity of the load distribution during the energy absorption process, which is defined by

$$
\mathrm {C F E} = \frac {\mathrm {M C F}}{\mathrm {P C F}} \tag {9}
$$

The compression displacement efficiency (CDE) represents the compression height utilization ratio of the energy absorption structures, and the expression is

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/643118dce23f72932b9619211afa8523a6457363420635dbafb1c8982decd955.jpg)



Fig. 2. The energy absorption properties of the BSH.


$$
\mathrm {C D E} = \frac {\delta_ {\mathrm {D}}}{h} \tag {10}
$$

# 2.3. Simulation and experiment

The simulation method is applied to obtain the energy absorption properties of the initial BSH dataset, and the finite element (FE) models are constructed by the commercial software Ls-Dyna. Fig. 3 displays the scheme of the FE model for the honeycomb structure. The Belytschko-Tsay shell elements with 5 integration points through shell thickness are used to discretize the BSH, and the average mesh size is  $0.7\mathrm{mm}$  to balance the computational cost and the sufficient accuracy (see Fig. S2a~b). In addition, the Belytschko-Tsay shell elements with 2 integration points through shell thickness are also used to discretize the plate, while the average mesh size is  $10\mathrm{mm}$ . The constituent material of the honeycomb structure, aluminum alloy AA1060-H112, is simplified by piecewise-linear plasticity material model (MAT 24) with elastic and plastic hardening properties. The basic material parameters are listed in Table 1, and the plastic hardening is defined by the effective stress-effective plastic strain curve shown in Fig. S1. The rigid model (MAT 20) is applied to the punch plate and support plate since their deformation can be ignored. To simulate the compression progress, the velocity control method along the z-axis is applied on the upper punch plate, while the lower support plate is fixed at all 6 degrees of freedom. It is important to note that the kinetic energy should be insignificant compared with the internal energy of the BSH to ensure the simulation of quasi-static condition [77]. In addition, the impact of strain rate on the mechanical behavior of AA1060 appears negligible unless subjected to exceptionally high strain rates [78]. Therefore, the velocity applied on the upper punch plate is  $1.0\mathrm{m / s}$  to balance the computational cost and sufficient accuracy (see Fig. S2c~d and Fig. S3). The stiffness-based hourglass control method is adopted in the finite element model to eliminate the effect of zero energy mode deformation resulting from the reduced integration elements. The Automatic Node to Surface contact condition is set between the BSH and two plates, where the nodes of the BSH are chosen as slave nodes, while the contact surfaces of two rigid plates are chosen as master surfaces. In addition, two tiny gaps are set between the two plates and the BSH to prevent the initial penetration. The Automatic Single Surface contact is applied to the BSH to avoid penetration and intersection between the honeycomb walls. The static and dynamic coefficients of friction are 0.2 equally [79].

Quasi-static compression experiments were conducted to validate the accuracy of the simulation model. As illustrated in Fig. 4a~b, two types of honeycomb specimens are fabricated using the wire-cut electrical discharge machining (WEDM) technique, known for its precision in producing thin-wall structures and cost-effectiveness compared to additive manufacturing methods. The experimental THH and the BSH have wall thicknesses of  $0.36\mathrm{mm}$  and  $0.45\mathrm{mm}$ , respectively. Additionally, both experimental honeycombs have a height of  $28\mathrm{mm}$  and a basic-edge length of  $16.67\mathrm{mm}$ , and the control points of the experimental BSH are detailed in Table S1. As illustrated in Fig. 4c, the tests were conducted using an electronic material testing machine with a load cell of  $100\mathrm{kN}$  at room temperature and normal humidity, and honeycombs were free contact with upper and bottom plates. In addition, the

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/19d0b07ae16fbfba8c3f3f02fb741cfffff6851c20b798950e987432171817b9.jpg)



Fig. 3. The FE model of the honeycomb.



Table 1 Material parameters of the aluminum alloy AA1060-H112 [76].


<table><tr><td>Young&#x27;s modulus E (GPa)</td><td>Yield stress σy (MPa)</td><td>Density ρs (g/cm3)</td><td>Poisson&#x27;s ratioν</td></tr><tr><td>69</td><td>33.42</td><td>2.70</td><td>0.33</td></tr></table>

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/d6d782a81e1aa43877c6c832cbf6f874b0a108df091bcd0be282e71f56b2b65a.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/5e346f80d323d9d50a22f5d360ef8f881335ab1060696faa5556643623b33b4e.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/0b264f8a5870a8bbfde80ca056c30bcbeefa386a12f59bc19f9d07eb6d47bede.jpg)



Fig. 4. Quasi-static compression experiment for honeycombs: (a) THH; (b) BSH; (c) Testing machine.


compression speed was set to  $2.0\mathrm{mm / min}$  to meet the quasi-static loading condition, and the compression force and displacement were recorded by the testing machine.

The out-of-plane compression mechanical response of honeycombs can be classified into four stages based on their deformation state. Stage I corresponds to the elastic stage, which occurs at the initial phase of the compression process. During this stage, the compression force applied on honeycomb increases linearly with displacement. As the stress distributed across the honeycombs exceeds the yield stress of the constituent material, the deformation state transitions to stage II, known as the yield and buckling stage. In this stage, plastic deformation is initiated within the honeycombs, and the first buckle emerges once the compression force surpasses the buckling force, corresponding to the PCF. Subsequently, the deformation state progresses to stage III, referred to as the progressive collapse stage, which dissipates a significant amount of impact kinetic energy. Multiple plastic hinge lines manifest on the honeycombs, causing the compression force to fluctuate around the MCF. Ultimately, the honeycombs enter stage IV, designated as the

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/b45c9dc277f47611e2804ba71e66315b70601e17357a453e5ed48f218561b0f7.jpg)



Fig. 5. Comparison of the force-displacement curves obtained by experiment and simulation.


densification stage, leading to a sharp rise in the compression force.

As illustrated in Fig. 5, for the THH and the BSH, the force-displacement curves obtained from both experimental and simulation data exhibit a notable similarity. The obvious discrepancy arises in the densification stage due to the contact algorithm of shell element, while the FE model utilizing solid elements displays superior performance in this stage (see Fig. S4). However, the computational expense associated with the FE model employing solid elements for thin-walled structures is significant due to the requirement for a fine mesh size along the wall direction. On the other hand, the FE model using shell elements demonstrates better capability in mirroring the deformation mode of honeycombs. Both the experimental specimens and the FE models exhibit progressive collapse as the deformation mode of the honeycombs, as shown in Fig. 6. The initial buckling positions on the experimental specimens are random due to the stochastic distribution of fragile regions [76,80], thereby influencing the subsequent location of the plastic hinge lines. Consequently, slight variations may arise between the deformation processes obtained from experiments and FE models. For instance, in the case of the THH, the experimental results indicate an initial buckling position at the middle region, whereas the FE model predicts an initial buckling position at the top region. Similarly, for the BSH, the experimental observations reveal initial buckling positions at both the middle and top parts of the honeycombs, while the FE model indicates an initial buckling position solely at the middle region of the honeycomb. Fortunately, the influence of the FE model on predicting energy absorption properties, including the PCF, MCF, and SEA, is negligible, which is supported by the observation in Fig. 5. As shown in Table 2, the relative error of PCF for the THH is  $7.59\%$  which is the maximum relative error between the results obtained the experiment and simulation, while other relative errors remain below  $5\%$ . Consequently, FEM proves to be an efficient tool for accurately predicting the mechanical performance of honeycombs. Therefore, FEM is employed to construct a comprehensive dataset for BSHs, which can effectively reduce research costs.

# 3. Data-driven optimization design

This section presents the architecture of the DNN models used to predict relative density, PCF, MCF, and SEA, and constructs an optimization design framework combined with the genetic algorithm.


Table 2 Comparisons of the energy absorption metrics obtained by experiment and simulation.


<table><tr><td>Metric</td><td>THH-EXP</td><td>THH-FEM</td><td>Relative error</td><td>BSH-EXP</td><td>BSH-FEM</td><td>Relative error</td></tr><tr><td>PCF (kN)</td><td>6.46</td><td>6.95</td><td>7.59%</td><td>18.57</td><td>19.21</td><td>3.45%</td></tr><tr><td>MCF (kN)</td><td>3.12</td><td>3.02</td><td>3.21%</td><td>9.12</td><td>9.07</td><td>0.55%</td></tr><tr><td>SEA (J/g)</td><td>4.92</td><td>5.15</td><td>4.67%</td><td>6.38</td><td>6.45</td><td>1.10%</td></tr></table>

# 3.1. Neural network model training

In this work, the construction of DNN models was performed using Keras with a TensorFlow backend, utilizing Python 3.9. Fig. 7 illustrates the architecture of the DNN models, where the input layer consists of 9 neurons representing the thickness and control points coordinates of the BSH. The output layer comprises a single neuron that represents properties of the BSH, such as relative density, PCF, MCF, and SEA. As characteristics of neural networks, the number of hidden layers and the number of neurons within each hidden layer are hyperparameters of the DNN model, which are dependent on the specific property being predicted. Each hidden layer is composed of a dense layer, a batch normalization layer, and an activation layer. The dense layer facilitates intricate mappings between the input and output spaces through weight parameters and bias terms. By standardizing the output of dense layer, the batch normalization layer enhances network stability and convergence, resulting in faster and more robust training. Moreover, it mitigates challenges associated with vanishing and exploding gradients commonly encountered in deep architectures. The activation layer introduces non-linearities into the neural network model, enabling the modeling of complex relationships between inputs and outputs. In this study, the LeakyReLU function was chosen as the activation function for its computational efficiency and ability to prevent complete inactivity of neurons. The expression of the LeakyReLU function is

$$
\operatorname {L e a k y R e L U} (x) = \left\{ \begin{array}{l l} x, & x > 0 \\ a x, & x \leq 0 \end{array} \right. \tag {11}
$$

Here,  $\alpha$  is set to 0.1.

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/62ee84d9f232686576d0ee985878338b38a73b8dfc41fc88e534d49789cd9540.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/a2d8343126bea256f1744d32e158ca5b69da9a993b49dedf09b5c495a16717d2.jpg)



Fig. 6. The deformation process of the honeycombs obtained by the quasi-static experiment and FE model: (a) THH; (b) BSH.


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/f15b1855e577f9404120d26eb4483675d0330c88ef1b0dd65219d71ed80c7cbb.jpg)



Fig. 7. Architecture of the DNN model.


To assess the training accuracy of the DNN model, a loss function was employed to optimize the parameters of model during the training iterations. The mean absolute percentage error (MAPE) was selected as the loss function, expressed as

$$
\mathrm {MAPE} = \frac {100 \%}{N} \sum_ {i = 1} ^ {N} \frac {\left| \widehat {y} _ {i} - y _ {i} \right|}{\max \left(\left| y _ {i} \right| , 10^{-5}\right)} \tag{12}
$$

where  $N,\widehat{y}_i$ , and  $y_{i}$  denote total amount of data, the  $i$ -th predicted label, and the  $i$ -th actual label, respectively. The adaptive moment estimation (ADAM) optimizer was selected for minimizing the MAPE in this study. The initial learning rate was set to 0.001, which was reduced by a factor of 0.1 every 1000 epochs. A batch size of 1024 and a total of 2000 epochs were used. The initial datasets were divided into a training, a validation, and a test set with a ratio of 8:1:1, and the validation set was merged into the training set after adjusting the hyperparameters of the DNN models. Besides, it is important that the BSHs in the training set and the validation set have similar distributions which means a better consistency (see Fig. S6). The best trained model, which exhibited the lowest train loss and test loss compared to the previous models, was saved for subsequent analysis. Four distinct DNN models were trained to predict the relative density, PCF, MCF, and SEA of the BSH, respectively. The number of hidden layers and neurons within each hidden layer were determined through multiple training trials based on the performance of the DNN model on the validation set (see Section S2). Table 3 displays the architectures of the DNN models utilized for relative density, PCF, MCF, and SEA predictions. Since relative density strongly correlates with the structural design parameters, the DNN model for relative density prediction adopted a relatively simple architecture. Similarly, the PCF, which corresponds to the first buckling mode, can be determined with a simplified DNN model structure due to the simple plastic deformation characteristics of the BSH. However, the MCF and SEA of the BSH are influenced by various factors, such as the contact state during the compression process. As a result, the MCF and SEA of the BSH exhibit complex relationships with the structural design parameters. Therefore, the development of an effective DNN model necessitates a greater number of hidden layers to capture the intricate relationships


Table 3 Structure parameters of the DNN models for different prediction.


<table><tr><td>Prediction</td><td>Input layer</td><td>Hidden layers</td><td>Output layer</td></tr><tr><td>ρ</td><td>9</td><td>(512,512,1024,1024)</td><td>1</td></tr><tr><td>PCF</td><td>9</td><td>(1024,1024,1024,2048,2048,2048)</td><td>1</td></tr><tr><td>MCF</td><td>9</td><td>(1024,1024,1024,1024,1024,1024,1024)</td><td>1</td></tr><tr><td>SEA</td><td>9</td><td>(1024,1024,1024,1024,1024,1024,1024)</td><td>1</td></tr></table>

and patterns associated with MCF and SEA.

Generally, prediction accuracy tends to improve with the expansion of the training dataset size. However, a marginal effect is observed, where each additional unit of a training sample diminishes its contribution to the refinement of the DNN model. The MAPE shown in Fig. 8 represent the average across three DNN models, aiming to decrease the variability induced by random weights initialization. With the training dataset size expansion, the MAPEs of the DNN models in predicting relative density, PCF, MCF, and SEA demonstrate a progressive decrease, ultimately approaching a plateau. This marginal effect results in a substantial computational cost to enhance the performance of the DNN models. The training dataset comprising 1000 samples can yield the MAPEs of the DNN models for predicting the relative density and PCF on the test dataset below  $1.53\%$  and  $3.54\%$ , respectively, indicative of excellent predictive capabilities. Nevertheless, the DNN models for predicting MCF and SEA exhibit larger MAPEs, reaching  $7.55\%$  and  $6.96\%$ , respectively, when the training dataset size amounts to 4000 samples. Fig. 9a~d illustrates the training process of the DNN models for predicting relative density, PCF, MCF, and SEA, respectively. Typically, the MAPE on test dataset surpasses that of the training dataset. However, owing to the inclusion of batch normalization layers and the relatively limited size of the test dataset, the DNN model for predicting relative density has a lower MAPE on the test dataset than training dataset. Upon removing all batch normalization layers from hidden layers, the MAPE of the DNN model for predicting relative density is anticipated to be

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/4eeece492285299ed7f055ae6a80f193820fcf19be1be5fefbe5fd656078deae.jpg)



Fig. 8. The convergence study on training set size.


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/ebb4a563906ed4b598b4609d5a8ba4303b299c5a049094e527ef0e274dafad1c.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/c43077f7c2ed998044090cb8ca1d9b200388e3e1217cc393d807742bceab8eb7.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/f27d1da9d88cb64d64c586d2d317df3d805af7bea43427b2376ee7cf3f257370.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/b975ef2956e6a964a1c8deadda97478b55533331183ffeb04f4c1106204d85bd.jpg)



Fig. 9. MAPE-epochs curve of different DNN models: (a) Relative density; (b) PCF; (c) MCF; (d) SEA.


higher on the training set in contrast to the test set (see Fig. S7). In contrast to the DNN models for predicting relative density and PCF, discernible discrepancies in MAPEs between the training dataset and the test dataset are observed for the DNN models predicting MCF and SEA. These distinctions emphasize that the MCF and SEA have a complex nonlinear relationship with structural design parameters. The trained DNN models exhibit enhanced efficiency in predicting the mechanical characteristics of BSHs, boasting a speed approximately 300 times faster than that of the FE model (see Table S6). Besides, the elapsed time required by DNN models for predicting properties of one sample or 4500 samples remains nearly identical due to parallel computing, indicating significant superiority in calculating the energy absorption performance of numerous samples.

# 3.2. Optimization design framework

The DNN models can predict the relative density, PCF, MCF, and SEA of BSHs with a high accuracy, but they cannot select the proper BSHs which meet the design diamonds automatically. Genetic algorithm (GA), an optimization method inspired by the principles of natural selection on genetics, mimic the evolutionary process to excellently solve global optimization issues by efficiently exploring the design space. There are three genetic operators, selection, crossover, and mutation, to manipulate the chromosome corresponding to an individual, which increase the mean fitness of the whole population and search for the individual with the largest fitness. Compared with particle swarm optimization algorithm (PSO), GA demonstrates superior computational efficiency and capability of escaping local optima (see Section S3). Therefore, the combination of the DNN model and the GA is a powerful strategy to find the design boundary or the best configuration under special design constraint conditions, and the design framework is shown in Fig. 10. As mentioned in Section 3.1, there is a marginal effect while increasing the number of the initial dataset to enhance the predicting accuracy of the

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/91bf30926140f531323eae62686e4e1b8a0c82c3544b554651f3996394ddfc7d.jpg)



Fig. 10. Optimization design framework of BSHs based on DNN model and GA.


DNN model. The accuracies for predicting relative density and PCF are high enough, but that of MCF and SEA are still needed to increase. Therefore, to enhance the predicting accuracy around the target regions and obtain the design target samples with a relatively small initial dataset size, a loop structure and data augmentation method are introduced to the framework. The loop is not stopped until the structural parameters and FEM results of the new samples generated by the GA are converged to that of the previous samples. In addition, the data augmentation copies one sample to 10 samples to enlarge the proportion in the training dataset, leading to a relative higher predicting accuracy on these newly generated samples. The definition of the fitness function, depending on the design target, is the most important criterion on the selection part, which significantly influences the results of the generated new samples. For instance, if the design target is to find the upper SEA design boundary of the BSHs with different relative density, the fitness function can be defined as

$$
F (\bar {\rho}, \text {S E A}) = k | \bar {\rho} - \bar {\rho} _ {0} | + \text {S E A} \tag {13}
$$

where  $\overline{\rho}_0$  is the target design relative density of the BSH, and  $k$  is the penalty coefficient. By adjusting  $k$  to a negative or positive value, the converged BSH have the maximum or minimum SEA with the relative density of  $\overline{\rho}_0$ . By ranging  $\overline{\rho}_0$  from  $\overline{\rho}_1$  to  $\overline{\rho}_2$ , the upper SEA design boundary of BSH with the relative density between  $\overline{\rho}_1$  and  $\overline{\rho}_2$  can be found. Similarly, if design target has two constraint conditions, such as constraint the relative density and PCF, the fitness function can be defined as

$$
F (\bar {\rho}, \mathrm {P C F}, \mathrm {S E A}) = k \left(\operatorname {R e L U} \left(\bar {\rho} - \bar {\rho} _ {0}\right) + \operatorname {R e L U} \left(\mathrm {P C F} - \mathrm {P C F} _ {0}\right)\right) + \mathrm {S E A} \tag {14}
$$

where  $\mathrm{PCF_0}$  is the target design initial peak compression force of the BSH and the expression of ReLU function is given by

$$
\operatorname {R e L U} (x) = \left\{ \begin{array}{l l} x, & x > 0 \\ 0, & x \leq 0 \end{array} \right. \tag {15}
$$

Through this fitness function, GA can select the samples with the maximum SEA under the control of the relative density and PCF.

# 4. Results and discussions

In this section, the upper design boundaries of BSHs are determined and discussed. Additionally, empirical equations used to predict the PCF, MCF, CDE, and SEA of BSHs positioned at the upper SEA design boundary are summarized from the dataset. Subsequently, the configurations and deformation mechanisms of the optimal BSHs with varying relative densities are examined. Finally, comparisons are made between the energy absorption capacities of BSHs and those of commonly utilized energy absorbing materials and structures.

# 4.1. The upper design boundaries of BSHs

Previous studies have demonstrated that the cross-sectional shapes of the honeycombs significantly influence their energy absorption performance. Therefore, it is interesting to explore whether a specific configuration exists that leads to optimal energy absorption properties under varying relative densities. Using the optimization design framework mentioned in Section 3.2, it is easy to obtain the upper SEA design boundary of BSHs across different relative densities while employing Eq. (13) as the fitness function. In addition, choosing  $k = -5$  is sufficient to make the relative density of BSH converge to the desired target with tiny error. The mass of BSH is explored within a search range of  $10\mathrm{g}$  to  $70\mathrm{g}$ , corresponding to relative densities spanning from  $2.6\%$  to  $18.3\%$ . As shown in Fig. 11a, the 5000 initial samples and 577 GA generated samples are represented by the black and red points, respectively. Evidently, the DNN-GA based design methodology significantly expands the design boundaries, leading to a substantial enhancement in SEA for samples within the GA set compared to those with equivalent relative densities in the initial set. The dark blue line (DNN-BD) is the upper SEA design boundary predicted by the DNN model with a convex shape,

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/7e33d263f966e4bccf69375893b3de69591b38733d2e085f127497daf8d581b6.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/7476b344e958787dd42c77e5ca2628dfc3fa03fc213c9f586ec10961eedd18ea.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/3133def41ad5eba94296b40e1c37f69508ce5eac227935ef07d7b91706c1327a.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/3478c9886cd01b355f07d392d61abda603b8ebe6877fb2f1aa3f6dcb37022abd.jpg)



Fig. 11. The upper design boundary for the BSH: (a) SEA; (b) PCF; (c) MCF; (d) CDE. DNN-BD represents the upper design boundary predicted by DNN model.


indicating an initial increase followed by a decrease in SEA with rising relative density. It has the same tendency with the upper SEA design boundary described by the samples in the GA set, and it also aligns with the upper SEA design boundary defined by the randomly generated initial set. For relative densities below  $10.5\%$ , the upper SEA design boundary is influenced by both the cross-sectional shape and the thickness. However, due to a design space restricting the thickness between  $0.2\mathrm{mm}$  and  $0.6\mathrm{mm}$ , the upper SEA design boundary for BSHs with relative densities exceeding  $10.5\%$  is solely determined by the cross-sectional shape. It is a critical factor that impacts the improvement of the energy absorption performance.

At a defined relative density, it is consistently observed that the BSH with the highest SEA tends to exhibit the largest PCF (see the  $\mathrm{SEA}_{\mathrm{max}}$  set in Fig. S9a). As illustrated in Fig. 11b, the upper boundary of PCF has an obviously linear correlation with the relative density when the relative density is below  $15.7\%$ . This relationship is substantiated by the initial set, GA set, and the boundary predicted by the DNN model. Due to the constraints within the design space, the PCF of BSHs with the relative densities exceeding  $15.7\%$  fails to reach the practical boundary. By expanding the permissible thickness range to  $0.2\mathrm{mm}$  to  $0.8\mathrm{mm}$ , the PCF of BSHs with relative densities surpassing  $15.7\%$  can achieve values conducive to reaching practical limits (see the  $\mathrm{GA}_{\mathrm{add}}$  set in Fig. S9a). Through linear regression fitting of boundary samples (see Fitting-BD in Fig. S9a), a boundary function can be formulated as

$$
\mathrm {P C F} _ {\mathrm {B D}} = 3. 1 4 8 5 \bar {\rho} - 1. 3 0 4 6 \tag {16}
$$

where  $\mathrm{PCF_{BD}}$  is the upper PCF boundary of BSH with a relative density  $\overline{\rho}$ . Similarly, the BSHs sharing the same relative density always tend to have the largest MCF to achieve the highest SEA (see the  $\mathrm{SEA}_{\mathrm{max}}$  set in Fig. S9b). The upper MCF boundary of the BSHs also shows a linear relationship with the relative density, as shown in Fig. 11c. In the design space, this boundary can be approximated by three linear functions (see the Fitting-BD in Fig. S9b), which expression is

$$
\mathrm{MCF}_{\mathrm{BD}} = \left\{ \begin{array}{ll}2.7340\bar{\rho} -4.0326, & 2.6\% \leq \bar{\rho} <  9.2\% \\ 1.8099\bar{\rho} +4.4691, & 9.2\% \leq \bar{\rho} <  14.5\% \\ 0.2431\bar{\rho} +27.1877, & 14.5\% \leq \bar{\rho}\leq 18.3\% \end{array} \right. \tag{17}
$$

where  $\mathrm{MCF}_{\mathrm{BD}}$  is the upper MCF boundary of BSH with a relative density  $\overline{\rho}$ . However, the CDE of the GA set does not align precisely with the boundary of the entire sample set, indicating that BSHs with the highest SEA do not necessarily require maximum CDE. Although the relationship between the CDE of the BSH with the largest SEA and the corresponding relative density is not a prefect linear relationship (see the  $\mathrm{SEA}_{\mathrm{max}}$  set in Fig. S9c), the whole tendency is the CDE decreases with the increase of the relative density. Therefore, a linear function can be employed to simplify this relationship (see the Fitting in Fig. S9c), which can be defined as

$$
\mathrm {C D E} _ {\mathrm {B D}} = - 0. 4 8 2 3 \bar {\rho} + 8 2. 4 6 3 3 \tag {18}
$$

where  $\mathrm{CDE}_{\mathrm{BD}}$  is the CDE of the BSH on the upper SEA boundary. Additionally, referring to Eq. (7), the SEA of the BSH can be expressed as

$$
\mathrm {S E A} _ {\mathrm {B D}} = \frac {\mathrm {M C F} _ {\mathrm {B D}} \times \mathrm {C D E} _ {\mathrm {B D}} \times h}{\bar {\rho} \times m _ {0}} \tag {19}
$$

where  $m_0$  represents the mass of the component enclosed by the BSH, with the material of the component aligning with the constituent material of the BSH. By substituting Eq. (17) and (18) to Eq. (19), Eq. (19) can be rewritten as

$$
\mathrm {SEA} _ {\mathrm {BD}} = \left\{ \begin{array}{l l} - 0.0967 \bar {\rho} - 24.3748 \frac {1}{\bar {\rho}} + 16.6680, & 2.6 \% \leq \bar {\rho} <   9.2 \% \\ - 0.0637 \bar {\rho} + 27.0132 \frac {1}{\bar {\rho}} + 10.7818, & 9.2 \% \leq \bar {\rho} <   14.5 \% \\ - 0.0086 \bar {\rho} + 164.3342 \frac {1}{\bar {\rho}} + 0.5083, & 14.5 \% \leq \bar {\rho} \leq 18.3 \% \end{array} \right. \tag{20}
$$

Eq. (20) is the empirical equation for the upper SEA boundary of BSHs, and the corresponding empirical boundary curve is illustrated in Fig. 12, exhibiting close alignment with boundaries determined by the FEM results and DNN results. The maximum SEA calculated by the FE model is  $13.41\mathrm{J / g}$ , while the maximum SEA predicted by the empirical equation is  $13.13\mathrm{J / g}$ , with a prediction error of just  $2.1\%$ . In the absence of design space constraints, the  $\mathrm{SEA}_{\mathrm{BD}}$  can be modified to

$$
\mathrm {SEA} _ {\mathrm {BD}} = - 0.0967 \bar {\rho} - 24.3748 \frac {1}{\bar {\rho}} + 16.6680, 2.6 \% \leq \bar {\rho} \leq 18.3 \% \tag{21}
$$

which only has the first function of Eq. (20) for the whole relative density range, resulting in a maximum SEA of  $13.60~\mathrm{J / g}$  at relative density of  $15.88\%$ . Consequently, the value of the red star on the orange dotted line in Fig. 12 can be seen as the empirical maximum SEA of BSHs.

# 4.2. The configurations and energy absorption mechanisms of the optimal BSHs

In Section 4.1, the upper SEA design boundary of BSHs the specified design constraints is introduced. This boundary provides valuable insights into exploring the maximum achievable SEA for BSHs. Furthermore, it is crucial to investigate the optimal configurations of BSHs across various relative densities and to comprehend the underlying design strategy embedded within the design boundary. Fig. 13 illustrates the representative dominated configurations of the optimal BSHs at different relative densities. It is noteworthy that BSHs with identical configurations type but varying relative densities exhibit minor variations in cross-sectional shape or thickness. The BSHs with a bowl shape, as depicted in Fig. 13a, demonstrate peak performance within a narrow relative density range of  $2.6\%$  to  $3.0\%$ . As the relative density exceeds  $3.0\%$  but remains below  $7.3\%$ , the optimal configuration transitions to 30-sided BSHs, as shown in Fig. 13b, which can be seen as a self-similar vertex hierarchy of THH. Fig. 13c illustrates the 5-shaped BSHs, excelling in SEA within the relative density bracket of  $7.3\%$  to  $9.6\%$ . It is

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/17d6ba8f230beb8188a1b9111fbf2f31b9dfcab5d9ef4e5e48b1523fcf107a4b.jpg)



Fig. 12. The empirical upper design boundary (EMP-BD) for the BSH.



(a)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/6a2900e373a30ec8ce6a87f531cb975297e312ce267992b95e6d34bcff59b425.jpg)



(b)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/2318f64744a5ec942c887d9a26c251ef140690affa5e0c4f0b70f329e084fe0d.jpg)



(c)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/0a62aade94d378aba77b17140735405876e8409d50a0e22e7c06be35ed25d699.jpg)



(d)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/a291e3fe822aa3f0a26a2ef217ec658a9724ad9703cf5f974589473b24a8b410.jpg)



(e)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/8b030eb9aae8ad99049f029a2b3721fd5b4dd819de33d70d8c76c72fe94a2659.jpg)



(f)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/e812d9ec53d3f811a479015b1aa2d0d5ab27e1e6da39669821b1fc3929f01a0b.jpg)



Fig. 13. The optimal configuration of the BSH for different relative density range: (a)  $\overline{\rho} \in [2.6\%, 3.0\%)$ ; (b)  $\overline{\rho} \in [3.0\%, 7.3\%)$ ; (c)  $\overline{\rho} \in [7.3\%, 9.6\%)$ ; (d)  $\overline{\rho} \in [9.6\%, 10.9\%)$ ; (e)  $\overline{\rho} \in [10.9\%, 13.4\%)$ ; (f)  $\overline{\rho} \in [13.4\%, 18.3\%]$ .


worth mentioning that the BSH featuring the 5-shaped configuration achieves the best energy absorption performance within the design space, with an SEA of  $13.41\mathrm{J / g}$ . As illustrated in Fig. 13d, the 2-shaped BSHs position along the upper SEA design boundary for relative densities ranging from  $9.6\%$  to  $10.9\%$ . With an increase in relative density, the optimal configuration of BSHs transitions to the M-shape, as shown in Fig. 13e, which demonstrates superior performance within the relative density range of  $10.9\%$  to  $13.4\%$ . The BSH depicted in Fig. 13f can be denoted as an  $r$ -shaped BSH, resembling the M-shaped BSH. The primary distinction lies in the wavy half-edge of the  $r$ -shaped BSH extending to the opposite side of the baseline, a feature does not present in the M-shaped BSH.

After identifying BSHs with the highest SEA, it is crucial to delve into the reasons behind their exceptional energy absorption capabilities. For analytical convenience, these configurations are segregated into two groups, including the BSHs on the ascending and declining stages of the upper SEA design boundary. Fig. 14 depicts the force-displacement curve and deformation mode for BSHs positioned at the ascending stage of the upper SEA design boundary. Generally, the deformation behavior of honeycombs can be categorized into local irregular bending deformation and progressive folding deformation (see Fig. S11a). The deformation mode of the bowl-shaped BSH follows the progressive collapse mode when the compression strain is below 0.39, transitioning to local irregular bending beyond this threshold (see Fig. S12a). The local irregular bending leads to a reduction in compression force and incomplete folding of the thin walls of the BSH, negatively impacting energy absorption efficiency. Similarly, as shown in Fig. 14b, the 30-sided BSH undergoes transitional deformation mode, encompassing progressive collapse and local irregular bending deformation with a

critical compression strain of 0.43. In contrast, the 5-shaped BSH, boasting the highest SEA, tends towards a full fold deformation mode, with only partial outer edges irregular bending which have negligible influence on the compression force. Moreover, the 5-shaped BSH exhibits a small and uniformly distributed folding wavelength, resulting in the formation of 6-9 plastic hinge lines along the height direction. As shown in Fig. 15, the deformation states of the 2-shaped BSH, the M-shaped BSH and the  $r$ -shaped BSH are similar with that of the 5-shaped BSH, with progressive folding deformation dominating the deformation patterns. During this stage, the relative density is primarily adjusted by altering the length of the B-spline edges due to wall thickness constraints. Notably, wall thickness significantly influences the EA of BSHs, with the rate of EA increase slowing as the wall thickness approaches its upper limit (see Fig. S14). Beyond a relative density of  $14.5\%$  enhancing the EA of BSHs through adjustments to cross-sectional shape becomes challenges. Therefore, achieving optimal SEA involves a delicate balance between wall thickness and the cross-sectional shape. Thicker wall thickness poses the risk of inducing global buckling in BSH, consequently reducing MCF and SEA of BSH.

Despite the intricate nonlinear characteristics during the post-buckling and large plastic deformation of BSHs under out-of-plane compression force, the super folding element theory [80] can elucidate the mechanism enhancing the energy absorption of BSHs. Super folding elements, such as V-shaped element, T-shaped element, Y-shaped element, and X-shaped element, absorb energy through bending deformation around static hinge lines, rolling of moving hinge lines, and membrane deformation during the formation of toroidal surfaces. The folding wavelength and mode of these super folding elements depend on their geometric parameters, such as the included angle and wall thickness [80]. In contrast to traditional honeycombs composed of straight lines, a BSH typically incorporates various super folding elements with curved edges of different curvatures, resulting in multiple folding directions on a B-spline edge simultaneously. This characteristic grants BSHs the flexibility to enhance energy absorption performances of different super folding elements by increasing energy dissipation through plastic deformation in bending, rolling, and membrane areas. Notably, the highest stress and plastic strain often occur along the plastic hinge lines and inner intersection lines of super folding elements (see Fig. S11). Consequently, an optimal BSH should exhibit specific characteristics aimed at achieving complete plastic deformation and uniform stress distribution. Firstly, the deformation mode of the BSH should approach progressive collapse. Secondly, the BSH should strike a suitable combination of cross-sectional shape and wall thickness for super folding elements to reduce the folding wavelength and expand the bending, rolling, membrane areas.

# 4.3. Validation of the DNN-GA optimization design framework

Given the substantial cost implications associated with conducting a high volume of experiments, the dataset utilized in this study primarily relied on FEM. Therefore, it is inevitable that the energy absorption properties derived from DNN models based on FEM may exhibit discrepancies when compared to experimental outcomes. To enhance the practical utility for engineering applications, the energy absorption characteristics of BSHs featuring cross-sectional shapes optimized through the DNN-GA framework were compared with corresponding experimental data. For enhanced representativeness, BSH with specific cross-sectional shape, namely the 30-sided BSH and the M-shaped BSH, were chosen to represent the BSHs positioned at the ascending and declining stage of the upper SEA design boundary, respectively. The control points information for the experiment samples is detailed in Table S8 and Table S11, with thin-walled thicknesses specified as 0.37 mm and 0.53 mm, respectively. All parameters in both simulation and experiment were meticulously maintained in accordance with Section 2.3. The structural failure was not observed during the whole compression process (see Fig. S17). As depicted in Fig. 16a, the forces

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/02089cbdcde6d7282128ef469a2158f73c3fd0d3ede5b2dbe9e28227b3e56198.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/75c33a2b5a6b64280819b032e4ced72548dcf69d32beae8e6e94c2638ffe8d97.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/1d2082c59ace4be47c467ca51dfeebf55b2e3828d97f6895cceecec00ea141c3.jpg)



Fig. 14. The force-displacement curve and deformation mode for BSHs positioned at the ascending stage of the upper SEA design boundary: (a) Bowl-shaped BSH; (b) 30-sided BSH; (c) 5-shaped BSH.


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/24ca6c2029fb4da3398e33d899ed256b31ed3142b65a65c90ab701a47edfd8fa.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/aed80d98abea64ff83920de9951fdd7ee80dc84fc8a9928bb1d8acbd080a22e9.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/06f9216daf85dfe9bbc7dea63d1ea4d8b6f1d908d29a71ed2ead56d8bc8dc98b.jpg)



Fig. 15. The force-displacement curve and deformation mode for BSHs positioned at the declining stage of the upper SEA design boundary: (a)2-shaped BSH; (b) M-shaped BSH; (c)  $r$ -shaped BSH.


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/ddfef1b1c78940a137e1ce9be57faffa6de577496024ad57cd341e58f3702ff7.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/7f7192e3f20b3971f3265c87a4d07c7d96ee889a1f15c3d4b23458fe3b966bf8.jpg)



Fig. 16. Comparison of FEM and experiments: (a) Force-displacement curves; (b) Final deformation state of 30-sided BSH; (c) Final deformation state of M-shaped BSH.


acting on the BSHs obtained by experiment and FEM exhibit similarity across the elastic stage, yield and buckling stage, and progressive collapse stage, while demonstrate obvious disparities in the densification stage. This is similar with the results demonstrated in Fig. 5 and Section 2.3. As illustrated in Fig.  $16\mathrm{b}\sim \mathrm{c}$ , the area of the local irregular bending region on the 30-sided BSH in experiment is smaller than that in FEM, which is contrast with observations for the M-shaped BSH. The MCF of the 30-sided BSH exhibits a larger relative error of  $10.94\%$  when comparing the results of experiment and simulation, as detailed in Table 4. Furthermore, the FEM underestimates the SEA of the 30-sided BSH in contrast to experimental data, despite the FEM yielding an efficient compression displacement of  $22.32\mathrm{mm}$ , surpassing the  $20.72\mathrm{mm}$  recorded in experiment. Conversely, the SEA of the M-shaped BSH is overestimated by the FEM, even though the FEM accurately estimates the MCF. This discrepancy can be attributed to the fact that the efficient compression displacement obtained by FEM amounts to  $21.40\mathrm{mm}$ , exceeding the experimental value of  $19.57\mathrm{mm}$ . Compared with experiments, the PCFs of both the 30-sided BSH and M-shaped BSH predicted by the FEM exhibit minor relative errors, each falling below  $2.0\%$ . Notably, both the SEA of the 30-sided BSH and M-shaped BSH surpass those of previous polyline/curve honeycomb designs, such as the horseshoe inspired honeycomb with  $8.75\mathrm{J/g}$  [35], the super hexagonal honeycomb with  $8.05\mathrm{J/g}$  [76], and the wavy hexagonal honeycomb with  $5.30\mathrm{J/g}$  [33]. Consequently, the DNN-GA optimization design framework emerges as a valuable tool for offering direction in the creation of energy absorbers with specified performance metrics in practical applications. Moreover, experiments can supersede simulations in the loop of the DNN-GA optimization design framework to enhance the accuracy of optimization, thereby achieving a balance between design precision and cost.

# 4.4. Comparison of energy absorption property with various energy absorption structures

As shown in Fig. 17a, the SEAs of the BSHs are compared with


Table 4 Comparisons of the energy absorption metrics obtained by experiment and simulation.


<table><tr><td>Metric</td><td>Mass (g)</td><td>PCF (kN)</td><td>MCF (kN)</td><td>SEA (J/g)</td></tr><tr><td>30-sided BSH-EXP</td><td>19.40</td><td>15.16</td><td>10.69</td><td>11.41</td></tr><tr><td>30-sided BSH-FEM</td><td>19.53</td><td>15.23</td><td>9.52</td><td>10.88</td></tr><tr><td>Relative error</td><td>0.67%</td><td>0.46%</td><td>10.94%</td><td>4.65%</td></tr><tr><td>M-shaped BSH-EXP</td><td>39.89</td><td>32.70</td><td>22.14</td><td>10.86</td></tr><tr><td>M-shaped BSH-FEM</td><td>40.48</td><td>33.22</td><td>21.85</td><td>11.55</td></tr><tr><td>Relative error</td><td>1.46%</td><td>1.59%</td><td>1.31%</td><td>6.35%</td></tr></table>

commonly utilized energy absorbing materials and structures in the industries, such as thin-walled tubes, metallic foams, and honeycombs. It is obvious that the design range of BSH encompasses the spider web-inspired honeycombs, SHHs, and horseshoe inspired honeycombs. Notably, the upper SEA design boundary surpasses that of most metallic foams, thin-walled tubes, and honeycombs, underscoring the superior energy absorption capacity of BSH and its potential for diverse engineering applications. Moreover, the compression strength of BSHs is like that of metal and polymer foams, but inferior to that of Nomex honeycombs, carbon fiber honeycombs, and bi-directional hierarchical honeycombs of equivalent density, as illustrated in Fig. 17b. This discrepancy implies that the PCFs of BSHs would be comparatively lower than these honeycombs when sharing the same cross-sectional area, thereby encouraging enhanced impact protection capabilities.

Generally, the constitute material of the energy absorption structures can highly influence their energy absorption performance. For a fair assessment of the energy absorption capabilities of BSH compared to previous polyline/curve honeycombs, the same material, aluminum alloy AA1060-H112, can be employed across different structures, such as the THH, super hexagonal honeycomb (SHH), and wavy hexagonal honeycomb (WHH) with 3 or 5 waves. As depicted in Fig. 18, the SEAs of the THH, SHH, WHH-3, and WHH-5 all fall below the upper SEA design boundary of BSHs. Conversely, their PCFs closely approach the upper PCF design boundary of BSHs, thereby signifying the superior energy absorption capabilities of BSHs among the polyline/curve honeycombs. The WHH-3 and WHH-5 have the best energy absorption at low relative density, attributed to global buckling deformation beyond a relative density of  $3.0\%$ . Similarly, the deformation pattern of SHH shifts to full folding deformation below a relative density of  $4.5\%$ , leading to enhanced energy absorption performance. Although THH also undergoes full folding deformation, it features only 3 lobes along the height direction, resulting in a lower SEA compared to the upper SEA design boundary of BSH. This distinction underscores the superior energy absorption capabilities of BSH over THH, SHH, and WHH, positioning BSH as a promising candidate for high-performance energy absorption applications within the realm of polyline/curve honeycombs. Finally, it is possible to further enhance the energy absorption performance of BSHs by introducing hierarchical and gradient design strategies in the future work. Besides, the DNN-GA optimization design framework has the potential to be extended to other honeycombs through the application of transfer learning methodology. It is valuable to consider developing a universal artificial intelligence model to predict the mechanical properties of various honeycombs in future research endeavors.

![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/c3ad4c62f857363139f215356392e52a24b6c3e1280d28eff055f85e95b8b53c.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/6d9da8dab8038be6231e48951ad8d0bd849165a7d388816d161a11041f4572fb.jpg)



Fig. 17. Comparison of BSH with various structures and materials: (a) SEA-  $\sigma_{\mathrm{p}}$  [76,81]; (b) Strength-  $\rho$  [44,82].


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/7ac31890e549af8bf243a905e5efd708df631988099a6c72480f6970ab76e0b1.jpg)


![](file://D:/MinerU/转换结果/157.pdf-5bf46b7a-7dc4-4d1c-a4a7-4afd45e798b5/images/30933458d52ca15a0c4edbad5c5758845903398043f4444faf481b5a24ec2638.jpg)



Fig. 18. Comparison of BSH with the previous polyline/curve honeycombs, including THH, SHH, and WHH, under the same constituent material: (a) SEA; (b) PCF.


# 5. Conclusions

In this work, a novel BSH structure was designed to expand the design possibilities within the realm of polyline/curve hexagonal honeycombs, which can systematically reflect the energy absorption characteristics of traditional single-edge honeycombs. The energy absorption capabilities of the BSH were assessed through FEM and verified by the quasi-static compression tests. Four DNN models were trained to predict the relative density, PCF, MCF, and SEA of the BSH low average prediction errors, which are  $0.78\%$ ,  $2.2\%$ ,  $7.3\%$ , and  $6.6\%$ , respectively. Besides, combined with genetic algorithm, an efficient optimization design framework was introduced to delineate the upper SEA design boundary of the BSH. The upper SEA design boundary demonstrates a rise-peak-drop trend with escalating relative density. The maximum SEA recorded for the BSH via FE model is  $13.41~\mathrm{J / g}$ , correlating to a relative density of  $9.15\%$ . Furthermore, BSHs at the upper SEA design boundary are also at the upper PCF and MCF design boundary. Empirical equations to calculate the upper design boundary of the energy absorption criteria, including PCF, MCF, and SEA, were summarized from the amassed data. The maximum SEA of the BSH extrapolated by empirical equations amounts to  $13.13~\mathrm{J / g}$ , with a relative density of  $9.2\%$ . BSHs at the upper SEA design boundary have diverse configurations across varying relative densities, falling into six categories, including bowl-shaped BSH, 30-sided BSH, 5-shaped BSH, 2-shaped BSH, M-shaped BSH, and  $r$ -shaped BSH. In addition, under the same constitute material, the maximum SEA of the BSH is 1.53, 1.37, 1.97, and 2.70 times than that of the THH, SHH,

WHH-3, and WHH-5, respectively. The expansive scope for customizing energy absorption capabilities positions BSHs as promising candidates for aerospace and automotive applications.

# CRediT authorship contribution statement

Sicong Zhou: Writing - original draft, Visualization, Validation, Software, Methodology, Investigation, Formal analysis. Kang Zhang: Software, Methodology, Formal analysis. Liuchao Jin: Visualization, Validation, Software. Qiang Gao: Writing - review & editing, Methodology, Investigation. Wei-Hsin Liao: Writing - review & editing, Supervision, Investigation, Funding acquisition.

# Declaration of competing interest

The authors declare that they have no known competing financial interests or personal relationships that could have appeared to influence the work reported in this paper.

# Acknowledgements

This work was supported by the Research Grants Council (Project Nos.: CUHK14211823, C4074-22G), Hong Kong Special Administrative Region, China, and The Chinese University of Hong Kong (Project Nos.: 4055178, 3110174).

# Supplementary materials

Supplementary material associated with this article can be found, in the online version, at doi:10.1016/j.tws.2025.112941.

# Data availability

Data will be made available on request.

# References



[1] M Shifa, F Tariq, AD. Chandio, Mechanical and electrical properties of hybrid honeycomb sandwich structure for spacecraft structural applications, J. Sandw. Struct. & Mater. 23 (1) (2019) 222-240.





[2] OA Ganilova, MP Cartmell, A Kiley, Experimental investigation of the thermoelastic performance of an aerospace aluminium honeycomb composite panel, Compos. Struct. 257 (2021) 113159.





[3] VK Goyal, S. Maghsoudy-Louyeh, Proof test methodology for reducing the risk of unvented honeycomb core failures in aerospace structures, J. Sandw. Struct. & Mater. 25 (1) (2022) 61-76.





[4] W Hou, Y Shen, K Jiang, et al., Study on mechanical properties of carbon fiber honeycomb curved sandwich structure and its application in engine hood, Compos. Struct. 286 (2022) 115302.





[5] S Upadhyaya, A Korgal, BS Sridhar, et al., Synthesis and characterization of honeycomb sandwiched composite material for automobile applications, Mater. Today: Proc. 54 (2022) 502-506.





[6] M Amraei, M Shahravi, Z Noori, et al., Application of aluminium honeycomb sandwich panel as an energy absorber of high-speed train nose, J. Compos. Mater. 48 (9) (2013) 1027-1037.





[7] Y Garbatov, S Scattareggia Marchese, G Epasto, et al., Flexural response of additive-manufactured honeycomb sandwiches for marine structural applications, Ocean Eng. 302 (2024) 117732.





[8] Y He, Z Bi, T Wang, et al., Design and mechanical properties analysis of hexagonal perforated honeycomb metamaterial, Int. J. Mech. Sci. 270 (2024) 109091.





[9] Y Deng, X Guo, Y Lin, et al., Dual-Phase Inspired Soft Electronic Sensors with Programmable and Tunable Mechanical Properties, ACS. Nano 17 (7) (2023) 6423-6434.





[10] Y Guo, J. Zhang, Shock absorbing characteristics and vibration transmissibility of honeycomb paperboard, Shock Vib. 11 (5-6) (2004) 521-531.





[11] W Shuai, E Li, H Wang, et al., Space mapping-assisted optimization of a thin-walled honeycomb structure for battery packaging, Struct. Multidisc. Optim. 62 (2) (2020) 937-955.





[12] X-L Peng, S. Bargmann, A novel hybrid-honeycomb structure: Enhanced stiffness, tunable auxicity and negative thermal expansion, Int. J. Mech. Sci. 190 (2021) 106021,





[13] K-J Liu, H-T Liu, J. Li, Thermal expansion and bandgap properties of bi-material triangle re-entrant honeycomb with adjustable Poisson's ratio, Int. J. Mech. Sci. 242 (2023) 108015.





[14] A Zhakatayev, Z Kappassov, HA. Varol, Analytical modeling and design of negative stiffness honeycombs, Smart Mater. Struct. 29 (4) (2020) 045024.





[15] S Chen, X Tan, J Hu, et al., A novel gradient negative stiffness honeycomb for recoverable energy absorption, Compos. B Eng. 215 (2021) 108745.





[16] N Mehreganian, AS Fallah, P. Sareh, Structural mechanics of negative stiffness honeycomb metamaterials, J. Appl. Mech. 88 (5) (2021) 051006.





[17] Q Gao, W-H Liao, L. Wang, On the low-velocity impact responses of auxetic double arrowed honeycomb, Aerosp. Sci. Technol. 98 (2020) 105698.





[18] H Lu, X Wang, T. Chen, In-plane dynamics crushing of a combined auxetic honeycomb with negative Poisson's ratio and enhanced energy absorption, Thin-Walled Struct 160 (2021) 107366.





[19] Q Gao, Z Ding, W-H. Liao, Effective elastic properties of irregular auxetic structures, Compos. Struct. 287 (2022) 115269.





[20] B Xiao, Y Liu, W Xu, et al., A bistable honeycomb mechanical metamaterial with transformable Poisson's ratio and tunable vibration isolation properties, Thin-Walled Struct 198 (2024) 111718.





[21] JH Xiao, ZX. Guo, Failure analysis of thickness gradient negative poisson's ratio concave honeycomb sandwich panels under local impact, Mech. Compos. Mater. 60 (2) (2024) 401-414.





[22] Y Gao, X Chen, Y. Wei, Graded honeycombs with high impact resistance through machine learning-based optimization, Thin-Walled Struct 188 (2023) 110794.





[23] X Niu, F Xu, Z Zou, et al., Impact resistance of horsetail bio-honeycombs, Int. J. Mech. Sci. 266 (2024) 108988.





[24] Y Hu, Y Li, Y Zhang, et al., Design methodology for functional gradient star-shaped honeycomb with enhanced impact resistance and energy absorption, Mater. Today Commun. 38 (2024) 108020.





[25] S Koch, F Duvigneau, R Orszulik, et al., Partial filling of a honeycomb structure by granular materials for vibration and noise reduction, J. Sound. Vib. 393 (2017) 30-40.





[26] P Sheng, X Fang, L Dai, et al., Synthetical vibration reduction of the nonlinear acoustic metamaterial honeycomb sandwich plate, Mech. Syst. Signal. Process. 185 (2023) 109774.





[27] E Rao, T. Fu, Acoustic radiation response of functionally graded sandwich plates cored by butterfly-shaped honeycombs with negative Poisson's ratio, J. Mech. Sci. Technol. 38 (5) (2024) 2321-2333.





[28] AV Ryzhenkov, EE Lapin, NA Loginova, et al., Evaluation of the thermal efficiency of a high-temperature heat-insulation structure based on honeycomb plastic, Therm. Eng. 63 (6) (2016) 445-448.





[29] C Zhang, S Song, Q Cao, et al., Improving the comprehensive properties of chitosan-based thermal insulation aerogels by introducing a biobased epoxy thermoset to form an anisotropic honeycomb-layered structure, Int. J. Biol. Macromol. 246 (2023) 125616.





[30] Z Xu, J Wang, L Pan, et al., Experimental, numerical and theoretical study on heat transfer in paper honeycomb structure, Int. J. Therm. Sci. 186 (2023) 108108.





[31] MK Khan, T Baig, S. Mirza, Experimental investigation of in-plane and out-of-plane crushing of aluminum honeycomb, Mater. Sci. Eng. A 539 (2012) 135-142.





[32] S Xie, Z Feng, H Zhou, et al., In-plane and out-of-plane compressive mechanical properties of Nomex honeycombs and their prediction, J. Braz. Soc. Mech. Sci. Eng. 42 (9) (2020) 460.





[33] NS Ha, G Lu, X. Xiang, Energy absorption of a bio-inspired honeycomb sandwich panel, J. Mater. Sci. 54 (8) (2019) 6286-6300.





[34] Y Chen, F Qian, L Zuo, et al., Broadband and multiband vibration mitigation in lattice metamaterials with sinusoidally-shaped ligaments, Extreme Mech. Lett. 17 (2017) 24-32.





[35] X Yang, Y Sun, J Yang, et al., Out-of-plane crashworthiness analysis of bio-inspired aluminum honeycomb patterned with horseshoe mesostructure, Thin-Walled Struct. 125 (2018) 1-11.





[36] G Feng, S Li, L Xiao, et al., Energy absorption performance of honeycombs with curved cell walls under quasi-static compression, Int. J. Mech. Sci. 210 (2021) 106746.





[37] K Zied, M Osman, T. Elmahdy, Enhancement of the in-plane stiffness of the hexagonal re-entrant auxetic honeycomb cores, Phys. Status Solidi (b) 252 (12) (2015) 2685–2692.





[38] S Li, Z Liu, VPW Shim, et al., In-plane compression of 3D-printed self-similar hierarchical honeycombs - Static and dynamic analysis, Thin-Walled Struct. 157 (2020) 106990.





[39] Y Zhang, S Cao, G. Liu, 3D printed bending-stretching coupled non-self-similar hierarchical cellular topology under in-plane loading, Compos. Struct. 323 (2023) 117442.





[40] Y Zhang, M Lu, CH Wang, et al., Out-of-plane crashworthiness of bio-inspired self-similar regular hierarchical honeycombs, Compos. Struct. 144 (2016) 1-13.





[41] D Zhang, Q Fei, J Liu, et al., Crushing of vertex-based hierarchical honeycombs with triangular substructures, Thin-Walled Struct. 146 (2020) 106436.





[42] X-C Zhang, N-N Liu, C-C An, et al., Dynamic crushing behaviors and enhanced energy absorption of bio-inspired hierarchical honeycombs with different topologies, Def. Technol. 22 (2023) 99-111.





[43] C Guo, X Cheng, L Lu, et al., Energy absorption of central self-similar honeycombs under quasi-static axial load, Int. J. Mech. Sci. 274 (2024) 109264.





[44] W Huang, Y Zhang, Y Xu, et al., Out-of-plane mechanical design of bi-directional hierarchical honeycombs, Compos. B Eng. 221 (2021) 109012.





[45] K Song, D Li, C Zhang, et al., Bio-inspired hierarchical honeycomb metastructures with superior mechanical properties, Compos. Struct. 304 (2023) 116452.





[46] HH Tsang, KM Tse, KY Chan, et al., Energy absorption of muscle-inspired hierarchical structure: Experimental investigation, Compos. Struct. 226 (2019) 111250.





[47] W Huang, Y Zhang, J Zhou, et al., Stabilized and efficient multi-crushing properties via face-centered hierarchical honeycomb, Int. J. Mech. Sci. 266 (2024) 108918.





[48] Q He, J Feng, Y Chen, et al., Mechanical properties of spider-web hierarchical honeycombs subjected to out-of-plane impact loading, J. Sandw. Struct. Mater. 22 (3) (2018) 771-796.





[49] H Liang, Q Wang, Y Pu, et al., In-plane compressive behavior of a novel self-similar hierarchical honeycomb with design-oriented crashworthiness, Int. J. Mech. Sci. 209 (2021) 106723.





[50] Y Nian, S Wan, X Li, et al., How does bio-inspired graded honeycomb filler affect energy absorption characteristics? Thin-Walled Struct. 144 (2019) 106269.





[51] H Wu, X Zhang, Y. Liu, In-plane crushing behavior of density graded cross-circular honeycombs with zero Poisson's ratio, Thin-Walled Struct. 151 (2020) 106767.





[52] Z Liu, J Liu, J Liu, et al., The impact responses and failure mechanism of composite gradient reentrant honeycomb structure, Thin-Walled Struct. 182 (2023) 110228.





[53] L. Boldrin, S. Hummel, F. Scarpa, et al., Dynamic behaviour of auxetic gradient composite hexagonal honeycombs, Compos. Struct. 149 (2016) 114-124.





[54] B Yu, B Han, P-B Su, et al., Graded square honeycomb as sandwich core for enhanced mechanical performance, Mater. Des. 89 (2016) 642-652.





[55] HH Xu, HC Luo, XG Zhang, et al., Mechanical properties of aluminum foam filled re-entrant honeycomb with uniform and gradient designs, Int. J. Mech. Sci. 244 (2023) 108075.





[56] M Hosseini, H. Mazaheri, Mechanical behavior of graded combined auxetic-honeycomb structures, Int. J. Mech. Sci. 276 (2024) 109223.





[57] J Huang, Q Zhang, F Scarpa, et al., Shape memory polymer-based hybrid honeycomb structures with zero Poisson's ratio and variable stiffness, Compos. Struct. 179 (2017) 437-443.





[58] A Ingrole, A Hao, R. Liang, Design and modeling of auxetic and hybrid honeycomb structures for in-plane property enhancement, Mater. Des. 117 (2017) 72-83.





[59] A Montazeri, A Hasani, M. Safarabadi, Bending performance and failure mechanism of 3D-printed hybrid geometry honeycombs with various poisson's ratios, J. Sandw. Struct. Mater. 25 (7) (2023) 709-729.





[60] M Xu, D Liu, P Wang, et al., In-plane compression behavior of hybrid honeycomb metastructures: Theoretical and experimental studies, Aerosp. Sci. Technol. 106 (2020) 106081.





[61] F Ghorbani, H Gharehbaghi, A Farrokhabadi, et al., Evaluation of the mechanical properties and energy absorption in a novel hybrid cellular structure, Aeroesp. Sci. Technol. 148 (2024) 109105.





[62] K Yang, L Rao, L Hu, et al., 3D curved-walled same-phase chiral honeycombs with controllable compression-torsion coupling effect via variable cross-section design, Thin-Walled Struct. 193 (2023) 111267.





[63] K Yang, Z Li, D. Ge, Quasi-static and dynamic out-of-plane crashworthiness of 3D curved-walled mixed-phase honeycombs, Thin-Walled Struct. 182 (2023) 110305.





[64] M Xu, Z Zhao, P Wang, et al., Mechanical performance of bio-inspired hierarchical honeycomb metamaterials, Int. J. Solids. Struct. 254-255 (2022) 111866.





[65] G Wang, Z Cai, X. Deng, In-plane dynamic impact mechanical properties of novel bi-directional hierarchical honeycomb, Eng. Fract. Mech. 300 (2024) 110009.





[66] J Yang, D Yang, Y Tao, et al., Machine learning assisted prediction and analysis of in-plane elastic modulus of hybrid hierarchical square honeycombs, Thin-Walled Struct. 198 (2024) 111736.





[67] Y Wang, Z Liao, S Shi, et al., Data-driven structural design optimization for petal-shaped auxetics using isogeometric analysis, Comput. Model. Eng. Sci. 122 (2) (2020) 433-458.





[68] H Wang, S-H Xiao, C. Zhang, Novel planar auxetic metamaterial perforated with orthogonally aligned oval-shaped holes and machine learning solutions, Adv. Eng. Mater. 23 (7) (2021) 2100102.





[69] Z Liao, Y Wang, L Gao, et al., Deep-learning-based isogeometric inverse design for tetra-chiral auxetics, Compos. Struct. 280 (2022) 114808.





[70] M Mohammadnejad, A Montazeri, E Bahmanpour, et al., Artificial neural networks for inverse design of a semi-auxetic metamaterial, Thin-Walled Struct. 200 (2024) 111927.





[71] MW Cho, K Ko, M Mohammadhosseinzadeh, et al., Inverse design of Bezier curve-based mechanical metamaterials with programmable negative thermal expansion and negative Poisson's ratio via a data augmented deep autoencoder, Mater. Horiz. (2024).





[72] X Shen, K Yan, D Zhu, et al., Inverse machine learning framework for optimizing gradient honeycomb structure under impact loading, Eng. Struct. 309 (2024) 118079.





[73] X Shen, Q Hu, D Zhu, et al., Dynamic mechanical response prediction model of honeycomb structure based on machine learning method and finite element method, Int. J. Impact. Eng. 184 (2024) 104825.





[74] C Yang, K Meng, L Yang, et al., Transfer learning-based crashworthiness prediction for the composite structure of a subway vehicle, Int. J. Mech. Sci. 248 (2023) 108244.





[75] Z Huang, X Zhang, H. Zhang, Energy absorption and optimization design of multicell tubes subjected to lateral indentation, Thin-Walled Struct. 131 (2018) 179-191.





[76] Y Yang, H Liu, Q Zhang, et al., Energy absorption characteristics of a super hexagonal honeycomb under out-of-plane crushing, Thin-Walled Struct. 189 (2023) 110914.





[77] SP Santosa, T Wierzbicki, AG Hanssen, et al., Experimental and numerical studies of foam-filled sections, Int. J. Impact. Eng. 24 (5) (2000) 509-534.





[78] Y Xu, L Xia, A Abd El-Aty, et al., Revealing the dynamic behavior and micromechanisms of enhancing the formability of AA1060 sheets under high strain rate deformation, J. Mater. Res. Technol. 28 (2024) 2402-2409.





[79] J Xiang, J. Du, Energy absorption characteristics of bio-inspired honeycomb structure under axial impact loading, Mater. Sci. Eng. A 696 (2017) 283-289.





[80] X Zhang, H. Zhang, Theoretical and numerical investigation on the crush resistance of rhombic and kagome honeycombs, Compos. Struct. 96 (2013) 143-152.





[81] NS Ha, G. Lu, A review of recent research on bio-inspired structures and materials for energy absorption applications, Compos. B Eng. 181 (2020) 107496.





[82] Y Zhang, T Liu, W. Tizani, Experimental and numerical analysis of dynamic compressive response of Nomex honeycombs, Compos. B Eng. 148 (2018) 27-39.

