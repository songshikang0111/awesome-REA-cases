# RTP084 and Agilex 7: TANG reports AI-assisted architecture, DMA and 100G optical-link research

Category: Hardware and interoperability · Other AI-assisted work
Record date: 2026-11-20
Stage: Needs verification

At 08:43:29 Beijing time on November 20, 2026, TANG (@roobtx) reports an R&S RTP084 and Intel Agilex 7 F-Tile project in a model-comparison post. The post describes the oscilloscope as 8 GHz/40 GSa/s and the FPGA work as 100GBASE-SR4 optical interconnect, listing architecture analysis, PCIe BAR0 dual-DMA reverse engineering and 25.78125 Gbps on-die two-dimensional diamond eye scans. The goal is low-level understanding and a physical test loop for instruments and an optical link, not routine frontend coding.

The same author's English version at 08:44:43 adds ADME 64-by-64 phase/voltage slices and 16-tap FFE cascades, claiming zero dropped frames across 45.87 million frames under Clause 91 RS(528,514) hardware error injection. All are author reports. Link configuration, counters, sampling interval, error records, scripts and original measurements were not obtained. Zero frame loss is not a complete bit-error or stability assessment.

The author frames this as Gemini/GPT industrial work but does not map individual models to oscilloscope, DMA or eye-scan tasks, nor substantiate the claimed six-month architectural gap. The separate six-vendor FPGA/EDA vulnerability project in the post has its own entry; its 145 sessions and over 16,700 tool steps are not assigned to this project. Retrieval confirms attribution, not technical validation of the images; the short-linked article was not read. No code, instruments or experiments were run here, and REA is unmentioned.

November 20 sealed snapshots: Chinese post 0 likes/57 views, English post 1 like/85 views; engagement does not validate hardware measurements.

## Sources

- [TANG's Chinese RTP084/Agilex 7 report, November 20, 2026 at 08:43:29 Beijing time](https://x.com/i/status/2123577937744248874)
- [Same-author English report adds ADME, FFE and measurement claims, November 20, 2026 at 08:44:43 Beijing time](https://x.com/i/status/2123578249922204015)

[中文](../tang-rtp084-agilex7-ai-dma-optical-link-report.md) | [Back to editor picks](../../README.md) | [Full index](../../INDEX.en.md) | [Category](../../categories/en/hardware.md)
