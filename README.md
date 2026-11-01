# LM1875-simple-board
Hello everyone, im here showing my homemade design about LM1875 amplifier board, with no low pass filter, high pass filter or anything else, except the amps.

**INFO:**
The amp is set at 10 gain (Rf = 22k & Rg = 1k ohm), anyway you can
put ur own and custom resistor value on R6, R7, R10 and R11.

# How it works?
The board works in BTL (Bridge Tier Load) mode, or in S (Single) mode.
You can put the same signal on INA and INB for BTL, and if you want Stereo, please be sure what INA and INB has L and R channels of audio (fr sht🥀).

# Absolute Maximum Ratings
1)Input AC voltage (RMS): ±18V (limited by the Opamp, M5218AL) or ±30V (Maximum voltage supported by LM1875).

2)Output power: 30W RMS (±15V, BTL, 8Ω load) or 15W RMS (±15V, SL, 4Ω/IC).

3)Maximum TDP: 6W (±30V) or 3W (±15V) (no load).

4)Audio Signal Input (INA and INB): -VEE to VCC (this is calculated by multiplying the AC input RMS voltage by the square root of 2

| Vdc (GND to -VEE or +VCC) = (Vrms (AC) * √2) / 2 |


*WARNING: this will only give you the rail-to-rail voltage from a common reference point (ground).

# Extra cautions

Please be sure what your AC voltage doesn't exceed the absolute maximum rating, and don't load the amplifier with 4 ohms in BTL mode, the ICs it will burn (the resistance of each one sees is Rload / 2).

ICs can dissipate large amounts of energy, so make sure your heatsink is powerful enough for them.

**Next changes upcoming later...**
