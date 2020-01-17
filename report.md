DEPARTMENT ELECTRICAL ENGINEERING
INDIAN INSTITUTE OF TECHNOLOGY ROORKEE
ROORKEE - 247667 (INDIA)
January-2020
 
Abstract
With the rising needs of more power consumption, to meet increase in requirement for power quality and reliability more and more distributed energy systems are added into the electrical infrastructure. Microgrid – a prospective framework, which addresses the technical concerns accompanying growing deployment of renewable sources. The inherent modern controls enable Microgrid to operate with a degree of autonomy than traditional grid. Operation of Microgrid is bifurcated into grid connected operation during normal conditions and autonomous or standalone operation in emergencies. Microgrid consists of large no of distributed energy resources (DER) and energy storage systems (ESS) and controllable loads and their interconnections. Power balance among generation and load, energy sharing in between the distributed generators and coordinated operation requires complex and stringent control schemes. Overall control is classified as local or coordinated control. Local control is based on local measurements while in coordinated control some sort of communication among the entities are present. Depending on the communication schemes, the control strategies are characterized as decentralized, centralized and distributed control. In centralized and the distributed network, the communication is based on digital communication technologies digital communication links (DCL). Centered on control functionality on each level of hierarchical control schemes are categorized intro primary control, secondary control and tertiary control. The principal roles of the Microgrid control structure are voltage and frequency regulation for both operating Modes; proper load sharing and DER coordination; Microgrid resynchronization with the main grid; power flow control between the Microgrid and the main grid; optimizing the Microgrid operating cost.
 
Contents
Chapter 1: Introduction	7
1.1 Background	7
1.2 Historical Perspective	7
1.3 Literature Survey	7
1.4 Concept of Microgrid	7
1.5 Technical and economic advantages of Microgrid	8
1.6 Challenges and disadvantages of Microgrid development	9
1.7 Management and operational issues of a Microgrid	9
1.8 Dynamic interactions of Microgrid with main grid	9
Chapter 2: Microgrid Types and Architecture	10
Chapter 3: Microgrid Control and Modelling	11
3.1 Control of AC Microgrids	11
3.1.1 Control Objectives in AC Microgrids	11
3.1.2 Primary Control Techniques in AC Microgrids	12
3.1.3 Secondary Control	14
3.1.4 Tertiary Control	16
3.2 Dynamic Modeling of AC Microgrids	17
3.2.1 Voltage-Controlled Voltage Source Inverters	17
3.2.2 Current-Controlled Voltage Source Inverters	17
3.3 Control of DC Microgrids	18
3.3.1 Control Objectives	18
3.3.2 Standard Control Technique	18
Chapter 4: Distributed Control of AC Microgrids	19
4.1 Distributed Secondary Frequency Control	19
4.2 Distributed Secondary Frequency and Power Control	19
4.2.1 Distributed Cooperative Control Protocol for Frequency and Active Power Sharing	19
4.2.2 Case Studies	19
4.3 Distributed Secondary Voltage Control of AC Microgrids	19
4.3.1 Secondary Voltage Control Objectives	19
4.3.2 Distributed Secondary Voltage Control Using Feedback Linearization	19
4.3.3 Case Studies	19
4.4 Distributed Secondary Voltage and Reactive Power Control of AC Microgrids	19
Chapter 5: Cooperative Control for DC Microgrids	20
7.1 Distributed Cooperative Controller for DC Microgrids	20
7.1.1 Graphical Representation of DC Microgrids	20
7.1.2 Cooperative Secondary Control Framework	20
7.1.3 Voltage Observer	20
7.2 Analytical Model Development for DC Microgrids	20
7.2.1 Global Dynamic Model	20
7.2.2 Guidelines for Controller Design	20
7.2.3 Steady-State Analysis	20
7.3 Distributed Adaptive Droop Control for DC Microgrids An Alternative Solution	20
7.4 Experimental Performance Evaluation	20
7.4.1 Design Procedure	20
7.4.2 Droop Controller Versus Cooperative Controller	20
7.4.3 Load Change Performance Assessment	20
7.4.4 Plug-and-Play Capability	20
7.4.5 Cyber-Link Failure Resiliency.	20
Chapter 6: Conclusion	21
Chapter 7: References	22

 
List of Abbreviations
ABBREVIATION
DESCRIPTION
BESS	Battery energy storage System
CC	Central controller
CCVSI	Current controlled voltage source converter
DBS	DC bus signaling.
DCC	Distributed Cooperative Control
DCL	Digital communication link
DG	Distributed generator.
DPS	Distributed power system.
INC	Incremental Conductance
MG	Microgrid
MGCC	Microgrid Central Controller
MPPT	Maximum Power Point Tracking
PCC	Point of Common Coupling
PLL	Phase Locked Loop
PLS	Power Line Signaling
THD	Total Harmonic Distortion
VCVSI	Current controlled voltage source converter
VSC	Voltage Source Converter


 
List of Figures
Figure 3.0 1: Hierarchical Control of Microgrid Control System [2016 © IEEE]	12
Figure 3.0 2: PQ Control Mode with active and reactive power references [2016 © IEEE]	13
Figure 3.0 3: Reference voltage determination for voltage control mode [2016 © IEEE] [5]	14
Figure 3.0 4: Voltage and current control loops in voltage control mode. [2016 © IEEE] [5]	14
Figure 3.0 5: Conventional Droop Method	14
Figure 3.0 6 : Simplified Diagram of a converter connected to a Microgrid	15
Figure 3.7: Small-signal model of the conventional active power control	16
Figure 3.0 8: Output frequency of inverter with inductive coupling and traditional droop control	17
Figure 3.0 9: Output frequency of inverter with inductive coupling and fictitious impedance control	17
Figure 3.0 10: Block diagram of secondary and tertiary control	18
Figure 3.0 11: Block diagram of Voltage controlled voltage source converters based DG	19
Figure 3.0 12: Block diagram of Current controlled voltage source converter based DG	20
Figure 4.0 1: Multi-agent environment for a microgrid system with DGs as agents	22
 
