# 🎮 Romish.gg

Romish.gg is a custom **CS2 10-man matchmaking platform** built to replicate the feel of FACEIT and Premier systems, while being entirely community-driven.  
It includes a real-time queue, ready-up phase, captain draft, map veto, match lobby, and server integration — all managed by a connected **Discord bot** and **DatHost API** backend.

---

## 🚀 Project Overview
The system is divided into three main components:

| Component | Tech Stack | Description |
|------------|-------------|-------------|
| **Frontend** | Vue 3 + Vite + Tailwind | Player interface: queue, draft, map veto, match lobby |
| **Backend** | Node.js + Express + MongoDB | Matchmaking logic, WebSocket connections, Dathost integration |
| **Discord Bot** | Node.js + Discord.js | Handles Discord verification and queue syncing |

All three communicate via secure REST and WebSocket connections.

---

## 💡 Why I Built This
I wanted a **custom matchmaking system** tailored for our CS2 community — something lightweight, scalable, and easy to integrate with both **Steam** and **Discord** APIs.  
FACEIT and third-party pug bots lacked the flexibility to handle queue logic, live veto phases, and friend management in one ecosystem — so Romish.gg was designed from scratch to do exactly that.

---

## ⚙️ How It Works
1. Players log in via Steam (OAuth)
2. They queue up and fill a 10-slot pool
3. The system assigns captains and starts the draft
4. Captains alternate picks, then proceed to map veto
5. Match data is sent to DatHost API for automatic server setup
6. Players receive a connect button and join the server instantly
7. Results sync back into MongoDB and update ELO

---

