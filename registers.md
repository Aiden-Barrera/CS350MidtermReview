# Intel x86-64 Registers

## General Purpose Registers (64-bit)

| 64-bit | 32-bit | 16-bit | 8-bit High | 8-bit Low |
|--------|--------|--------|------------|-----------|
| RAX    | EAX    | AX     | AH         | AL        |
| RBX    | EBX    | BX     | BH         | BL        |
| RCX    | ECX    | CX     | CH         | CL        |
| RDX    | EDX    | DX     | DH         | DL        |
| RSI    | ESI    | SI     | -          | SIL       |
| RDI    | EDI    | DI     | -          | DIL       |
| RBP    | EBP    | BP     | -          | BPL       |
| RSP    | ESP    | SP     | -          | SPL       |

## Extended Registers (R8-R15)

| 64-bit | 32-bit | 16-bit | 8-bit Low |
|--------|--------|--------|-----------|
| R8     | R8D    | R8W    | R8B       |
| R9     | R9D    | R9W    | R9B       |
| R10    | R10D   | R10W   | R10B      |
| R11    | R11D   | R11W   | R11B      |
| R12    | R12D   | R12W   | R12B      |
| R13    | R13D   | R13W   | R13B      |
| R14    | R14D   | R14W   | R14B      |
| R15    | R15D   | R15W   | R15B      |

## Notes

- **AH, BH, CH, DH**: High 8-bit portions of AX, BX, CX, DX (legacy registers only)
- **SIL, DIL, BPL, SPL**: Low 8-bit portions (available in 64-bit mode with REX prefix)
- **R8-R15**: Extended registers introduced with x86-64, no high 8-bit variants
- All registers can be accessed at different sizes depending on the instruction used
