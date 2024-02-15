#### USB Mapping

|Internal [255]||||||
|---|---|---|---|---|---
|ITE |2. UK02 | AppleUSB20XHCIPort |  2 (02000000) | 14200000 | Type 3 |
|Bluetooth |14. UK14 | AppleUSB20XHCIPort | 14 (0e000000) | 14e00000 | Type 3 |


|USB 2.0 [0]||||||
|---|---|---|---|---|---|
|Front Panel 1/2|4. UK04 | AppleUSB20XHCIPort |  4 (04000000) | 14400000 | Type 3|
|Port 1,2,3,4|6. UK06 | AppleUSB20XHCIPort |  6 (06000000) | 14600000 | Type 3 |
|Port 9|7. UK07 | AppleUSB20XHCIPort |  7 (07000000) | 14700000 | Type 3 |
|Port 8|8. UK08 | AppleUSB20XHCIPort |  8 (08000000) | 14800000 | Type 3 |
|Port 7|9. UK09 | AppleUSB20XHCIPort |  9 (09000000) | 14900000 | Type 3 |
|Port 6|10. UK10 | AppleUSB20XHCIPort | 10 (0a000000) | 14a00000 | Type 3 |


|USB 3.0 [3]||||||
|---|---|---|---|---|---|
|Front Panel 2/2|18. UK18 | AppleUSB30XHCIPort | 18 (12000000) | 15200000 | Type 3|
|Port 9 |21. UK21 | AppleUSB30XHCIPort | 21 (15000000) | 15500000 | Type 3 |
|Port 8 |22. UK22 | AppleUSB30XHCIPort | 22 (16000000) | 15600000 | Type 3 |
|Port 7 |23. UK23 | AppleUSB30XHCIPort | 23 (17000000) | 15700000 | Type 3 |
|Port 6 |24. UK24 | AppleUSB30XHCIPort | 24 (18000000) | 15800000 | Type 3 |

|USB C 2.0 [8]||||||
|---|---|---|---|---|---|
|Port 5 |5. UK05 | AppleUSB20XHCIPort |  5 (05000000) | 14500000 | Type 3 |

|USB C 3.0 [9]| (No Internal Switch)|||||
|---|---|---|---|---|---|
|Port 5 |20. UK20 | AppleUSB30XHCIPort | 20 (14000000) | 15400000 | Type 3 |

#### Comandos
Habilitar as Ports selecionadas: `14,2,6,10,9,8,7,4,24,23,22,21,18,20,1`

Alterar Tipo das Ports:
- Internas: `T:2,14:255`
- USB 2.0: `T:4,6,7,8,9,10:0`
- USB 3.0: `T:18.21.22.23.24:3`
- USB C 2.0: `T:1:8`
- USB C 3.0: `T:20:9`