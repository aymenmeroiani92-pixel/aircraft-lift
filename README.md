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
