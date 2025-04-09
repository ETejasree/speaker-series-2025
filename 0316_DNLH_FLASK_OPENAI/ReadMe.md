# 📢 DOT NET LEARNERS HOUSE  Meetup – Monthly Event - Mar 2025

## Date Time: 16-MAR-2025 at 09:00 AM IST

## Event URL:https://www.meetup.com/dot-net-learners-house-hyderabad/events/304750920
## YouTube URL:https://www.youtube.com/watch?v=rrZqYt2YDFM

![Information | 100x100](./Documentation/Images/Information.PNG)

![Seat Belt | 100x100](./Documentation/Images/SeatBelt.PNG)




## *🎯 Goal of the Session:*  
By the end of this session, attendees will:  
✅ Set up a *React + Tailwind CSS* project.  
✅ Build a *fully responsive chat UI*.  
✅ Ensure the UI follows a *modern, clean design* with Tailwind.  

---

## *📝 Demo Script:*

### *1️⃣ Introduction (2 min)*
"Hi everyone! Now that our backend is up and running, it's time to focus on the *frontend* — specifically, building a modern chat UI using *React and Tailwind CSS*.  
By the end of this session, you'll see a clean, responsive interface, and in the next one, *Sowmya* will hook it up to the Flask backend."


---
# the System Architecture
![System Architecture | 100x100](./Documentation/Images/SystemArchitecture.jpg)


Welcome to our AI integration journey! In this session, we'll shift our focus to the **frontend** and build a clean, responsive **chat UI** using **React + Tailwind CSS**.

---

### 2️⃣ Setting Up the Project (4 min)

1. **Create a new React + TypeScript app with Vite:**

```bash
npm create vite@latest flask-react-aoai-ui --template react-ts
cd flask-react-aoai-ui
npm install
```

2. **Install Tailwind CSS and dependencies:**

```bash
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

3. **Configure `tailwind.config.js`:**

```js
export default {
  content: ["./index.html", "./src/**/*.{js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};
```

4. **Import Tailwind in `src/index.css`:**

```css
@import 'tailwindcss/base';
@import 'tailwindcss/components';
@import 'tailwindcss/utilities';
```

> ✅ Now you're ready to start building your UI!

---

### 3️⃣ Building the Chat UI (6 min)

Create a new file: `src/components/Chat.tsx`

```tsx
import { useState } from "react";

const Chat: React.FC = () => {
  const [prompt, setPrompt] = useState<string>("");

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

      <button
        className="bg-blue-600 text-white px-6 py-2 rounded-lg hover:bg-blue-700 transition"
      >
        🚀 Send
      </button>
    </div>
  );
};

export default Chat;
```

> 🎨 This gives us a modern, minimal UI, ready for AI responses!

---

### 4️⃣ Run and Test the App (3 min)

Start the development server:

```bash
npm run dev
```
---
### 5️⃣ Wrap-up & Next Steps (1 min)

- Recap:
  > “We've now built a fully functional and responsive chat UI using React and Tailwind CSS.”

---

## 🧠 Key Takeaways

- **React + Vite** offers a fast development environment.
- **Tailwind CSS** enables rapid UI development with utility-first styling.
- You've built a solid UI foundation ready for API integration.

---

## 🙌 Thank You!

Feel free to fork this repo, explore more with Tailwind, and continue building!
