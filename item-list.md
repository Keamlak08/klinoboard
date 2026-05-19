Drivetrain
- CIM FRC Motor: high torque brushed DC motor that drives the board forward, mounted to the deck with tons of duct tape
- Skateboard (Tony Hawk brand): serves as the chassis, front trucks kept stock for steering
- 3/8" Steel Rod: cut to size as the custom rear axle, ground flat where parts clamp onto it
- Pillow Block Bearings (x2): let the axle spin freely inside the 3D printed truck
- 3D Printed Rear Truck: holds the pillow block bearings and mounts to the underside of the deck
- Motor Sprocket: attaches to the CIM shaft and connects to the chain
- 3d Axle Sprocket: 3d printed and locked onto the steel axle with hot glue, receives power from the chain to spin the wheel
- 25h Chain: transfers rotation from the motor sprocket to the axle sprocket
- 3D Printed Wheel Hub Peg: clamps the rear wheel to the axle so they spin together locked on with hot glue

Power and Electronics
- 3S LiPo Battery 11.1V (x2): only used one, powers motor connected through pwm
- USB Power Bank: powers the ESP32 and all electronics separately from the motor
- PWM: Controlls power regulation to slow down/speed up motor
- ESP32 Dev Module: the brain, handles all logic including NFC auth, and pedal input
- Breadboard + Jumper Wires + Random extension cord wire (for higher gauge): connects all the electronics together without soldering

Special
- diy Foot Pedal: the stash item we wanted but couldnt get, so we hacked it ourself.
  - Carboard / 3D printed spring + spring found from ripping apart some random machine 
  - 2x Accelerometers: Used to find the degree the foot pedal is pressed at to signal power regulation for pwm
- USB NFC Reader: reads the Stasis ID tags to authenticate a rider before the board will move
- Stasis NFC ID Tags: scanned to unlock the board for a timed ride session, motor disables when time runs out