Chapter 1: Introduction

1.1 Background
1.2 Historical Perspective
1.3 Literature Survey
1.4 Concept of Microgrid
Microgrids are small-scale, LV CHP supply networks designed to supply electrical and heat loads for a small community, such as a housing estate or a suburban locality, or an academic or public community such as a university or school, a commercial area, an industrial site, a trading estate or a municipal region. Microgrid is essentially an active distribution network because it is the conglomerate of DG systems and different loads at distribution voltage level. The generators or micro-sources employed in a Microgrid are usually renewable/non-conventional DERs integrated together to generate power at distribution voltage. From operational point of view, the micro-sources must be equipped with power electronic interfaces and controls to provide the required flexibility to ensure operation as a single aggregated system and to maintain the specified power quality and energy output. This control flexibility would allow the Microgrid to present itself to the main utility power system as a single controlled unit that meets local energy needs for reliability and security. The key differences between a Microgrid and a conventional power plant are as follows:
(1) Micro-sources are of much smaller capacity with respect to the large generators in conventional power plants.
(2) Power generated at distribution voltage can be directly fed to the utility distribution network.
(3) Micro-sources are normally installed close to the customers’ premises so that the electrical/heat loads can be efficiently supplied with satisfactory voltage and frequency profile and negligible line losses.
The technical features of a Microgrid make it suitable for supplying power to remote areas of a country where supply from the national grid system is either difficult to avail due to the topology or frequently disrupted due to severe climatic conditions or man-made disturbances.
From grid point of view, the main advantage of a Microgrid is that it is treated as a controlled entity within the power system. It can be operated as a single aggregated load. This ascertains its easy controllability and compliance with grid rules and regulations without hampering the reliability and security of the power utility. From customers’ point of view, Microgrids are beneficial for locally meeting their electrical/heat requirements. They can supply uninterruptible power, improve local reliability, reduce feeder losses and provide local voltage support. From environmental point of view, Microgrids reduce environmental pollution and global warming through utilization of low-carbon technology. However, to achieve a stable and secure operation, a number of technical, regulatory and economic issues have to be resolved before Microgrids can become commonplace. Some problem areas that would require due attention are the intermittent and climate-dependent nature of generation of the DERs, low energy content of the fuels and lack of standards and regulations for operating the Microgrids in synchronism with the power utility. The study of such issues would require extensive real-time and off line research, which can be taken up by the leading engineering and research institutes across the globe.
1.5 Technical and economic advantages of Microgrid
The development of Microgrid is very promising for the electric energy industry because of the following advantages:
	Environmental issues – It is needless to say that Microgrids would have much lesser environmental impact than the large conventional thermal power stations. However, it must be mentioned that the successful implementation of carbon capture and storage (CCS) schemes for thermal power plants will drastically reduce the environmental impacts. Nevertheless, some of the benefits of Microgrid in this regard are as follows: 
	Reduction in gaseous and particulate emissions due to close control of the combustion process may ultimately help combat global warming.
	Physical proximity of customers with microsources may help to increase the awareness of customers towards judicious energy usage.
	Operation and investment issues – Reduction of physical and electrical distance between microsource and loads can contribute to:
	Improvement of reactive support of the whole system, thus enhancing the voltage profile.
	Reduction of T&D feeder congestion.
	Reduction of T&D losses to about 3%.
	Reduction/postponement of investments in the expansion of transmission and generation systems by proper asset management.
	Power quality – Improvement in power quality and reliability is achieved due to:
	Decentralization of supply.
	Better match of supply and demand.
	Reduction of the impact of large-scale transmission and generation outages.
	Minimization of downtimes and enhancement of the restoration process through black start operations of microsources.
	Cost saving – The following cost savings are achieved in Microgrid:
	A significant saving comes from utilization of waste heat in CHP mode of operation. Moreover, as the CHP sources are located close to the customer loads, no substantial infrastructure is required for heat transmission. This gives a total energy efficiency of more than 80% as compared to a maximum of 40% for a conventional power system.
	Cost saving is also effected through integration of several microsources. As they are locally placed in plug-and-play mode, the T&D costs are drastically reduced or eliminated. When combined into a Microgrid, the generated electricity can be shared locally among the customers, which again reduces the need to import/export power to/from the main grid over longer feeders.
	Market issues – The following advantages are attained in case of market participation:
	The development of market-driven operation procedures of the Microgrids will lead to a significant reduction of market power exerted by the established generation companies.
	The Microgrids may be used to provide ancillary services.
	Widespread application of modular plug-and-play microsources may contribute to a reduction in energy price in the power market.
	The appropriate economic balance between network investment and DG utilization is likely to reduce the long-term electricity customer prices by about 10%.
