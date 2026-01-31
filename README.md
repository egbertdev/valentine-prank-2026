# 🌹 The "Unclickable" Valentine's Prank 🏃‍♂️💨

A high-stakes, chaotic Valentine's Day landing page where the "Yes" button has trust issues and the "No" button has a massive growth spurt. Built for maximum engagement and viral potential.

## 🚀 Live Demo
[View the Prank Live!](https://valentines-prank-2026.vercel.app) 

## ✨ Features
- **Evasive UI:** The "Yes" button uses real-time mouse/touch tracking to dodge the user with pinpoint accuracy.
- **Aggressive Scaling:** Every failed attempt to click "Yes" makes the "No" button grow exponentially, eventually consuming the viewport.
- **Dynamic Assets:** Featuring the legendary Ruto "Stressed" meme for peak cultural relevance and humor.
- **Lead Gen Integrated:** Subtle "Need a custom site?" CTA to convert viral traffic into professional inquiries.
- **Mobile Optimized:** Fully responsive and tested for the TikTok "POV" format.

## 🛠️ Tech Stack
- **Frontend:** HTML5 & Tailwind CSS (JIT Engine)
- **Logic:** Vanilla JavaScript (Event-driven DOM manipulation)
- **Deployment:** Vercel

## 📖 The "Sauce" (Technical Logic)
The core evasion logic utilizes a `mousemove` listener that calculates the button's bounding box. When the cursor enters the proximity threshold, the script triggers a new coordinate calculation within the safe zones of the window object.

```javascript
const moveButton = () => {
    // Calculates random coordinates within the visible viewport
    const x = Math.random() * (window.innerWidth - btnWidth);
    const y = Math.random() * (window.innerHeight - btnHeight);
    
    yesBtn.style.position = 'absolute';
    yesBtn.style.left = `${x}px`;
    yesBtn.style.top = `${y}px`;
};