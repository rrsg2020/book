# Protocol

<p style="text-align:justify;">
Participants were instructed to acquire data for T1 mapping data using the spin-echo inversion recovery protocol for T1 mapping as reported in (Barral et al. 2010), as detailed in Table 2. This protocol uses four inversion times optimized for human brain T1 values and uses a relatively short TR (2550 ms). It’s important to note that this acquisition protocol is not suitable for T1 mapping fitting models that assume TR > 5T1. Instead, more general models of inversion recovery, such as the Barral et al. fitting model described in Section 2.4.1, can be used to fit this data.
</p>

<b style="text-align:justify;">
Table 2. Imaging protocol for inversion recovery T1 mapping proposed  to the participants for the 2020 joint RRSG-qMRSG reproducibility challenge. The protocol is the brain imaging protocol used in (Barral et al. 2010), and which is meant for the T1 values observed in healthy human brains.
</b>

| Pulse Sequence                     | Spin-echo inversion recovery   |
| :---                               |          :----:                | 
| **Repetition Time (TR)**           | 2550 ms                        |
| **Inversion Time (TI)**            | 50, 400, 1100, 2500 ms         |
| **Echo Time (TE)**                 | 14 ms                          |
| **In-plane resolution**            | 1x1 mm<sup>2</sup>             |
| **Slice thickness**                | 2 mm                           |

<p style="text-align:justify;">
Participants were advised to adhere to this protocol as closely as possible, but to report any differences in protocol parameters due to technical limitations of their scanners and/or software. The recommended data exportation type was complex (magnitude & phase, or real & imaginary), and magnitude-only data was also acceptable if complex data could not be exported.
</p>