1.6 Challenges and disadvantages of Microgrid development
1.7 Management and operational issues of a Microgrid
1.8 Dynamic interactions of Microgrid with main grid 
The capacity of Microgrid being sufficiently small, the stability of main grid is not affected when it is connected to the main grid. However, in future, when Microgrids will become more commonplace with higher penetration of DERs, the stability and security of the main grid will be influenced significantly. In such case the dynamic interactions between Microgrid and the main grid will be a key issue in the operation and management of both the grids. However, as of now, since the DERs in Microgrids are mainly meant to ensure only local energy balance within a small load pocket, the effects of DER penetration are likely to have a low impact on the main grid. Nevertheless, Microgrids need to be designed properly to take care of their dynamic impacts on main grid such that overall stability and reliability of the whole system is significantly improved.


 
Chapter 2: Microgrid Types and Architecture
 
Chapter 3: Microgrid Control and Modelling

In this chapter, there are separate discussions on the control objectives in AC and DC Microgrids. Conventional and existing AC and DC Microgrid control schemes are vigorously studied in this chapter. Depending on the desired control objectives, suitable mathematical models for Distributed Generators are derived and represented in this literature. These mathematical models fuels the inspiration to the designing of various advanced control algorithms.

3.1 Control of AC Microgrids 
In this section, first the control objectives in AC Microgrids are explained. Then, based on these control objectives, the hierarchical control structure of AC Microgrids is discussed. The hierarchical control structure contains three main levels, namely primary, secondary, and tertiary control levels. Finally, the dynamical model of distributed generators is derived. These dynamical models will be used in subsequent chapters to design distributed control protocols for Microgrids.

3.1.1 Control Objectives in AC Microgrids 
Operation of Microgrid is categorized in two different modes: grid-connected mode and autonomous mode. The proper control of Microgrid is a prerequisite for stable and economically efficient operation. The principal roles of the Microgrid control structure are as follows:
	Voltage and frequency regulation for both operating modes
	Proper load sharing and DG coordination
	Microgrid resynchronization with the main grid
	Power flow control between the Microgrid and the main grid
	Optimizing the Microgrid operating cost 
	Proper handling of transients and restoration of desired conditions when switching between modes.
