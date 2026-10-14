# PhysioThermal Lab: Deep Heat & Ultrasound Tissue Simulation

An interactive clinical biophysics simulator designed for physical therapy, rehabilitation, and medical engineering students and clinicians.

## Features

1. **Real-World Clinical Parameters & Dosimetry**:
   - **Therapeutic Ultrasound (US)**:
     - Frequency selector: **1.0 MHz** (Deep targets: 3–5 cm) vs. **3.0 MHz** (Superficial targets: 1–2.5 cm, 3x heating rate).
     - Intensity: Real clinical SATA intensity slider from **0.20 to 2.80 W/cm²** with live Total Acoustic Power (Watts) calculated across Effective Radiating Area (ERA: 5.0 cm²).
     - Duty Cycle: **Continuous (100% Thermal)**, **Pulsed 50%**, **Pulsed 20% (Non-thermal / Acoustic streaming)**, and **Pulsed 10% (Cellular repair)**.
     - Acoustic Coupling: **Optimal Gel Layer (100%)** vs. **Suboptimal / Air Gap**.
   - **Diathermy (SWD / MWD)**:
     - Inductive Coil (Drum, 27.12 MHz) vs. Capacitive Plates (27.12 MHz) vs. Microwave (MWD, 2450 MHz).
     - Power Output: Adjustable from **10W to 300W** (Dose I Sub-thermal to Dose IV Vigorous).
     - Towel Layer & Perspiration: Dry cotton towel vs. Damp/sweat scald hazard simulation.
   - **Treatment Duration & Accumulation**:
     - Treatment duration from **1.0 to 15.0 minutes**.
     - Live elapsed session timer with Play / Pause / Reset and dynamic thermal saturation curve.

2. **Ultrasound Movable Mode vs. Stationary Hazard**:
   - **Movable Mode (Safe Clinical Technique)**: Continuous stroking technique (1.5 to 5.5 cm/s). Glides the transducer across the skin and evenly distributes acoustic energy without focal hotspots.
   - **Stationary Mode (Critical Hazard)**: Simulates the dangerous consequence of holding the ultrasound head still. Triggers acoustic standing waves at the cortical bone interface, rapid periosteal temperature spike (>43°C), flashing burn warning, and periosteal pain alarms.
   - Interactive touch and mouse drag on the transducer head.

3. **Live Tissue Thermal & Burn Monitors**:
   - Continuous real-time temperature (°C) and physiological status for 5 anatomical layers:
     - **Epidermis & Skin**: Normal &rarr; Erythema &rarr; Cutaneous Pain & Blister Burn (>44°C).
     - **Subcutaneous Adipose (Fat)**: Safe &rarr; Capacitive SWD Overheating & Adipose Necrosis Risk (>43°C).
     - **Skeletal Muscle Belly**: Mild &rarr; Moderate &rarr; Optimal Collagen Stretch Window (40–42°C) &rarr; Overheating (>44°C).
     - **Joint Capsule / Deep Tendon**: Viscoelastic elongation zone.
     - **Bone Periosteum**: Safe &rarr; Acoustic Standing Wave Periosteal Bone Burn (>43°C).

4. **Vercel & Modern Web Ready**:
   - Zero-dependency client-side HTML5 canvas + Tailwind CSS + Lucide Icons + Tone.js.
   - Fully responsive for mobile phones, tablets, laptops, and 4K displays.
   - Ready for instant deployment on [Vercel](https://modalitysimulation.vercel.app/).


