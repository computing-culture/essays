## DirectX Coverage with Earliest Supported Runtime

● Native: VPU/GPU drivers target this DX version *and* VPU/GPU accelerates DX features in hardware  
◐ Compatible: VPU/GPU drivers instantiate software orchestration (common) or software emulation (uncommon)  
○ Incompatible  

| Card                      | Earliest DX install | DX3 | DX5 | DX6 | DX7 | DX8 | DX9 |
| ------------------------- | ------------------- | --- | --- | --- | --- | --- | --- |
| S3 ViRGE                  | DX1                 | ●   | ○   | ○   | ○   | ○   | ○   |
| Voodoo1                   | DX3                 | ●   | ●   | ○   | ○   | ○   | ○   |
| Voodoo2                   | DX5                 | ◐   | ●   | ○   | ○   | ○   | ○   |
| Banshee (SGRAM)           | DX5                 | ◐   | ●   | ●   | ○   | ○   | ○   |
| Voodoo3 2000              | DX6                 | ◐   | ◐   | ●   | ○   | ○   | ○   |
| TNT2 (128-bit)            | DX6                 | ◐   | ◐   | ●   | ◐   | ○   | ○   |
| Matrox G200               | DX6                 | ◐   | ◐   | ●   | ◐   | ○   | ○   |
| Savage4 Pro               | DX6                 | ◐   | ◐   | ●   | ◐   | ○   | ○   |
| Rage 128 Pro              | DX6                 | ◐   | ◐   | ●   | ◐   | ○   | ○   |
| Matrox G450               | DX6                 | ◐   | ◐   | ●   | ◐   | ○   | ○   |
| Radeon 7000 (128-bit)     | DX6                 | ◐   | ◐   | ●   | ◐   | ○   | ○   |
| GeForce2 MX               | DX7                 | ◐   | ◐   | ◐   | ●   | ○   | ○   |
| GeForce4 MX (128-bit)     | DX7                 | ◐   | ◐   | ◐   | ●   | ○   | ○   |
| Radeon 7200 (DDR)         | DX7                 | ◐   | ◐   | ◐   | ●   | ○   | ○   |
| Kyro II (Hercules 4000)   | DX7                 | ◐   | ◐   | ◐   | ◐   | ○   | ○   |
| GeForce3                  | DX8                 | ◐   | ◐   | ◐   | ◐   | ●   | ○   |
| Radeon 9000               | DX8                 | ◐   | ◐   | ◐   | ◐   | ●   | ○   |
| Radeon 9200 (128-bit)     | DX8                 | ◐   | ◐   | ◐   | ◐   | ●   | ○   |
| GeForce FX 5200 (128-bit) | DX9                 | ◐   | ◐   | ◐   | ◐   | ◐   | ◐   |
| Radeon 9550 (128-bit)     | DX9                 | ◐   | ◐   | ◐   | ◐   | ◐   | ●   |
| Radeon 9600 (128-bit)     | DX9                 | ◐   | ◐   | ◐   | ◐   | ◐   | ●   |
| Radeon 9700 Pro           | DX9                 | ◐   | ◐   | ◐   | ◐   | ◐   | ●   |
| Radeon X1650              | DX9                 | ◐   | ◐   | ◐   | ◐   | ◐   | ●   |
| Radeon HD 3650            | DX9                 | ◐   | ◐   | ◐   | ◐   | ◐   | ●   |

Note1: Some cards are technically exceptional for having multiple driver sets targeting different DX versions  
Note2: Some cards do not target a DX version that they fully implement in hardware

## Citation

Computing Culture. *Table: DirectX / VPU and GPU Compiled Reference*.  
Computing Culture Essays, 2026.  
https://github.com/computing-culture/essays