The significance and timescales of these requirements are different, thus there is a requirement of a hierarchical control structure to address each requirement at a different control hierarchy level. The microgrid hierarchical control strategy consists of three levels, namely primary, secondary, and tertiary controls. The primary control operates at the fastest timescale and maintains voltage and frequency stability of the microgrid subsequent to the islanding process when switching from grid-connected mode. It is essential to provide independent active and reactive power sharing controls for the DGs in the presence of both linear and nonlinear loads. Moreover, the power sharing control avoids undesired circulating currents. The primary control level includes fundamental control hardware, commonly referred to as zero level, which comprises internal voltage and current control loops of the DGs. The secondary control compensates for the voltage and frequency deviations caused by the operation of the primary controls and restores frequency and voltage synchronization. At the highest level and slowest timescale, the tertiary control manages the power flow between the microgrid and the main grid and facilitates an economically optimal operation.

3.1.2 Primary Control Techniques in AC Microgrids
The primary control is designed to satisfy the following requirements:
	To stabilize the voltage and frequency: Subsequent to an islanding event, the microgrid may lose its voltage and frequency stability due to the mismatch between the power generated and consumed, which was otherwise provided by the grid.
	To offer plug-and-play capability for DGs and properly share the active and reactive powers among them, preferably, without any communication links.
	To mitigate circulating currents that can cause overcurrent phenomenon in the power electronic devices and damage the DC-link capacitor.
The control structure of a VSI may vary based on its objectives. Before going into the details of primary control, one has clear understanding of converters objectives. Voltage-controlled voltage source inverters (VCVSI) facilitate the voltage and frequency control of DGs. Current-controlled voltage source inverters (CCVSI) control the direct and quadrature components of the VSI output current, which, in turn, regulates the active and reactive power delivery.[1]
The primary control provides the reference points for the real-time voltage and current control loops of DGs. These inner control loops are commonly referred to as zero-level control. The zero-level control is generally implemented in either active/reactive power (PQ) mode or voltage control mode [2]. In the PQ control mode, the DG active and reactive power delivery is regulated on the predetermined reference points, as shown in Fig. 3.2. The control strategy is implemented with a current-controlled voltage source inverter (CCVSI). In Fig. 3.2, H1 controller regulates the DC-link voltage and the active power through by adjusting the magnitude of the output active current of the converter, ip. H2 controller regulates the output reactive power by adjusting the magnitude of the output reactive current, i.e., iq [3].

In the voltage control mode, the DG operates as a voltage-controlled voltage source inverter (VCVSI) where the reference voltage, vo*, is determined by the primary control, conventionally via droop characteristics [3], as shown in Fig. 3.3. The nested voltage and current control loops in the voltage control mode are shown in Fig. 3.4. This controller feeds the current signal as a feedforward term via a transfer function (e.g., virtual impedance)

















