# Sinusoidal FK Dataset for Inverse Kinematics

This repository contains a synthetic dataset generated using Forward Kinematics (FK) of a robotic manipulator. The joint angles follow sinusoidal variations to cover a wide range of poses. The resulting end-effector positions in Cartesian coordinates (x, y, z) are recorded for each set of joint angles.

## 📌 Purpose

This dataset was used during a research internship at IIT BHU to train Artificial Neural Networks (ANN) for solving the inverse kinematics (IK) problem. The goal was to predict joint angles from end-effector positions.

## 🧠 Dataset Details

- **Input:** Joint angles (sinusoidal)
- **Output:** Corresponding end-effector positions (x, y, z)
- **Applications:** 
  - Training ML models for IK
  - Evaluating SCG, LM, BR optimizers
  - Simulation of robotic arm movement

## 🛠 How it was generated

The forward kinematics equations were applied using a standard DH parameter model for a 3-DOF/6-DOF arm (depending on your case). Sinusoidal functions were used to vary the joint angles over time, ensuring diverse and smooth motion data.

## 🔍 Example Columns

| θ1 (rad) | θ2 (rad) | θ3 (rad) | x (cm) | y (cm) | z (cm) |
|----------|----------|----------|--------|--------|--------|

## 📂 File

- `sinusoidal_fk_dataset.csv` — The main dataset file.

## 🧪 Usage

Can be directly used with Python (NumPy, Pandas), PyTorch, TensorFlow, or other ML frameworks for model training or testing.

---

Let me know if you'd like a `README.md` template with visuals or code examples too!
