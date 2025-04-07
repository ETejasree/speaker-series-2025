# 📢 GLOBAL AI HYDERABAD - 2025

## Date Time: 12-apr-2025 at 09:00 AM IST

## Event URL:

![Information | 100x100](./Documentation/Images/Information.PNG)

![Seat Belt | 100x100](./Documentation/Images/SeatBelt.PNG)




## *🎯 Goal of the Session:*  
By the end of this session, attendees will:  
✅ Set up a *React + Tailwind CSS* project.  
✅ Build a *fully responsive chat UI*.  
✅ Ensure the UI follows a *modern, clean design* with Tailwind.  

---

## *📝 Demo Script:*

### *1️⃣ Introduction (1 min)*
"Hi everyone! Now that our backend is up and running, it's time to focus on the *frontend* — specifically, building a modern chat UI using *React and Tailwind CSS*.  
By the end of this session, you'll see a clean, responsive interface, and in the next one, *Sowmya* will hook it up to the Flask backend."


---
# the System Architecture
![System Architecture | 100x100](./Documentation/Images/SystemArchitecture.jpg)


## **⚙️ Project Setup (~2 min)**

**1. Create the React project using Vite:**
```bash
npm create vite@latest flask-react-aoai-ui --template react-ts
cd flask-react-aoai-ui
npm install
```

**2. Install and configure Tailwind CSS:**
```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

**Update `tailwind.config.js`:**
```js
export default {
  content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
  theme: { extend: {} },
};
```

**Import Tailwind in `index.css`:**
```css
@import 'tailwindcss/base';
@import 'tailwindcss/components';
@import 'tailwindcss/utilities';
```

"That’s it — we’re ready to build our chat UI!"

---

## **💬 Building the Chat UI (~4 min)**

**Create `Chat.tsx`:**
```tsx
import { useState } from "react";

const Chat: React.FC = () => {
  const [prompt, setPrompt] = useState("");

  return (
    <div className="p-6 w-full max-w-2xl mx-auto space-y-4 font-inter">
      <h2 className="text-2xl font-semibold text-gray-800">Chat with AI 🤖</h2>

      <div className="bg-gray-700 text-white p-4 rounded-lg border-l-4 border-blue-500 min-h-[100px] flex items-center justify-center">
        <p className="text-base font-light">Your response will appear here</p>
      </div>

      <textarea
        className="w-full p-3 border rounded-lg shadow-md focus:ring focus:ring-blue-300"
        placeholder="Type your question..."
        value={prompt}
        onChange={(e) => setPrompt(e.target.value)}
      />

      <button className="bg-blue-600 text-white px-6 py-2 rounded-lg hover:bg-blue-700 transition">
        🚀 Send
      </button>
    </div>
  );
};

export default Chat;
```

"This component gives us a simple, clean layout with a prompt box, a response area, and a button — styled entirely using Tailwind."

---

## **🚀 Running & Testing (~1 min)**

To launch the app:
```bash
npm run dev
```

"You’ll now see a polished UI — all that’s left is to hook it up with Flask, which *Sowmya* will cover next."

---

## **🎯 Wrap-up (~30 sec)**

"Today, we built a fully responsive and styled chat UI using React and Tailwind.  
Next time, we’ll connect it to our backend for real-time interaction.  
Thanks for joining!"

---

Let me know if you want this as a slide outline or a printable handout!