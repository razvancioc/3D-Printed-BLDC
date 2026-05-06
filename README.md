# 3D-Printed-BLDC
# 3D Printed 12N14P BLDC Motor 🚧 (Work in Progress)

![CAD](https://img.shields.io/badge/Design-Fusion%20360-orange.svg)
![Hardware](https://img.shields.io/badge/Hardware-3D%20Printed-lightgrey.svg)
![Status](https://img.shields.io/badge/Status-Work%20in%20Progress-yellow.svg)

A fully customizable, experimental Brushless DC (BLDC) motor designed to be 3D printed. This project explores the limits of 3D printing in high-RPM applications (up to 20,000 RPM) using a **12N14P** configuration optimized for drones (4S batteries, ~1350 KV). 

*Note: This project is currently under active development and construction.*

---

## 📖 Overview

This motor is being designed from the ground up to overcome the classic challenges of 3D-printed motors (e.g., plastic melting, eddy currents, and high-RPM hoop stress). By combining 3D-printed plastic with reinforcement elements (Kevlar/Cyanoacrylate), steel cores (insulated nails) for the stator, and high-quality bearings, the goal is to build a motor capable of delivering real, usable torque.

### Technical Specifications (Target)
* **Configuration:** 12 Stator Teeth / 14 Rotor Poles (12N14P)
* **Target RPM:** 20,000 RPM at 14.8V (4S Battery)
* **Motor Constant (KV):** ~1350 KV
* **Winding Scheme:** dLRK (A-b-C-a-B-c-A-b-C-a-B-c)
* **Windings:** 0.5 mm enameled copper wire (3 strands in parallel per turn), 13 turns/tooth.

---

## 🛠️ Bill of Materials (BOM)

| Component | Specifications / Details | Quantity |
| :--- | :--- | :--- |
| **Magnets** | Neodymium, flat (5x5x1 mm) | 14 pcs |
| **Bearings** | MR84ZZ metal shielded (4x8x3 mm) | 2 pcs |
| **Central Shaft** | Steel / Stainless Steel, 4 mm diameter | 1 pc |
| **Copper Wire** | Enameled, 0.5 mm diameter | ~10 meters |
| **Stator Core** | Thin steel nails (varnish-insulated) | - |
| **Adhesive / Resin** | Loctite 638 (shaft), Epoxy Resin (magnets) | - |
| **3D Parts** | Stator, Rotor (Bell), Base (PETG / ABS / PC) | 1 Set |

---

## 📸 Build Log & Assembly (Ongoing)

### 1. 3D Printing the Components
The parts are being printed with strict tolerances in mind. The stator features 4 mm walls for the teeth, and the rotor has an internal 14-sided polygonal profile to ensure a perfectly flat mounting surface for the magnets.

![3D Printed Parts](path/to/your-printed-parts-image.jpg)
*> Add a picture of the freshly printed Stator and Rotor here.*

### 2. Stator Assembly & Winding
To increase efficiency and reduce overheating, the center of each plastic tooth is filled with steel (varnish-insulated nails). The winding is being done manually following the dLRK scheme. To support currents up to 20A, 3 strands of 0.5 mm wire are routed in parallel.

![Wound Stator](path/to/your-wound-stator-image.jpg)
*> Add a close-up picture of the copper wound around the stator here.*

### 3. Rotor (Bell) Assembly
The magnets are secured using epoxy resin, strictly following the **North-South** alternating pole rule. The designed pockets allow for a perfect slide-in fit, maintaining a 0.5 - 0.8 mm air gap from the stator.

To prevent the motor from exploding due to centrifugal force (hoop stress), the exterior of the bell will be wrapped in Kevlar thread and sealed with Cyanoacrylate.

![Rotor Assembly](path/to/your-rotor-magnets-image.jpg)
*> Add a picture of the inside of the rotor, showing the glued magnets.*

![Kevlar Reinforcement](path/to/your-kevlar-wrap-image.jpg)
*> Add a picture of the exterior of the rotor and the retaining ring here.*

### 4. Final Assembly (Pending)
The 4 mm shaft will be press-fitted into the rotor, passed through the MR84ZZ bearings mounted in the center of the stator, and secured with a C-clip at the bottom.

![Assembled Motor](path/to/your-final-motor-image.jpg)
*> Add a picture of the fully assembled motor here once completed.*

---

## ⚡ Upcoming Testing & Calibration

Once the build is complete, the following tests will be performed using a standard drone ESC and an optical tachometer:

1. **No-Load KV Test:** Measuring the RPM without a propeller at a known voltage.
2. **Turn Adjustment:** If the RPM differs from the targeted 1350 KV, the number of turns will be adjusted using the calibration equation from the design phase.
3. **Load Test:** Mounting a 6" or 7" propeller and monitoring the stator temperature.

---

## ⚠️ Safety Warning
This motor is designed to reach extremely high speeds (20,000 RPM). A faulty 3D print or weak magnet adhesion can lead to catastrophic rotor failure and disintegration. **Always wear safety goggles during testing and never stand in the rotational plane of the propeller!**
