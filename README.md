# aircraft-lift
Simple project to calculate lift force of an aircraft wing using Python.
# lift.py
# حساب قوة الرفع لجناح طائرة

# المتغيرات
rho = 1.225   # كثافة الهواء (kg/m^3)
V = 70        # سرعة الطائرة (m/s)
S = 16        # مساحة الجناح (m^2)
Cl = 1.2      # معامل الرفع

# معادلة الرفع
L = 0.5 * rho * V**2 * S * Cl

print(f"قوة الرفع = {L:.2f} نيوتن")
# lift.py
rho = 1.225   # air density (kg/m^3)
V = 70        # velocity (m/s)
S = 16        # wing area (m^2)
Cl = 1.2      # lift coefficient

L = 0.5 * rho * V**2 * S * Cl
print(f"Lift Force = {L:.2f} N")
# drag.py
rho = 1.225   # air density
V = 70        # velocity
S = 16        # wing area
Cd = 0.03     # drag coefficient

D = 0.5 * rho * V**2 * S * Cd
print(f"Drag Force = {D:.2f} N")
# ld_ratio.py
L = 9500  # lift force (N)
D = 350   # drag force (N)

ratio = L / D
print(f"Lift-to-Drag Ratio = {ratio:.2f}")
# stall.py
Cl_max = 1.5   # maximum lift coefficient
slope = 0.1    # lift curve slope (per degree)

stall_angle = Cl_max / slope
print(f"Approximate Stall Angle = {stall_angle:.1f} degrees")
# range.py
import math

V = 200        # velocity (m/s)
c = 0.6        # fuel consumption (1/hr)
L_D = 15       # lift-to-drag ratio
Wi = 60000     # initial weight (N)
Wf = 40000     # final weight (N)

R = (V / c) * L_D * math.log(Wi / Wf)
print(f"Aircraft Range = {R:.2f} km")
# endurance.py
import math

c = 0.6        # fuel consumption (1/hr)
L_D = 15       # lift-to-drag ratio
Wi = 60000     # initial weight (N)
Wf = 40000     # final weight (N)

E = (1 / c) * L_D * math.log(Wi / Wf)
print(f"Aircraft Endurance = {E:.2f} hours")
