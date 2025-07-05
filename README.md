<p align="center">
  <img src="Assets/Indian_Space_Research_Organisation_Logo.svg.png" alt="ISRO Logo" width="140" height="120"/>
  &nbsp;&nbsp;&nbsp;
  <img src="Assets/3.png" alt="NARL Logo" width="140" height="140"/>
  &nbsp;&nbsp;&nbsp;
  <img src="Assets/0.png" alt="INSA" width="140" height="140"/>
  &nbsp;&nbsp;&nbsp;
  <img src="Assets/1.png" alt="INSA Logo" width="140" height="140"/>
  &nbsp;&nbsp;&nbsp;
  <img src="Assets/2.png" alt="INSA Logo" width="140" height="140"/>
  &nbsp;&nbsp;&nbsp;
</p>

# Detection and Spectral Analysis of Convection-Triggered Gravity Waves Using Ground-Based LIDAR Remote Sensing

📍 **Institution:** National Atmospheric Research Laboratory (NARL), Gadanki  
📅 **Duration:** 8 Weeks (Summer Research Fellowship Programme - SRFP 2025)  
👨‍💻 **Intern:** Sudhan R (SRFP Reg. No: ENGS1672)  
🧑‍🏫 **Guide:** Dr. Bhavani Kumar Yellapragada, MSc, Ph.D. (Retd. Scientist, Department of Space, NARL)

---

## 🛰️ Project Overview

This project explores the detection and spectral analysis of convection-triggered gravity waves in the lower atmosphere using high-resolution LiDAR backscatter data. The study was conducted during SRFP 2025 at NARL, aiming to understand atmospheric gravity wave behavior triggered by convective activity.

---

## 🎯 Objectives

- Decode and preprocess Licel-format LiDAR TR files to extract atmospheric backscatter data.
- Generate Range-Time Intensity (RTI) plots to visualize vertical atmospheric oscillations.
- Extract time series data at multiple altitudes and apply Fast Fourier Transform (FFT) for spectral analysis.
- Identify and interpret dominant frequencies and corresponding wave periods.
- Investigate the vertical propagation and nature of gravity waves during the Convective Boundary Layer (CBL) evolution.

---

## 🧪 Methodology

- **Data Source:** Licel binary LiDAR files from NARL (23 January 2014, 16:26–17:57 IST)
- **Data Preprocessing:**
  - Decode binary files into NumPy arrays.
  - Remove background noise and normalize signal.
  - Stack 850+ backscatter profiles into a combined matrix.
- **Visualization:**
  - Create RTI plots showing signal intensity over time and altitude.
- **Spectral Analysis:**
  - Apply FFT on time series from 10 altitude bins (385 m to 409.3 m).
  - Identify dominant frequencies and convert to wave periods.

---

## 📈 Results

| Altitude (m) | Dominant Frequency (Hz) | Wave Period (min) | Interpretation |
|--------------|--------------------------|--------------------|----------------|
| 385.0        | 0.015044                 | ~1.1               | Local noise/turbulence |
| 393.1        | 0.000040                 | ~421.0             | Long-period GW |
| 398.5        | 0.000435                 | ~38.3              | Convective GW  |
| 403.9        | 0.000277                 | ~60.1              | CBL-induced GW |
| 409.3        | 0.000277                 | ~60.1              | CBL-induced GW |

- Consistent wave period of ~421 min observed across multiple altitudes.
- Shorter periods (38–60 min) found at mid-altitudes suggest convection-triggered waves.
- Phase difference analysis confirmed vertical propagation patterns.

---

## 🛠️ Tools and Technologies

- **Languages:** Python 3.10+
- **Libraries:** NumPy, SciPy, Matplotlib, Pandas
- **Environments:** Google Colab, Jupyter Notebook
- **Other Tools:** FFT, RTI Plotting, Spectral Analysis

---

## 💡 Insights and Observations

- RTI plots showed distinct vertical oscillations in backscatter signal.
- Gravity wave activity was strongest between 398 m to 406 m altitude.
- Low-altitude high-frequency signals (~1.1 min) likely represent localized noise.
- Phase progression with height indicates upward wave propagation.

---

## 🔭 Future Scope

- Extend analysis to multi-day LiDAR observations.
- Integrate with meteorological data (e.g., radiosondes, wind, temperature).
- Use advanced spectral methods (Wavelet Transform, EMD).
- Automate decoding and plotting with a full Python pipeline.
- Prepare research paper for journals or conferences.

---

## 🙏 Acknowledgements

I sincerely thank:
- **IAS, INSA, and NASI** for the SRFP 2025 opportunity.
- **Dr. Bhavani Kumar Yellapragada** for invaluable mentorship and insights.
- **NARL, Gadanki** for data, facilities, and support.
- **Sri Eshwar College of Engineering** for institutional encouragement.

---

## 📚 References

- Ratnam et al., 2002 – Gravity wave activity over Gadanki using LiDAR and radiosonde data.
- Tsuda et al., 2000 – Global morphology of gravity waves from GPS data.
- Bhavani Kumar et al., 2006 – LIDAR observations of boundary layer dynamics over tropical stations.
- Full reference list available in the [final report](./FINAL_REPORT_VER_2.pdf).

---

📩 **Contact:** rajansudhan0@gmail.com