Droop Control: The droop control method is referred as independent, autonomous, and wireless control due to the elimination of communication links between the converters. The conventional active power control (frequency droop characteristic) and reactive power control (voltage droop characteristic), those illustrated in Figure 3 5, are used for voltage mode control. Principles of the conventional droop methods can be explained by considering an equivalent circuit of a VCVSI connected to an AC bus, as shown in Figure 3 6. If switching ripples and high-frequency harmonics are neglected, the VCVSI can be modeled as an AC source, with the voltage of E∠δ. In addition, assume that the common AC bus voltage is Vcom∠0 and the converter output impedance and the line impedance are lumped as a single effective line impedance of Z∠θ.
The complex power delivered to the common AC bus is calculated as
S=V_com I^*=(V_com E∠θ-δ)/Z-(〖V_com〗^2∠θ)/Z 					(3.1)
from which the real and reactive powers are achieved as
{█(P= (V_com E)/Z  cos⁡〖(θ-δ)〗-〖V_com〗^2/Z  cos⁡〖(θ)〗@Q= (V_com E)/Z  sin⁡〖(θ-δ)〗-〖V_com〗^2/Z sin(θ))┤   					(3.2)
If the effective line impedance, Z∠θ, is assumed to be purely inductive, θ = 90o,
then (3.2) can be reduced to
{█(P= (V_com E)/Z  sin⁡〖(δ)〗@Q= (V_com E cos⁡〖(δ)〗-〖V_com〗^2)/Z)┤							(3.3)
If the phase difference between the converter output voltage and the common
AC bus, d, is small enough, then sin δ = δ and cos δ = 1. Thus, one can apply the
frequency and voltage droop characteristics to fine-tune the voltage reference of the
VCVSI as shown in Fig. 3.6 based on
{█(ω=ω^*- D_P P@E=E^*-D_Q Q)┤								(3.4)
where the primary control references E* and ω* are the DG output voltage RMS value and angular frequency at the no-load condition, respectively. The droop coefficients, DP and DQ, can be adjusted either heuristically or by tuning algorithms. In the former approach, DP and DQ are determined based on the converter power rating and the maximum allowable voltage and frequency deviations. For instance, in a microgrid with N DGs, corresponding DP and DQ should satisfy the following constraints

{█(Δω_max= D_P1 P_n1=D_P2 P_n2=D_P3 P_n3=⋯=D_PN P_nN@ ΔE_max= D_Q1 Q_n1=D_Q2 Q_n2=D_Q3 Q_n3=⋯=D_QN Q_nN )┤		 (3.5)
where Δω_max and ΔE_max are the maximum allowable angular frequency and voltage
deviations, respectively. P_ni and Q_ni are the nominal active and reactive powers of
the ith DG.
During the grid-tied operation of microgrid, the DG voltage and angular frequency,
E and ω, are enforced by the grid. The DG output active and reactive power references, Pref and Qref, can hence be adjusted through E* and ω* as
{█(P_ref=(ω^*-ω )/D_P @Q_ref=(E^*-E)/D_Q )┤ 								(3.6)
Dynamic response of the conventional primary control, on the simplified system
of Fig. 3.6, can be studied by linearizing (3.3) and (3.4). For instance, the linearized
active power equation in (3.3) and frequency droop characteristic in (3.4) are
{█(ΔP=GΔδ@Δω=〖Δω〗^*-D_P ΔP)┤							(3.7)
Where at the operating point of Vcom0, E0, and δ0
G=(V_com0 E_0)/Z  cos⁡〖(δ_0)〗 							(3.8)
And  Δδ=∫▒Δω dt						 		(3.9)
Therefore, the small-signal model for the active power control in (3.4) is
ΔP(s)=G/(〖s+D〗_P G) 〖Δω〗^* (s)							(3.10)

Few Potential disadvantages of conventional droop control is mentioned below. Control is affected by the system parameters, only functional for highly inductive transmission lines. It cannot handle nonlinear loads. Voltage regulation is not guaranteed. Adjusting the controller speed for the active and reactive power controllers can affect the voltage and frequency controls.


3.1.3 Secondary Control
Primary control may cause frequency and voltage deviations after the local control commands even in steady state as shown in fig 3.5 [4] and 3.6 [4]. Although the energy storage devices can compensate for this deviation, they are unable to provide the power for load frequency control over the long term due to their short energy capacity. Primary control is implemented locally at each DG. The secondary control, as a centralized controller, restores the microgrid voltage and frequency and compensates for the deviations caused by the primary control. This level of the control hierarchy is designed to have slower dynamic response than that of the primary. Figure 3.7 represents the block diagram of the conventional secondary control with a centralized control structure. As shown in this figure, frequency of the microgrid and the terminal voltage of a given DG are compared with the corresponding reference values, ωref and vref , respectively. Then, individual controllers process the error signals as in (equation 3.1, 3.2); the resulting signals (∂ω and ∂E) are sent to the primary controller of the DG to compensate for the frequency and voltage deviations.

∂ω=K_(P_ω ) (ω_ref-ω)+K_(I_ω ) ∫▒(ω_ref-ω)dt+∆ω_s 				(3.5)
∂E=K_(P_E ) (v_ref-E)+K_(I_E ) ∫▒(v_ref-E)dt 						(3.6)


 


3.1.4 Tertiary Control
Tertiary control is the last control level hierarchical control and operates on the slowest timescale. It considers the economic concerns for optimal operation of the microgrid and manages the power flow between microgrid and main grid. In the grid-tied mode, the power flow between microgrid and main grid can be managed by adjusting the amplitude and frequency of DG as shown in Fig. 3.10.

3.2 Dynamic Modeling of AC Microgrids
The microgrid control schemes employ the dynamic nonlinear model of DGs. In this section, the dynamical model of VCVSIs and CCVSIs is explained.

3.2.1 Voltage-Controlled Voltage Source Inverters 
The block diagram of a voltage-controlled voltage source inverter (VCVSI)-based DG is shown in Fig. 3.8. It contains an inverter bridge, connected to a primary DC power source (e.g., photovoltaic panels or fuel cells). The control loops, including the power, voltage, and current controllers, adjust the output voltage and frequency of the inverter bridge. Given the relatively high switching frequency of the inverter bridge, the switching artifacts can be safely neglected via average-value modeling.
















It should be noted that the nonlinear dynamics of each DG are formulated in its own d-q (direct–quadrature) reference frame. It is assumed that the reference frame of the ith DG is rotating at the frequency of ωi. The reference frame of one DG is considered as the common reference frame with the rotating frequency of ωcom. The angle of the ith DG reference frame, with respect to the common reference frame, is denoted as δi and satisfies the following differential equation.

	(δ_i ) ̇=ω_i-ω_com  					 (3.7)
The power controller block, shown in Fig. 3.12, contains the droop technique in (3.4) and provides the voltage references vodi* and voqi* for the voltage controller, as well as the operating frequency ωi for the inverter bridge. Two low-pass filters with the cutoff frequency of ωci are used to extract the fundamental component of the output active and reactive powers, denoted as Pi and Qi, respectively. The differential equations of the power controller can be written as


{█((P_i ) ̇= 〖-ω_ci P〗_i+ω_ci (v_odi i_odi+v_oqi i_oqi)@(Q_i ) ̇= 〖-ω_ci Q〗_i+ω_ci (v_oqi i_odi-v_odi i_oqi))┤					(3.8)
where vodi, voqi, iodi, and ioqi are the direct and quadrature components of voi and ioi
in Fig. 3.11. As shown in Fig. 3.11, the primary voltage control strategy for each
DG aligns the output voltage magnitude on the d-axis of the corresponding reference
frame. Therefore,
{█(v_odi^*= 〖E_i〗^*-D_Qi Q_i@v_oqi^*= 0)┤								(3.9)
The block diagram of the voltage controller is shown in Fig. 3.13. The differential
algebraic equations of the voltage controller are written as


{█((φ_di ) ̇= 〖v_odi〗^*-v_odi@(φ_qi ) ̇= 〖v_oqi〗^*-v_oqi )┤									(3.10)
{█(〖i_ldi〗^*= F_i i_odi-〖〖ω_b C〗_fi v〗_oqi+K_PVi (〖v_odi〗^*-v_odi )+K_IVi φ_di@〖i_lqi〗^*= F_i i_oqi+〖〖ω_b C〗_fi v〗_odi+K_PVi (〖v_oqi〗^*-v_oqi )+K_IVi φ_qi )┤			(3.11)
where φ_di and φ_qiare the auxiliary state variables defined for PI controllers in
Fig. 3.13 and ωb is the nominal angular frequency. Other parameters are shown in
Figs. 3.11 and 3.13.

{█((ξ_di ) ̇= 〖i_ldi〗^*-i_ldi@(ξ_qi ) ̇= 〖i_lqi〗^*-i_lqi )┤									(3.10)
{█(〖v_idi〗^*= -〖ω_b L〗_fi i_lqi+K_PCi (〖i_ldi〗^*-i_ldi )+K_ICi ξ_di@〖v_iqi〗^*= +〖ω_b L〗_fi i_ldi+K_PCi (〖i_lqi〗^*-i_lqi )+K_ICi ξ_qi )┤				(3.11)

where ξ_di and ξ_qi are the auxiliary state variables defined for the PI controllers 
i_ldi and i_lqi are the direct and quadrature components of i_li in Fig. 3.11.
Other parameters are shown in Figs. 3.11 and 3.14.
The differential equations for the output LC filter and output connector are as
follows:
(i_ldi ) ̇= -R_fi/L_fi  i_ldi+ω_i i_lqi 〖+1/L_fi  v〗_idi-〖1/L_fi  v〗_odi					(3.12)
(i_lqi ) ̇= -R_fi/L_fi  i_lqi+ω_i i_ldi 〖+1/L_fi  v〗_iqi-〖1/L_fi  v〗_oqi 					(3.13)
(v_odi ) ̇=ω_i v_oqi 〖+1/C_fi  i〗_ldi-〖1/C_fi  i〗_odi							(3.14)
(v_oqi ) ̇=〖-ω〗_i v_odi 〖+1/C_fi  i〗_lqi-〖1/C_fi  i〗_oqi							(3.15)


(i_odi ) ̇= -R_ci/L_ci  i_odi+ω_i i_oqi 〖+1/L_ci  v〗_odi-〖1/L_ci  v〗_bdi					(3.16)
(i_oqi ) ̇= -R_ci/L_ci  i_oqi-ω_i i_odi 〖+1/L_ci  v〗_oqi-〖1/L_ci  v〗_bqi					(3.17)
Equations (3.7)–(3.17) form the large-signal dynamical model of the ith DG.
The large-signal dynamical model can be written in a compact form as
{█((x_i ) ̇=f_i (x_i)-k_i (x_i)D_i 〖+g〗_i (x_i)u_i@y_i= 〖h_i (x〗_i))┤							(3.18)
where the state vector is
 x_i=〖[δ_i   P_i   Q_i   φ_di   φ_qi   ξ_di   ξ_qi   i_ldi   i_lqi   v_odi   v_oqi   i_odi   i_oqi]〗^T
The term D_i=〖[ω_com v_bdi  v_bqi]〗^T is considered as a known disturbance. The
detailed expressions for f_i (x_i ), k_i (x_i) and g_i (x_i) can be extracted from (3.7) to (3.17).

3.2.2 Current-Controlled Voltage Source Inverters
The block diagram of a current-controlled voltage source inverter (CCVSI)-based DG is shown in Fig. 3.15. It contains an inverter bridge, connected to a primary DC power source. The current controller adjusts the direct and quadrature terms of output current ioi. As shown in Fig. 3.15, a control block is used to calculate the angle of the ith CCVSI reference frame with respect to the common reference frame αi such that the quadrature term of output voltage voqi becomes zero. This control block is named as αi calculator.
The block diagram of the current controller is shown in Fig. 3.17. The differential
algebraic equations of the current controller are written as

(ξ_di ) ̇= i_drefi-i_odi									 (3.18)
(ξ_qi ) ̇= i_qrefi-i_oqi									 (3.19)
〖v_idi〗^*= v_odi-〖ω_b L〗_fi i_oqi+K_PCi (i_drefi-i_odi )+K_ICi ξ_di			 (3.20)
〖v_iqi〗^*= v_oqi+〖ω_b L〗_fi i_odi+K_PCi (i_qrefi-i_oqi )+K_ICi ξ_qi		 	 (3.21)






















 
3.3 Control of DC Microgrids
Although inverter-based AC Microgrids have been prevalent, DC Microgrids are currently emerging at distribution levels. The DC nature of emerging renewable energy sources (e.g., solar) or storage units (e.g., batteries and ultra-capacitors, super-capacitors) efficiently lends itself to a DC microgrid paradigm that avoids redundant conversion stages. Many of the new loads are electronic DC loads (e.g., in data centers). Even some traditional AC loads, e.g., induction machines, can appear as DC loads when controlled by inverter-fed drive systems. Moreover, DC Microgrids can overcome some disadvantages of AC systems, e.g., transformer inrush current, frequency synchronization, reactive power flow, phase unbalance, and power quality issues.
3.3.1 Control Objectives 
A DC microgrid is an interconnection of DC sources and DC load through a transmission/distribution network. Given the intermittent nature of electric loads, sources must be dynamically controlled to provide load power demand at any moment, while preserving a desired voltage at consumer terminals. Sources may reflect a variety of rated powers. It is desired to share the total load demand among these sources in proportion to their rated power; such load sharing approach is widely known as proportional load sharing. This approach prevents overstressing of sources and helps to span lifetime of the power-generating entities in the microgrid. While the source voltages are the sole variables controlling power flow, they must be tightly managed to also ensure a desirable voltage regulation.

3.3.2 Standard Control Technique


 
Chapter 4: Distributed Control of AC Microgrids

The traditional secondary control of Microgrids discussed in Chap. 3 exploits a centralized control structure. Central controllers command globally based on gathered system-wide information and require a complex and in some cases two-way communication network. All DGs are commanded by communications from a single central controller. This adversely affects system flexibility and configurability and increases reliability concerns by posing a single point of failure. The single point of failure means that if the central controller fails, the whole control system fails. In this chapter, distributed control structure is used to implement the secondary control of Microgrids. A Microgrid can be considered as a multi-agent system where its DGs are the energy nodes (agents). Figure 4.1 shows a distributed communication structure that takes advantage of the multi-agent environment for a microgrid system with DGs as agents. A distributed structure of the communication network improves the system reliability. In this control structure, the control protocols are distributed on all DGs. Therefore, the requirement for a central controller is obviated and the control system does not fail down subsequent to outage of a single unit.

In this chapter, we take advantage of the graph theory notions and distributed control methods in Chap. 3 to design improved, distributed, and sparse communication networks for Microgrids. The distributed cooperative control of multi-agent systems can be used to implement the secondary control of Microgrids. The term “distributed” means that the controller utilizes a communication network by which each agent only receives information from its neighboring agents. The term “cooperative” means that, in contrast to the competitive control, all agents act as one group toward a common synchronization goal and follow cooperative decisions.

Distributed Cooperative Control (DCC) of multi-agent systems was vigorously discussed in many literatures. DCC is categorized into the regulator synchronization problem and the tracking synchronization problem. In the regulator synchronization problem, also called leaderless consensus, all agents synchronize to a common value that is not prescribed or controllable. In the tracking synchronization problem, all agents synchronize to a leader node that acts as a command generator. Neighboring agents can communicate with each other. The leader is only connected to a small portion of the agents.

The secondary control of Microgrids is similar to the tracking synchronization problem of a multi-agent system where the DG voltages and frequencies are required to track their prescribed nominal values. The dynamics of DGs in Microgrids are nonlinear and non-identical. Therefore, a method known as input–output feedback linearization is used here to transform the nonlinear heterogeneous dynamics of DGs to linear dynamics. Input–output feedback linearization transforms the secondary voltage control problem to a second-order multi-agent tracking synchronization problem. On the other hand, the secondary frequency control is transformed to a first-order multi-agent tracking synchronization problem using input–output feedback linearization. Based on the transformed dynamics, fully distributed voltage and frequency control protocols are derived for each DG.

The proposed distributed controls are implemented through a sparse communication network, with only one-way communication links, where each DG requires only its own information and the information of its neighbors.

4.1 Distributed Secondary Frequency Control
In this section, distributed cooperative control techniques for multi-agent systems are used to design secondary frequency controllers for Microgrids. A method known as input–output feedback linearization can be used as shown here to transform the nonlinear heterogeneous dynamics of DGs to linear dynamics. Once input–output feedback linearization is applied, the secondary frequency control leads to a first-order multi-agent synchronization problem. Fully distributed frequency control protocols are derived for each DG that synchronizes the DG frequencies to the prescribed nominal value. The proposed secondary frequency control is implemented through a sparse communication network. The communication network is modeled by a digraph. Each DG requires only its own information and information from its neighbors on the digraph. This leads to a sparse distributed communication structure that only requires one-way communication links and is more reliable than centralized secondary frequency controls.
4.2 Distributed Secondary Frequency and Power Control
4.2.1 Distributed Cooperative Control Protocol for Frequency and Active Power Sharing
4.2.2 Case Studies 
4.3 Distributed Secondary Voltage Control of AC Microgrids 
4.3.1 Secondary Voltage Control Objectives 
4.3.2 Distributed Secondary Voltage Control Using Feedback Linearization
4.3.3 Case Studies
4.4 Distributed Secondary Voltage and Reactive Power Control of AC Microgrids
 
Chapter 5: Cooperative Control for DC Microgrids 
7.1 Distributed Cooperative Controller for DC Microgrids 
7.1.1 Graphical Representation of DC Microgrids
7.1.2 Cooperative Secondary Control Framework
7.1.3 Voltage Observer
7.2 Analytical Model Development for DC Microgrids
7.2.1 Global Dynamic Model
7.2.2 Guidelines for Controller Design
7.2.3 Steady-State Analysis
7.3 Distributed Adaptive Droop Control for DC Microgrids An Alternative Solution 
7.4 Experimental Performance Evaluation 
7.4.1 Design Procedure 
7.4.2 Droop Controller Versus Cooperative Controller
7.4.3 Load Change Performance Assessment 
7.4.4 Plug-and-Play Capability
7.4.5 Cyber-Link Failure Resiliency.
 
Chapter 6: Conclusion 

 
Chapter 7: References
[1]	A. Bidram, A. Davoudi, and F. L. Lewis, “A multiobjective distributed control framework for islanded AC microgrids,” IEEE Trans. Ind. Informatics, vol. 10, no. 3, pp. 1785–1798, 2014.
[2]	D. E. Olivares et al., “Trends in microgrid control,” IEEE Trans. Smart Grid, vol. 5, no. 4, pp. 1905–1919, 2014.
[3]	J. A. P. Lopes, C. L. Moreira, and A. G. Madureira, “Defining control strategies for analysing microgrids islanded operation,” 2005 IEEE Russ. Power Tech, PowerTech, vol. 21, no. 2, pp. 916–924, 2005.
[4]	N. Hatziargyriou, Microgrid: Architecture and Control, vol. 1, no. 1. 2014.
[5]	A. Bidram and A. Davoudi, “Hierarchical structure of microgrids control system,” IEEE Trans. Smart Grid, vol. 3, no. 4, pp. 1963–1976, 2012.

