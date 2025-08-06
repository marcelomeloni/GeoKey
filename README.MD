
# 🔐 Geometric Key Vault

A beautiful and interactive single-page application where cryptography meets geometry.

This project allows users to **generate a numeric private key**, **transform it into a slope (m)** of a straight line, and **securely store/reconstruct** the key using two deterministic points from that line.

> 🔎 Inspired by the idea of turning sensitive data into mathematical representations.

---

## 🚀 Features

- ✅ Numeric private key generation (78 digits)
- ✅ Converts key into slope (m) for a straight line
- ✅ Derives two deterministic points (x, y) from the slope
- ✅ Allows reverse operation: input two points → recover key
- ✅ Modern UI/UX with Tailwind CSS and shadcn/ui
- ✅ Fully interactive, single-page application (SPA)
- ✅ Styled after the Phantom Wallet aesthetic (dark + purple tones)

---

## 🧠 How It Works

1. **Generate Key**  
   A 78-digit numeric private key is randomly generated.

2. **Convert to Slope (m)**  
   The private key is transformed into a floating-point number:  
   `0.[privateKey] → slope (m)`

3. **Create 2 Points on the Line**  
   Example:
Point A: (0, 0)
Point B: (1, m)
Equation: y = m * x


4. **Store or Share Safely**  
You only need two points to reconstruct the slope, and therefore the private key.

5. **Recover the Key**  
Input the same points → recover the exact private key.

---

## 📸 Screenshot

> *Include here a screenshot or GIF of the UI once available.*

---

## 📦 Tech Stack

- **React + Vite**
- **Tailwind CSS**
- **shadcn/ui** (UI components)
- **Framer Motion** (animations)
- **TypeScript** (optional, recommended)

---

## 🛠️ Setup & Run Locally

```bash
git clone https://github.com/your-username/geometric-key-vault.git
cd geometric-key-vault
npm install
npm run dev
