---
name: Bug report
about: Create a report to help us fix things
title: "<VAC1_RX_Gain> OUTPUT LEVEL always 0 dB at StartUP (even when set at -40)"
labels: bug
assignees: ''

---

**Describe the bug**
When Thetis is first launched and started, The <VAC1_RX_Gain> (and  <VAC2_RX_Gain>) actually OUTPUT 0 dB, no matter what they were set at when Thetis was last shutdown, or what they show on the panel or in the setup.
Thetis v2.10.3.8 x64
Anan 10E Firmware v1.5 Protocol 1

**To Reproduce**
1. Set the VAC1 RXGain slider on panel to -40
2. Shutdown Thetis
3. Start Thetis
4. Notice that the VAC1 RXGain slider on panel is still -40
5. Observe the VAC1 level on any application such as WSJT-X and/or Spectrum Lab.  It is MUCH higher than normal.
6. Now "bump" the VAC1 RXGain slider on panel to -39.
7. Observe that the VAC1 level on WSJT-X and/or Spectrum Lab IS NOW CORRECT.

**Expected behaviour**
I expect that the VAC RXGain level would behave based on it's set value at startup.


**Screenshots**
If applicable, add screenshots to help explain your problem.

**Desktop (please complete the following information):**
 - OS: Windows 10 Home / 64

**Additional context**
The only ways I have found to fix the incorrect output level, is to change the VAC RXgain setting on panel or in SETUP by +/- 1 dB, which corrects the OUTPUT level for the VAC immedialely.  However, the failure occurs the next time (everytime) Thetis is launched.
