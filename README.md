# BIST-Design-and-Implementation
Test setup using Random Test Socket (RTS) as well as STUMPS BIST architecture was designed to calculate fault coverage for given Netlist. This individual project was carried out on ModelSim.

Proposed System:
1. Scan Insertion
This provides the scan for accessing state flip flops inputs and outputs in CUT. It is required to facilitate the test generated by the AECpt. The original netlist is modified in such a way that it includes the necessary scan flip flops and signals.
2. RTS Architecture
The RTS BIST Architecture adds a PRPG to the primary inputs of the circuit, the MISR to the primary output and SRSG and SISA to the beginning and end of the scam inserted internal state flip flops. Size and polynomial configurable LFSRs are used for PRPG, MISR, SRSG, SISA. The use of parameterized and configurable LFSRs and RTS controller enables to improve fault coverage by adjusting the parameters.
