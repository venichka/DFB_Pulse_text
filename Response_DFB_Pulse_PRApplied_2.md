*We appreciate that the authors have made major improvements upon the points we raised previously. In particular, the major comments on rationale for parameter settings, modeling justification, and figure improvements are addressed.*

*In response to our question 'Did the authors consider any diffractive coupling between nanoholes in the equations of system dynamics?', the authors seem to only consider how the pump size affects the mode volumes but not the quality factor. However, the finite boundary of the pump beam can be important in terms of both influencing the mode quality and introducing mode hybridization from edge effect [Nature Communications 8, 13687 (2017)] given the relatively small pump size (~15 um, around 30x30 nanoholes). This might come from the limit in modeling, which the author can further justify.*

**Response**

Indeed, in the single-mode approximation, we suppose that the finite size of the pump beam influences only on the mode volume, but not the mode quality factor. However, our numerical simulations of the full model, Eqs. (1)-(3), which describes mode hybridization inside the finite pump beam and the change of mode quality factors (this is manifested in the radiation pattern and  $\pi$-phase shift for a dark mode, for details see Fig. 8b and 9 in [Nefedkin, Nikita E., et al.  *ACS Photonics* 5.8 (2018): 3031-3039]), demonstrate good agreement with the single-mode approximation, compare Fig. 2 and Fig. 4. 

We also note that the analytical evaluation shows that the delay time of the output pulse does not depend on the quality factor ($\gamma_a^{-1}$), see Eq. (16), which is another argument in favor of using such a single-mode approximation. This conclusion is valid when $\log(N_{\text{at}}) \gg 1$, i.e., when the pump beam size is larger than $\sim5$ $\mu \text{m}$. This size of the pump beam limits our single-mode approximation. 

We have placed this comment in the "Single Mode Approximation" section of the revised version of the manuscript.

---

*We have other comments below*

- *Sentence fragment in paragraph 3 of conclusion, "To sum up there is*
*the diameter..."*
- *Strange phrasing in paragraph 1 of Single Mode Approximation
section, "…We can see that the EM field distribution practically does
not change in the first and second stages". For a more technical
sound, we suggest removing the word "practically" and in general
rewording the sentences to improve flow.*

**Response**

We have taken into account all the comments and changed these points.

- To conclude we have shown that there is the diameter of the pump beam...
- In Eqs. (1)-(3), we take into account several hundred of the Bloch modes of the plasmonic structure, which together form the EM field distribution in the active medium. Numerical simulations show that this distribution does not change in the first and second stages of the system response.

