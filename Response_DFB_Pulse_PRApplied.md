----------------------------------------------------------------------

# Report of Referee A -- NB10105/Nefedkin

----------------------------------------------------------------------

*This paper theoretically studied the ultrafast response time of a plasmonic distributed feedback laser in the large-signal modulation regime. The authors demonstrated the dependence of response limit with pump spot size using both numerical and analytical approaches. The identification on different ultrafast stages and insights on pump-tunable lasing dynamics could facilitate the applications of plasmon lasers in optoelectronic devices.*

**Review**

*However, the manuscript focused on plasmonic nanohole arrays with a specific parameter design (100-nm hole, 470-nm spacing and 100-nm film thickness). Are the conclusions on the critical pump spot size and ultrafast response limit (1 ps) general enough to plasmon nanohole array lasers in different design parameters (film thickness, hole size, spacing)? Also, plasmon lasers based on nanohole arrays and nanoparticle arrays show different lasing mechanisms from surface plasmon polariton and surface lattice resonances, respectively. It is not a fair comparison between the calculated response time of plasmon nanohole arrays and experimental results of nanoparticle arrays to verify the accuracy of theoretical modeling (final paragraph, the introduction section).*

**Response**

Note that the pump spot effectively excites the EM field inside the pumped area which forms an effective laser mode. The existence of the *critical* size of the pump beam corresponds to the size of the effective mode. Qualitatively, the size of the effective mode is equal to the characteristic propagation length of the EM field along the plasmonic structure, which is$\sim v_{\text{group}}/ \gamma_a$. When the size of the pump beam is greater than the size of the effective laser mode, the response time almost does not depend on the size of the pump beam. When the size of the pump beam becomes smaller than the size of the effective laser mode, the response time increases with the decrease of the pump beam size.

The effective laser mode is formed by the Bloch modes of a periodic plasmonic structure which determine a characteristic group velocity and a dissipation constant. Of course, modes in different types of structure have different group velocities and relaxation constants. Nevertheless, from the qualitative arguments presented above, there is always the *critical* size of the pump beam, for which the response time is minimal.

