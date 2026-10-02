# Drive Calculation

## 1. Design Parameters

The main parameters of the conveyor are:

- Conveyor length: 1.2 m
- Belt width: 0.3 m
- Maximum load: 20 kg
- Belt speed: 0.3 m/s
- Conveyor type: Slider bed
- Pulley diameter: 80 mm

I selected a slider bed because the conveyor is relatively short and
the maximum load is only 20 kg. The construction is also simpler than
a roller bed.

## 2. Load Friction

The weight force of the maximum load is:

F_G = m * g

F_G = 20 * 9.81 = 196.2 N

For the first calculation, a friction coefficient of 0.25 is used.

F_R,load = 0.25 * 196.2

F_R,load = 49.05 N

## 3. Belt Friction

The belt mass per area is 4.1 kg/m².

The area of the upper belt section is:

A = 1.2 * 0.3 = 0.36 m²

Therefore, the belt mass is:

m_belt = 0.36 * 4.1 = 1.476 kg

The weight force is:

F_G,belt = 1.476 * 9.81 = 14.48 N

The friction force of the belt is:

F_R,belt = 0.25 * 14.48 = 3.62 N

## 4. Total Resistance Force

The total resistance force in this simplified model is:

F_R = 49.05 + 3.62

F_R = 52.67 N

## 5. Pulley Torque

The pulley diameter is 80 mm.

r = 0.04 m

The theoretical torque is:

T = F_R * r

T = 52.67 * 0.04

T = 2.11 Nm

For the preliminary design, I use a design factor of 1.5 and
a transmission efficiency of 0.85.

T_design = (2.11 * 1.5) / 0.85

T_design = 3.72 Nm

## 6. Pulley Speed

The required pulley speed is:

n = (60 * v) / (pi * D)

n = (60 * 0.3) / (pi * 0.08)

n = 71.6 rpm

## 7. Power

The theoretical power is:

P = F * v

P = 52.67 * 0.3

P = 15.80 W

With the preliminary design factor and transmission efficiency:

P_design = (15.80 * 1.5) / 0.85

P_design = 27.88 W

## 8. Cross-Check

The angular velocity of the pulley is:

omega = (2 * pi * 71.6) / 60

omega = 7.50 rad/s

Using P = T * omega:

P = 2.11 * 7.50

P = 15.83 W

This is close to the result of 15.80 W calculated with P = F * v.

## 9. Preliminary Drive Requirements

The first calculation gives the following requirements:

- Pulley speed: about 72 rpm
- Theoretical torque: 2.11 Nm
- Preliminary design torque: 3.72 Nm
- Theoretical power: about 15.8 W
- Preliminary design power: about 27.9 W

The next step is to select and compare suitable geared motors.
