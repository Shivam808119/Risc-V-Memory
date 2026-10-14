# Sources and scope

This static site combines architecture teaching with guided investigation of ten RISC-V core families. General explanations are educational summaries. Core-specific facts should be verified against the exact release/configuration being studied.

## Official starting points

- SERV: https://github.com/olofk/serv
- PicoRV32: https://github.com/YosysHQ/picorv32
- Ibex docs: https://ibex-core.readthedocs.io/en/latest/ and https://github.com/lowRISC/ibex
- VEGA project: https://github.com/vega-processor
- CV32E40P manual: https://docs.openhwfoundation.org/projects/cv32e40p-user-manual/en/cv32e40p_v1.3.2/intro.html and https://github.com/openhwgroup/cv32e40p
- Rocket Chip: https://github.com/chipsalliance/rocket-chip
- SweRV: https://github.com/chipsalliance/Cores-SweRV
- VexRiscv: https://github.com/SpinalHDL/VexRiscv
- BOOM/SonicBOOM docs: https://docs.boom-core.org/ and https://github.com/riscv-boom/riscv-boom
- Shakti: https://shakti.org.in/ and https://github.com/shaktiproject

## Useful public documentation references consulted

- PicoRV32 README describes its native valid/ready interface and byte strobes: https://github.com/YosysHQ/picorv32
- Ibex instruction-fetch interface documentation: https://github.com/lowRISC/ibex/blob/master/doc/03_reference/instruction_fetch.rst
- CV32E40P user manual describes OBI instruction and data interfaces: https://docs.openhwfoundation.org/projects/cv32e40p-user-manual/en/cv32e40p_v1.3.2/intro.html
- VexRiscv README lists simple/cached bus plugins and optional translation support: https://github.com/SpinalHDL/VexRiscv

## Scope cautions

- “Supports” does not mean “enabled in your build.”
- A prefetch FIFO is not automatically a cache. A TLB caches translations, not data. A bus buffer is not necessarily a cache.
- ISA requirements, core microarchitecture, generated configuration, SoC interconnect, memory controller and board wiring are separate layers.
- NUMA is relevant when the actual platform has non-uniform memory domains; it is not an intrinsic feature of every RISC-V core.
- Roofline is a performance model, not a hardware block.
- Cache coherence is not automatically guaranteed by the RISC-V ISA; it depends on the memory system and platform.
- For a technical report, record exact repository commit, parameters, SoC configuration and source evidence.
