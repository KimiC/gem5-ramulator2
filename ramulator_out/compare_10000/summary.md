| Config | ECC | DRAM model | Mitigation model | Reads | ACT | PRE | REFab | VRR | RFM/DRFM | Fault trials | Raw flips | Corrected flips | Visible flips | Raw flip ratio | Visible flip ratio | Cycles | Finding |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| DDR4-2400R | off | DDR4-VRR | OracleRH tRH=4 | 10000 | 9999 | 8952 | 2134 | 2135 | 0 | 0 | 0 | 0 | 0 | 0.000000 | 0.000000 | 9999000 | VRR triggered |
| DDR4-3200AA | off | DDR4-VRR | OracleRH tRH=4 | 10000 | 9999 | 9197 | 1602 | 1602 | 0 | 0 | 0 | 0 | 0 | 0.000000 | 0.000000 | 9999000 | VRR triggered |
| DDR5-3200BN | off | DDR5 | Command count only | 10000 | 9999 | 8431 | 3214 | 0 | 0 | 0 | 0 | 0 | 0 | 0.000000 | 0.000000 | 9999000 | RFM/DRFM not issued |
| DDR5-3200BN-RFM | off | DDR5 | DDR5RFM tRH=4 directed-rfm | 10000 | 9999 | 8431 | 3214 | 0 | 357 | 0 | 0 | 0 | 0 | 0.000000 | 0.000000 | 9999000 | RFM/DRFM issued |
| DDR4-3200AA-Fault | off | DDR4 | RowHammerFaultModel tRH=4 P=0.5 | 10000 | 9999 | 9197 | 1602 | 0 | 0 | 2403 | 1174 | 0 | 1174 | 0.488556 | 0.488556 | 9999000 | Injected flips are visible |
| DDR5-3200BN-Fault | off | DDR5 | RowHammerFaultModel tRH=4 P=0.5 | 10000 | 9999 | 8431 | 3214 | 0 | 0 | 535 | 268 | 0 | 268 | 0.500935 | 0.500935 | 9999000 | Injected flips are visible |
| DDR5-3200BN-ECC-Fault | on-die SBC/128b | DDR5 | RowHammerFaultModel tRH=4 P=0.5 | 10000 | 9999 | 8431 | 3214 | 0 | 0 | 535 | 268 | 268 | 0 | 0.500935 | 0.000000 | 9999000 | ECC corrected injected single-bit flips |