However, the specific value of the time response strongly depends on the type of the plasmonic structure. Indeed, the response time depends on the Rabi constant of interaction. In turn, the Rabi constant is determined by the volume of the plasmonic mode which is different for surface plasmon-polariton and surface lattice resonances. In our numerical simulations, we consider plasmon lasers based on nanohole arrays, though in the work [[Daskalakis, Konstantinos S., et al. *Nano letters* 18.4 (2018): 2658-2665.](https://pubs.acs.org/doi/abs/10.1021/acs.nanolett.8b00531)] the experiment has been conducted for plasmon lasers based on nanoparticle arrays in the different geometry. In this regard, we agree with the referee that the comparison of the response times obtained in the experiment and in our simulations is not a fair verification of the accuracy of our theoretical modeling. 

In the revised version of the manuscript, we reformulate the last paragraph in the <u>Introduction</u> section by excluding this direct comparison between our theory and the experiment. In <u>Conclusion</u>, we add the qualitative arguments that the *critical* size of the pump beam is a common feature for plasmonic DFB lasers.



**Review**

*In addition, can the authors more explanations and rationales on how experimental conditions such as pump size and pump power density (excitation fluence) are incorporated in the modeling?*

**Response**

In our modeling, we take into account a large number of atoms, which have different coordinates $\textbf{r}_m​$. The coupling constant between $j​$th mode of the plasmonic structure and $m​$th atom depends on atom's coordinates as
$$
\Omega _{jm} =  - {{\bf{d}}_m} \cdot {{\bf{E}}_j}({{\bf{r}}_m})/ \hbar
\tag{1}
$$

where the electric field is taken at the position of the $m$th atom. The Rabi constants enter as coefficients in the Eqs. (1) – (3).

The pulse pump of the active medium enters as an initial condition for the atomic population inversion. The initial value of the population inversion for the atoms whose coordinates lie inside the area of the pumping spot is $D_0$. Initial population inversions of other atoms equal to $-1$, i.e. they are in the ground state. The *size* of the pump beam enters as an area, inside which atoms are excited. 

Pump power density (excitation fluence) enters through the value of $D_0​$. The connection between them has the form 
$$
\frac{D_0 + 1}{2} = \eta \frac{P_0 \Delta t}{n_c S l \hbar \omega}
\tag{2}
$$
Here $P_0$ is power of the laser pulse pump; $\Delta t$ is duration of the pump pulse; $n_c$ is the concentration of atoms of the active medium; $S$ is the area of the pump beam; $l$ is the width of the active medium layer; $\hbar \omega$ is the transition frequency of the atom; and $(D_0 + 1)/2$ is the population of the excited state arising due to the pump pulse. 

Thus, we assume that the entire pulse energy comes to the excitation of atoms of the active medium. In real experiment, there are additional circumstances as a result of which a part of the energy from pulse pumping does not come into the active medium. These circumstances are taken into account as an additional coefficient $\eta <1$ in a right-hand side of (2). 

In our simulations **the power of the pump pulse** is $P_0 \approx ​$. This value is typical for experiments carried out with the same plasmonic structure in the same geometry, see [[F. Beijnum, P. Veldhoven, E. Geluk, M. Dood, G. Hooft, and M. van Exter, *Phys. Rev. Lett.* 110, 206802 (2013).](https://journals.aps.org/prl/abstract/10.1103/PhysRevLett.110.206802)].

Note that the dependence of the response time on the pump beam size is observable in a wide range of $D_0$ values, and a fine tune of the pumping power is not necessary to observe the predicted dependency.

In the revised manuscript, we add explanations on how experimental conditions, such as pump size and pump power density  are incorporated in the modeling.



**Review**

*Did the authors consider any diffractive coupling between nanoholes in the equations of system dynamics, given that pump size may influence the resonance mode quality (Purcell factor) and EM fields near the holes?*

**Response**

Diffractive coupling between nanoholes is taken into account in laser equations (1) – (3).

First, we have found the EM field distribution of the Bloch modes of the plasmonic structure within the coupled-mode theory. Note that the first order of the coupled-mode theory describes the hybridization of initially non-interacting SPP modes through scattering on the holes, i.e. takes into account diffractive coupling **[]**. Scattering rates have been taken from Ref. [[V. T. Tenner, A. N. van Delft, M. J. A. de Dood, and M. P. van Exter, *Journal of Optics* 16, 114019 (2014)](https://iopscience.iop.org/article/10.1088/2040-8978/16/11/114019/meta)] for the plasmonic laser based on Au film perforated by the nanoholes array. The coupled-mode theory with such scattering rates demonstrates good agreement with the experimental measurement of the band-structure of the plasmonic nanohole arrays laser [[V. T. Tenner, A. N. van Delft, M. J. A. de Dood, and M. P. van Exter, *Journal of Optics* 16, 114019 (2014)](https://iopscience.iop.org/article/10.1088/2040-8978/16/11/114019/meta)]. 

Second, we use the obtained EM field distributions to calculate the Rabi constants between the Bloch modes and atoms of the active medium. These Rabi constants, the eigenfrequencies and the relaxation rates of the Bloch modes enter the laser equations (1) – (3). The Eqs. (1) – (3) determine the amplitude of each Bloch mode. The amplitudes depend on the interaction between the Bloch mode and active atoms, and, as a consequence, on the pump beam size. The field of the collective mode is formed by the large number of Bloch modes of a periodic plasmonic structure. As a result, the volume of the collective mode changes with a change in the pump beam size. The Purcell factor and the rates of the spontaneous and stimulated emissions also change. The strongest change occurs when the diameter of the pump beam is less than the critical value, at which the strongest dependence of the response time on the diameter appears.

Note that in our modeling the diameter of the pump beam is always much larger than the period of the nanohole array. For this reason, we do not take into account effects on the boundary of the pump beam.

In the revised manuscript, we add the description of the band-structure of the plasmonic nanoholes array laser in the <u>Section 2</u> of the main part of the manuscript and the <u>Appendix</u>.



**Review**

*Also, how is the Rabi constant in the modeling related to the Purcell factor of a specific plasmon cavity? More justifications are needed.*

**Response**

We added the derivation of the Rabi constant through the parameters of the plasmonic structure and the active medium in the revised version of the manuscript , see <u>Section 2</u> in main part of the text and the <u>Appendix</u>.



**Review**

*We have other comments below*

**1.** *On page 4, the authors claimed that “The time independence of the EM field distribution allows us to consider the plasmonic laser as a single mode laser,” but they need to justify how the time evolution of EM field is correlated to single-mode approximation. Is there any effect from high-order diffractive modes for the hole arrays? Why does the EM field distribution slightly change from Fig 3d to 3f?*

**Response**

In our simulations we take into account $\sim 500$ Bloch modes of the plasmonic structure which form together the EM field distribution in the active medium. However, our simulations show that the *resulting* EM field distribution slightly changes in the first and second stage of the output pulse evolution. In other words, there is a dynamical equilibrium between relaxation and propagation of the EM field outside the pump beam on the one hand, and the stimulated amplification of the EM field in the active medium on the other hand. We use the fact of the constancy of the EM field distribution to construct the single-mode model. We consider that there is a single collective mode, the EM field distribution of which coincides with the EM field distribution found in the numerical simulations of the multimode problem. This assumption allows to derive the single-mode laser equations. The results obtained in the framework of the single-mode model are in good agreement with the results of the multimode model, see Figs. 2(a), 4 and Fig. 5a.

The change of the EM field distribution from Fig. 3d to 3f is associated with a stronger decrease of the population inversion in the third stage of the response. This leads to a violation of  the dynamical equilibrium between relaxation, propagation of the EM field and the stimulated amplification of the EM field in the system. As a result, the EM field distribution begins to change, and the intensity of the EM field begins to decrease.

We added the appropriate explanations in the revised version of the manuscript.



**2.** *Regarding the figures, the order of Figure 5b and 5a can be switched since 5b appeared earlier in the main text. In Figure 5b, what are the units of t_delay? Figure 3 needs additional labeling such as scale bar and timing point of chosen snapshots, and the authors can add more explanations in the figure caption such as the meaning of dashed circles.*

**Response**

We have made the required changes. We changed the order of Figs. 5a and 5b. We indicated the units for $t_\text{delay}$ in Fig. 5b. We added a scale bar to the Fig. 3; we indicated in the figure caption the time
moments corresponding to the intensity field distributions in Figs. 3. We described the meaning of dashed circles in the Fig. 3.



**3.** *The authors point out the similarity of Eq. (15) to the time dependence of a superradiant burst, and how that system resembles the current problem and approach (page 6). The parallelism between these two systems is interesting; however, these few sentences seem out of place relative to the major discussion on ultrafast stages of the laser response. We suggest this information be moved to the introduction or conclusion section, and presented as either as potential motivation or future prospect of study.*

**Response**

We placed all mentions to the superradiance problem to the <u>Conclusion</u> section of the manuscript and noted the potential interest in studying the similarity of the observed phenomenon and superradiance.



----------------------------------------------------------------------

# Report of Referee B -- NB10105/Nefedkin

----------------------------------------------------------------------

*In this manuscript, the Authors theoretically analyze the dynamics of a two-dimensional lasing system, consisting of a periodic metallic sheet supporting plasmonic modes, coated with a lasing material. The dynamics of the lasing phenomenon is studied as a function of the size of the pump laser which generates the population inversion in the lasing material. The Authors find that the response time of the laser, i.e. the delay between the input pump pulse and the output laser pulse, decreases with the size of the pump beam.*

*I find that this manuscript is very well written, with a concise and instructive introductory section. The main result of this work, i.e. the dependence of the response time on the pump beam size, is clearly stated. The Authors also motivate why the study of the response time is important for optoelectronic devices. I recommend this paper for publication, but I kindly ask the Authors to address the two points that I raise below.*

**Review**

*My main criticism of the paper concerns the statement that the calculations reveal an "optimal" beam size, yielding the shortest response time. From Fig.2(b) one sees that the shortest response time corresponds to a very flat minimum in the red curve. I doubt the robustness of this minimum as the system's parameters, or the level of approximation of the theory, are changed. I strongly suggest that the Authors rephrase the text, claiming that $d \sim 15 \mu\text{m}​$ corresponds to the minimum size to achieve a short response time, and not the optimal size.*

**Response**

We agree with the referee that the minimum is flat and some unaccounted effects, such as non-ideal plasmonic structure, inhomogeneous distribution of the active medium, etc., may change the value of the size beam for which the response time is minimal. We rephrase the text claiming that $d \sim 15 \mu \text{m}​$ corresponds to the minimum size to achieve the short response time for considered structure, rather than the optimal size.

**Review**

*My second criticism is that the parameters used to calculate the results in Fig.2 are not given in the text. It is written that Fig.1 corresponds to the solution of Eqs.(1)-(3), but what is the size of the device, how many modes are considered, i.e. what are the values of the Rabi couplings, etc.? (The parameters are given only for the single-mode approximation.)*

**Response**

**2.** We have indicated the parameters of the plasmonic DFB laser in the main part of the manuscript. We have added a description of the mode structure of the plasmonic laser and a method for calculating the values of the constants (Rabi constant, the relaxation rates, etc.) from the laser equations (1) – (3). We also add <u>Appendix</u> in the revised manuscript.