<h1 align="center">
  <!-- <img height="100" alt="Reality Router MK1" src="https://github.com/user-attachments/assets/c1833c9d-b30f-4daa-8247-d4b9bf5516c3" /> -->
    Reality Router MK2
</h1>
<p align="center"> <i>“From plastic, to infinity and beyond”</i> </p>
<!-- **A custom desktop CNC mill** -->

A custom designed **CNC router** built from **3D printed parts** and an **Ender 3’s electronics system**
<!-- 
<img src="assets/Render.png" width="500px" style="border-radius: 20px">
<span style="display: flex;">
<img src="assets/Onshape1.png" width="200px">
<img src="assets/Onshape2.png" width="200px">
<img src="assets/Onshape3.png" width="200px">
<img src="assets/Onshape4.png" width="200px"> -->

</span>

[Onshape CAD](https://cad.onshape.com/documents/c7ce2f56ba9457b235044411/w/5da64270988a68e8e36d9466/e/d720e5cdc24e29f3d02d7b4e?renderMode=0&leftPanel=false&uiState=6a1f846e9b09696752afb0b3)

## MK2

This is mark 2 of the Reality Router, an upgraded version that aims to fix mechanical issues, overhaul the control system, polish the machine, and more.

Goals:
1. Control system overhaul: I will be switching to Klipper-for-CNC instead of grblHAL + CNC.js because it offers a much more capable system thats actively maintained and also allows me to
    - Add an on-board interface with a 3.5" touchscreen and a joystick that works with KlipperScreen (I'll likely make my own fork for a better CNC interface)
    - See upgrade #2
    - Have a better web interface and use the extensive Klipper plugin ecosystem
2. Spindle Controller: I'll use an additional RP2040 MCU on the toolhead with a couple servo motors to interact with the controls on the spindle
3. Motor Upgrades: I want to upgrade the machine to NEMA23 motors which will also require an upgraded control board, and given the Klipper upgrade I might design a custom PCB or just wire some stepper drivers to an MCU. This will be a pricey upgrade but I'll see where I can cut costs. (Hopefully will get an LDO sponsor).
4. Z Axis Repairs: The biggest design mistake I made was shifting the spindle weight too far out from the X gantry which put too much strain on the PLA. I'll rebalance the weight with an additional linear rail
5. Aluminum Reinforcements: After talking with people at OpenSauce, it was pretty clear the machine needed to be a lot more rigid than it was currently. I'll reinforce all load-bearing brackets with a 1/8" aluminum plate and reprint in PETG-CF
6. Axis Homing: I'll add a XYZ touch probe to auto home axes and also add an E-Stop switch
7. Vacuum Foot: I'll add a foot on the Z gantry to support a shop-vac hose