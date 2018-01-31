# Quantum Chemistry Speed Test

**The rules**: Calculations must only use a single core. The B3LYP used should be that used by default by Gaussian and NWChem (namely the VWN3 not VWN5). And please, no Gaussian input files or results.

Various people have submitted results:
- [Eric Berquist](http://github.com/berquist/qmspeedtest)
- [Karol Langner](http://github.com/langner/qmspeedtest)
- [Michael Banck](http://github.com/mbanck/qmspeedtest)
- [Noel O'Boyle](http://github.com/baoilleach/qmspeedtest)
- [Pedro Silva](http://github.com/PedroJSilva/qmspeedtest)

Please fork the [original repo](http://github.com/baoilleach/qmspeedtest) and submit your own!

## Eric Berquist's results

**Machine:** AMD Opteron(tm) Processor 6172 [Magny Cours] @ 2.10 GHz running 64-bit RHEL 6

**Fancy compiler or maths libraries used when compiling:** Intel compilers w/ MKL (various versions)

### HF

| QM Package | Version    | Time (min) | Steps | per step | Total E           | HOMO        | LUMO       |
| ---------- | -------    | ---------- | ----- | -------- | -------           | ----        | ----       |
| DALTON     | 2013.2     | 26.8       | 19    | 1.41     | -644.675706212821 | -0.35364477 | 0.07433447 |
| DALTON     | 2015.0     |            |       |          |                   |             |            |
| GAMESS     | 2013-05-01 | 10.74      | 30    | 0.36     | -644.6757056212   | -0.3536     | 0.0744     |
| NWChem     | 6.1.1      | 26.1       | 20    | 1.30     | -644.675706608673 | -0.3536105  | 0.07435037 |
| ORCA       | 2.9.1      | 28.61      | 13    | 2.20     | -644.675706036271 | -0.353622   | 0.074344   |
| ORCA       | 3.0.1      | 24.95      | 13    | 1.92     | -644.675706036270 | -0.353622   | 0.074344   |
| ORCA       | 3.0.3      | 24.78      | 13    | 1.91     | -644.675706017977 | -0.353613   | 0.074351   |
| Q-Chem     | 4.1.0.1    | 6.08       | 14    | 0.43     | -644.675706161474 | -0.354      | 0.074      |
| Q-Chem     | 4.3.0      | 5.57       | 14    | 0.40     | -644.6757061614   | -0.354      | 0.074      |
| TURBOMOLE  | 6.6        | 14.73      | 20    | 0.74     | -644.67570607014  | -0.35367    | 0.07431    |

### B3LYP

| QM Package | Version    | Time (min) | Steps | per step | Total E            | HOMO        | LUMO        |
| ---------- | -------    | ---------- | ----- | -------- | -------            | ----        | ----        |
| DALTON     | 2013.2     | 123.0      | 20    | 6.15     | -648.4956905852    | -0.26060842 | -0.06441321 |
| DALTON     | 2015.0     |            |       |          |                    |             |             |
| GAMESS     | 2013-05-01 | 153.3      | 41    | 3.74     | -648.4956883277    | -0.2601     | -0.0641     |
| NWChem     | 6.1.1      | 66.4       | 27    | 2.46     | -648.495694154848  | -0.2605694  | -0.06439231 |
| ORCA       | 2.9.1      | 39.29      | 14    | 2.81     | -648.495621346673  | -0.260530   | -0.064412   |
| ORCA       | 3.0.1      | 33.72      | 13    | 2.59     | -648.495620645754  | -0.260533   | -0.064445   |
| ORCA       | 3.0.3      | 32.18      | 13    | 2.47     | -648.495620579978  | -0.260515   | -0.064433   |
| Q-Chem     | 4.1.0.1    | 12.51      | 14    | 0.89     | -648.495723730569  | -0.260      | -0.064      |
| Q-Chem     | 4.3.0      | 10.98      | 14    | 0.78     | -648.4957237305999 | -0.260      | -0.064      |
| TURBOMOLE  | 6.6        | 15.50      | 23    | 0.67     | -648.49565883340   | -0.26099    | -0.06464    |

**Machine:** Intel(R) Xeon E5-1620(R) @ 3.60 GHz running 64-bit Ubuntu 13.10

**Fancy compiler or maths libraries used when compiling:** Intel Parallel Studio XE 2013 SP1 (Compiler v14.0.1/MKL v11.1.1)

### HF

| QM Package | Version         | Time (min) | Steps | per step | Total E           | HOMO        | LUMO       |
| ---------- | -------         | ---------- | ----- | -------- | -------           | ----        | ----       |
| DALTON     | 2013.0          | 10.3       | 19    | 0.5      | -644.675706212821 | -0.35364477 | 0.07433447 |
| MPQC       | 2.3.1, Ubuntu   | 28.3       | 28    | 1.0      | -644.6757062224   | -0.353644   | 0.074333   |
| NWChem     | 6.3, Ubuntu     | 8.7        | 20    | 0.4      | -644.675706609025 | -0.3536110  | 0.07435021 |
| ORCA       | 2.9.1           | 13         | 13    | 1.0      | -644.675706036270 | -0.353622   | 0.074344   |
| ORCA       | 3.0.1           | 11         | 12    | 0.9      | -644.675706036272 | -0.353622   | 0.074344   |
| Psi        | 4.0.0b5, Ubuntu |            |       |          |                   |             |            |
| Q-Chem     | 4.1.0.1         | 2.6        | 14    | 0.2      | -644.675706161474 | -0.354      | 0.074      |

### B3LYP

| QM Package | Version         | Time (min) | Steps | per step | Total E           | HOMO        | LUMO        |
| ---------- | -------         | ---------- | ----- | -------- | -------           | ----        | ----        |
| DALTON     | 2013.0          | 42.6       | 20    | 2.1      | -648.4956905852   | -0.26060842 | -0.06441321 |
| MPQC       | 2.3.1, Ubuntu   | 143.8      | 25    | 5.8      | -648.4957002690   | -0.260571   | -0.064391   |
| NWChem     | 6.3, Ubuntu     | 26         | 27    | 1.0      | -648.495694167510 | -0.2605703  | -0.06439253 |
| ORCA       | 2.9.1           | 18         | 14    | 1.3      | -648.495621346649 | -0.260530   | -0.064412   |
| ORCA       | 3.0.1           | 14.5       | 13    | 1.1      | -648.495620645744 | -0.260533   | -0.064445   |
| Psi        | 4.0.0b5, Ubuntu |            |       |          |                   |             |             |
| Q-Chem     | 4.1.0.1         | 4.8        | 14    | 0.3      | -648.495723730572 | -0.260      | -0.064      |

## Baoilleach's results

**Machine:** Intel(R) Core(TM) i7-2600 CPU @ 3.40GHz running 64-bit Centos 6.3

**Fancy compiler or maths libraries used when compiling:** None (system gcc, blas, lapack)

### HF

| QM Package | Version | Time (min) | Steps | per step | Total E       | HOMO      | LUMO     |
| ---------- | ------- | ---------- | ----- | -------- | -------       | ----      | ----     |
| erkale     | r1013   | 810        | 90    | 9        | -644.67570139 | -0.353712 | 0.074269 |
| NWChem     | 6.3     | 8.8        | 20    | 0.4      | -644.67570661 | -0.353611 | 0.074350 |

### B3LYP

| QM Package | Version | Time (min) | Steps | per step | Total E        | HOMO      | LUMO      |
| ---------- | ------- | ---------- | ----- | -------- | -------        | ----      | ----      |
| erkale     | r1013   | 933        | 58    | 16.1     | -648.49566820  | -0.260899 | -0.064457 |
| NWChem     | 6.3     | 27.6       | 27    | 1.0      | -648.495694167 | -0.260570 | -0.064393 |

## Michael Banck's results

**Machine:** Lenovo T400 (Intel(R) Core(TM)2 Duo CPU     P8400  @ 2.26GHz)

**Fancy compiler or maths libraries used when compiling:** Debian 7 packages

### HF

| QM Package | Version  | Time (min) | Steps | per step | Total E       | HOMO      | LUMO     |
| ---------- | -------  | ---------- | ----- | -------- | -------       | ----      | ----     |
| erkale     | r1013    | 3394       | 90    | 37.7     | -644.67570139 | -0.353712 | 0.074269 |
| MPQC       | 2.3.1    | 64         | 28    | 2.3      | -644.67570622 | -0.353644 | 0.074333 |
| Psi4       | 4.0beta5 | 115        | 16    | 7.2      | -644.67570580 | -0.353619 | 0.074353 |
| NWChem     | 6.1      | 21         | 23    | 0.9      | -644.67570680 | -0.353608 | 0.074350 |
| NWChem     | 6.3r2    | 19         | 20    | 1.0      | -644.67570661 | -0.353611 | 0.074350 |

### B3LYP

| QM Package | Version  | Time (min) | Steps | per step | Total E        | HOMO      | LUMO      |
| ---------- | -------  | ---------- | ----- | -------- | -------        | ----      | ----      |
| erkale     | r1013    | 9065       | 58    | 156.3    | -648.495668200 | -0.260899 | -0.064457 |
| MPQC       | 2.3.1    | 387        | 25    | 15.4     | -648.495700269 | -0.260571 | -0.064391 |
| Psi4       | 4.0beta5 | 190        | 16    | 11.9     | -648.495697810 | -0.260556 | -0.064363 |
| NWChem     | 6.1      | 56         | 27    | 2.1      | -648.495694155 | -0.260569 | -0.064392 |
| NWChem     | 6.3r2    | 55         | 27    | 2.0      | -648.495694168 | -0.260570 | -0.064393 |

## MY NAME HERE's results

**Machine:** Description of one CPU and the OS

**Fancy compiler or maths libraries used when compiling:** Intel compiler? MKL?

### HF

| QM Package | Version | Time (min) | Steps | per step | Total E | HOMO | LUMO |
| ---------- | ------- | ---------- | ----- | -------- | ------- | ---- | ---- |
|            |         |            |       |          |         |      |      |

### B3LYP

| QM Package | Version | Time (min) | Steps | per step | Total E | HOMO | LUMO |
| ---------- | ------- | ---------- | ----- | -------- | ------- | ---- | ---- |
|            |         |            |       |          |         |      |      |
