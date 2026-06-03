# 🤖 Obstacle Avoiding Robot

An autonomous obstacle-avoiding robot built with Arduino, using an ultrasonic sensor and servo motor to detect and navigate around obstacles in real time.

---

## ✨ How It Works

The robot moves forward continuously. When an obstacle is detected within **15cm**, it:

1. Stops and backs up
2. Scans **right** then **left** using a servo-mounted ultrasonic sensor
3. Turns toward whichever direction has more open space
4. Continues moving forward

---

## 🧰 Hardware Required

| Component | Quantity |
|-----------|----------|
| Arduino Uno | 1 |
| L293D Motor Shield (AF Motor Shield) | 1 |
| DC Motors | 4 |
| HC-SR04 Ultrasonic Sensor | 1 |
| Servo Motor (SG90 or similar) | 1 |
| Robot Chassis + Wheels | 1 set |
| Battery Pack | 1 |
| Jumper Wires | As needed |

---

## 📌 Pin Configuration

| Pin | Connected To |
|-----|--------------|
| A0 (TRIG_PIN) | Ultrasonic Sensor Trigger |
| A1 (ECHO_PIN) | Ultrasonic Sensor Echo |
| Digital 10 | Servo Motor Signal |
| Motor Shield M1–M4 | DC Motors 1–4 |

---

## 📚 Libraries Required

Install these from the Arduino Library Manager:

- **AFMotor** — Adafruit Motor Shield library
- **NewPing** — Ultrasonic sensor library
- **Servo** — Built-in Arduino servo library

---

## 🚀 Getting Started

1. Assemble the chassis and mount all motors, the sensor, and the servo
2. Connect the ultrasonic sensor to pins **A0** (Trig) and **A1** (Echo)
3. Attach the servo signal wire to pin **10**
4. Place `obstacle_avoiding_robot.ino` inside a folder of the **same name**
5. Open the folder in **Arduino IDE**
6. Install the required libraries
7. Select your board: `Tools → Board → Arduino Uno`
8. Select the correct port: `Tools → Port`
9. Click **Upload**

---

## ⚙️ Key Settings

| Parameter | Value | Description |
|-----------|-------|-------------|
| `MAX_DISTANCE` | 200 cm | Maximum sonar range |
| `MAX_SPEED` | 190 | Maximum motor speed (0–255) |
| Obstacle threshold | 15 cm | Distance to trigger avoidance |
| Servo center | 115° | Forward-facing position |
| Servo right | 50° | Right scan position |
| Servo left | 170° | Left scan position |

---

## 👥 Team

| Name | GitHub |
|------|--------|
| Shruti Khisa | [@ShrutiKhisa](https://github.com/ShrutiKhisa) |
| Farhan Tanvir | [@FarhanTanvir](https://github.com/FarhanTanvir) |
| Shaira Akhter Diba | [@ShairaDiba](https://github.com/ShairaDiba) |
| Fazli Rabbi Noor | [@FarhanNoor](https://github.com/FarhanNoor) |

##  Status
 completed

