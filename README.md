# Automatic Water Tank Level Indicator Using 8085

**Name:** Ruqsaar Shaikh  
**Roll No.:** 18049

## Aim
To design and simulate an Automatic Water Tank Level Indicator using the 8085 microprocessor in GNUsim8085.

## Software Used
- GNUsim8085

## Working
The 8085 reads the water-level input from I/O port `00H` and sends the corresponding value to output port `01H`.

### Water Level Indication

| Input | Output | Water Level |
|------|--------|-------------|
| 00H | 00H | LOW |
| 01H | 01H | MEDIUM |
| 02H | 02H | FULL |

## 8085 Program

```asm
IN 00H
OUT 01H
HLT
