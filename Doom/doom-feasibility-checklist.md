# Doom Feasibility Checklist — LG Octane (VN530)

A quick-reference guide for evaluating the possibility of running Doom on the LG Octane safely.

---

## 1️⃣ Gather Information
- [ ] Document phone specs:
  - CPU: Qualcomm MSM6500 (~200–300 MHz)  
  - RAM: 128 MB  
  - Screen: 240×320, 16-bit color  
  - Storage: internal + microSD  
  - OS: BREW 3.x  
  - Input: keypad / directional pad

---

## 2️⃣ Identify Challenges
- [ ] Note platform limitations (BREW requires signed apps)  
- [ ] Record CPU and RAM constraints  
- [ ] Assess screen and input limitations  
- [ ] Evaluate storage availability

---

## 3️⃣ Determine Requirements for a Port
- [ ] Access BREW SDK for compilation  
- [ ] Modify Doom source code for:
  - Keypad controls  
  - 240×320 resolution  
  - Reduced memory usage  
- [ ] Identify carrier signing or emulator requirements

---

## 4️⃣ Plan Safe Experimentation
- [ ] Use an emulator to simulate Octane hardware and controls  
- [ ] Test dummy BREW apps (graphics, input, audio)  
- [ ] Track memory, CPU, and storage usage for analysis

---

## 5️⃣ Document Findings
- [ ] Record all observations in `research/doom-feasibility.md`  
- [ ] Highlight limitations and potential improvements  
- [ ] Keep the checklist updated for future research

---

> ⚠️ **Important:** Do NOT attempt flashing, unlocking, or bypassing carrier restrictions. Focus on analysis, simulation, and safe experimentation only.
