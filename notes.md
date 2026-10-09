# 📝 Quick Notes — Node.js & First React Project

## Node.js
- Node.js = JS ko browser ke bahar (terminal pe) chalane ka runtime
- Browser ka JS engine (Chrome = V8) ko Node computer pe le aata hai
- Ab `.js` file ko `node file.js` se run kar sakte ho — browser nahi chahiye
- React ke liye Node zaroori: project setup, npm packages, dev server sab Node pe chalte hain
- Node install 🔑 → `node -v` aur `npm -v` dono version dikhayein

## npm
- npm = Node Package Manager (libraries download + manage)
- `npm install` → package.json ke hisaab se saari dependencies node_modules me daal deta hai
- `npm run dev` → dev server start karta hai (localhost pe app chalta hai, save = auto refresh)
- `npm create vite@latest` → naya project banana

## Hello.js (Python/Java bridge)
- Variable: `const name = "Aisha";`  (Python: `name = "Aisha"`, Java: `String name = "Aisha";`)
- Print: `console.log(...)`  (Python: `print()`, Java: `System.out.println()`)
- String: `` `Hello ${name}` `` (Python ka f-string jaisa)
- Array: `const a = ["HTML","CSS","JS"];`  (Python list / Java String[] jaisa)
- Loop: `for (const x of a) { console.log(x); }`  ya  `a.forEach((x) => console.log(x));`
- Hamesha `===` use karo `==` nahi

## React — theory
- React = JavaScript library, UI banana (interactive, reusable, component-based)
- Component-based = har tukda alag component (Navbar, Card, Profile), reusable
- Declarative = hum UI "describe" karte hain, React khud DOM update karta hai
- Vanilla JS = hum manually DOM update karte hain (`getElementById...`) → zyada code, galtiyan
- Component = UI return karne wala function, naam Capital se shuru (`Profile`, `Card`)
- Props = component ko data pass karna (function ke arguments jaisa)

## Vite project setup (commands)
- `npm create vite@latest my-first-react-app` → React + JavaScript select karo
- `cd my-first-react-app`
- `npm install` → dependencies download (thoda time lagega)
- `npm run dev` → local server (localhost:5173)
- `Ctrl + C` → server band karne ke liye
- naye Vite pe optional sawaal ho sakta hai → install prompt par "No" kar do, phir khud `npm install`

## Folder structure (kaunsi file kya karti hai)
- `index.html` — ekmaatra HTML file, sirf `<div id="root"></div>` + script to main.jsx
- `src/main.jsx` — entry point, `#root` pe `<App />` render karta hai (React attach)
- `src/App.jsx` — root component, app ka main UI yahan likha jaata hai
- `src/Profile.jsx` — apna component (reusable)
- `src/index.css` — global styles (poori app pe)
- `src/App.css` — App component ke styles
- `src/assets/` — images/icons jo import karke use hote hain
- `public/` — static files (favicon, svg) bina process serve
- `package.json` — project ka ID card (name, scripts, dependencies)
- `package-lock.json` — exact dependency versions lock
- `vite.config.js` — Vite config
- `eslint.config.js` — code quality rules
- `.gitignore` — GitHub pe push nahi karne wali files ki list
- `node_modules/` — installed libraries, edit/mat push karo, delete → `npm install` se wapas
- Flow: `index.html → main.jsx → App.jsx → browser UI`

## JSX ke 4 rules
- `class` nahi, `className` use karo (React me `class` reserved hai)
- `{ }` ke andar JS chalta hai (variable, expression, sab)
- Ek component sirf ek parent return kare — do elements ke liye `<>...</>` (Fragment) ya `<div>` wrap karo
- Component naam **Capital letter** se shuru karo, warna React HTML tag samajh lega
- `useState` = React ka state (badalne wala data), `[val, setVal] = useState(0)`

## Common errors
- `npm: command not found` → Node install nahi hua, Node LTS + terminal restart
- `Cannot find module` → npm install nahi chalaya, project folder me `npm install`
- Blank page → browser console + terminal ke error padho
- "Adjacent JSX elements must be wrapped" → 2 elements wrap karo `<div>` ya `<>...</>`
- Component render nahi hota → naam capital letter se shuru karo

## Submission
- Folder: `task_01/`
- Files: `hello.js`, `my-first-react-app/` (node_modules ke **bina**), `Concepts.md`, `FolderStructure.md`
- ⚠️ `node_modules` push mat karo (`.gitignore` me hai) — `git status` se confirm karo
- GitHub link submit karo
