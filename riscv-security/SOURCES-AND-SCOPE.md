# Sources and scope

This website is an educational guide, not a security certification or a full audit.

## Architectural references
- [RISC-V Privileged Architecture — introduction](https://docs.riscv.org/reference/isa/priv/priv-intro.html)
- [RISC-V Machine ISA — PMP description](https://docs.riscv.org/reference/isa/priv/machine.html)
- [RISC-V Smepmp specification](https://docs.riscv.org/reference/isa/priv/smepmp.html)
- [RISC-V ratified specifications library](https://docs.riscv.org/)
- [RISC-V Security Model project](https://github.com/riscv/riscv-security-model)
- [Ibex security features documentation](https://ibex-core.readthedocs.io/en/latest/03_reference/security.html)
- [PicoRV32 project and memory interface](https://github.com/YosysHQ/picorv32)
- [CV32E40P documentation](https://cv32e40p.readthedocs.io/)
- [Rocket Chip repository](https://github.com/chipsalliance/rocket-chip)
- [BOOM documentation](https://docs.boom-core.org/)
- [VexRiscv repository](https://github.com/SpinalHDL/VexRiscv)
- [SERV documentation](https://serv.readthedocs.io/)
- [SweRV cores repository](https://github.com/chipsalliance/Cores-SweRV)
- [Shakti project](https://shakti.org.in/)

## Interpretation rules
- RISC-V ISA/privileged specifications define architectural behavior; they do not prove that a given core implements every optional mechanism.
- Core-specific claims must be tied to a release, commit, configuration and SoC integration.
- Security features in a documentation page may be optional, compile-time configured, runtime configured, or dependent on a wrapper.
- A CPU's PMP does not automatically constrain DMA or every other bus master.
- Secure boot, debug lifecycle, key provisioning, firmware policy and most peripheral isolation are system-level concerns.
- Side-channel and fault-injection resistance require a threat model and evidence; they cannot be inferred from the ISA name.
- Mark findings as **verified**, **inferred**, or **unknown**. Never turn an unverified assumption into a factual claim.

## Recommended evidence record
Record the exact source revision, file and line, configuration, test setup, expected result, observed result, logs/waveforms, and residual risk.
