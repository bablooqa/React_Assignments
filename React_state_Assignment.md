
Use TypeScript where possible, but you may create `.jsx` versions if needed. [web:1]

---

## 🧩 Section 1: State Management Basics (Q1–Q8)

### Q1. Counter Component – `Counter.tsx`
Create a simple counter with **Increment** and **Decrement** buttons.  
- Use `useState` to store the count.  
- Display the current count on the screen. [web:2]

---

### Q2. Toggle Switch – `ToggleSwitch.tsx`
Build a toggle that switches between `ON` and `OFF`.  
- Use boolean state.  
- Change text and basic styling depending on the state. [web:2]

---

### Q3. Text Input Display – `TextDisplay.tsx`
Create an input that displays the current value below it in real time.  
- Use `onChange` event and `useState`. [web:2]

---

### Q4. Color Picker – `ColorPicker.tsx`
Create 5 buttons (red, blue, green, yellow, purple).  
- On click, change a box’s background color.  
- Store the selected color in state. [web:2]

---

### Q5. List Manager – `ListManager.tsx`
Create an input and an **Add** button.  
- Add text as items in a list.  
- Show all items in an unordered list. [web:2]

---

### Q6. Character Counter – `CharacterCounter.tsx`
Input field with live character count.  
- Show count while typing.  
- Show a warning if length > 100. [web:2]

---

### Q7. Multi-State Dashboard – `UserDashboard.tsx`
Manage multiple pieces of state:  
- `username: string`  
- `age: number`  
- `isActive: boolean`  
Render inputs to update each and show all values. [web:2]

---

### Q8. Shopping Cart Counter – `ProductCard.tsx`
Create a product card with:  
- Quantity `+` / `-` buttons (no negative values)  
- Fixed unit price  
- Display `totalPrice = quantity × unitPrice`. [web:2]

---

## 🖱️ Section 2: Event Handling (Q9–Q14)

### Q9. Mouse Position Tracker – `MouseTracker.tsx`
Track mouse position over a specific div.  
- Show `x` and `y` coordinates on the screen using mouse events. [web:1]

---

### Q10. Keyboard Event Handler – `KeyboardListener.tsx`
Listen for key presses.  
- Show last pressed key, key code, and whether Shift/Ctrl/Alt was pressed. [web:1]

---

### Q11. Double Click Counter – `DoubleClickCounter.tsx`
Increment a counter only on **double click**, not on single click.  
- Use `onDoubleClick`. [web:2]

---

### Q12. Form Submit Handler – `LoginForm.tsx`
Simple login form with `email` and `password`.  
- On submit, prevent default.  
- Show entered values in an alert or on screen. [web:6]

---

### Q13. Dropdown Menu – `DropdownMenu.tsx`
Button that toggles a dropdown.  
- Open/close on button click.  
- Close when clicking outside (use event listener on document). [web:1]

---

### Q14. Drag and Drop Box – `DraggableBox.tsx`
Create a draggable box.  
- Use mouse events to move the box within a container. [web:1]

---

## ⚙️ Section 3: React Hooks (Q15–Q22)

### Q15. `useEffect` Data Fetch – `UserProfile.tsx`
Fetch a single user on mount:  
- API: `https://jsonplaceholder.typicode.com/users/1`  
- Use `useEffect` + `fetch` and display name, email, and address. [web:1]

---

### Q16. `useEffect` Cleanup – `Timer.tsx`
Create a timer that counts seconds from 0.  
- Use `setInterval` in `useEffect`.  
- Clear the interval on unmount. [web:2]

---

### Q17. `useRef` Focus Management – `FocusManager.tsx`
Form with multiple inputs and a **Focus First** button.  
- On click, focus the first input using `useRef`. [web:2]

---

### Q18. `useRef` Previous Value – `PreviousValueTracker.tsx`
Input field that shows:  
- Current value  
- Previous value (using `useRef`) [web:1]

---

### Q19. `useMemo` Expensive Calculation – `FactorialCalculator.tsx`
Number input with factorial display.  
- Use `useMemo` to memoize factorial calculation. [web:2]

---

### Q20. `useCallback` Optimized Child – `ParentChild.tsx`
Parent component with counter and a child that receives a callback.  
- Use `useCallback` to prevent child re-renders (verify via `console.log`). [web:8]

---

### Q21. Custom Hook – `useLocalStorage.ts` + `ThemeToggle.tsx`
Create a custom hook `useLocalStorage(key, initialValue)` that syncs state with `localStorage`.  
- Use it in `ThemeToggle.tsx` to persist light/dark theme. [web:5]

---

### Q22. Custom Hook – `useFetch.ts` + `PostsList.tsx`
Create `useFetch<T>(url)` custom hook that returns:  
- `data`  
- `loading`  
- `error`  
Use it in `PostsList.tsx` to fetch and display posts. [web:5]

---

## ✅ Section 4: Form Validation (Q23–Q30)

You can implement validation manually or use patterns inspired by libraries like Zod / React Hook Form, but do not rely on them directly for this assignment. [web:6]

### Q23. Email Validator – `EmailValidator.tsx`
Single email input.  
- Validate format with regex on blur.  
- Show error message for invalid email. [web:6]

---

### Q24. Password Strength Checker – `PasswordStrength.tsx`
Password input with live strength indicator.  
- Requirements:  
  - Min 8 characters  
  - At least 1 uppercase  
  - At least 1 number  
  - At least 1 special character  
- Show strength as Weak / Medium / Strong. [web:6]

---

### Q25. Registration Form – `RegistrationForm.tsx`
Fields: `username`, `email`, `password`, `confirmPassword`.  
- `username`: 3–25 chars  
- `email`: valid format  
- `password`: follow rules from Q24  
- `confirmPassword`: must match password  
Display error messages per field. [web:6]

---

### Q26. Number Range Validator – `RangeValidator.tsx`
Numeric input that only allows values between 1–100.  
- Show error if value is out of range or not a number. [web:6]

---

### Q27. Required Fields Form – `ContactForm.tsx`
Contact form with `name`, `email`, `message`.  
- All required  
- Disable submit button until all fields are valid and non-empty. [web:6]

---

### Q28. Credit Card Formatter – `CreditCardInput.tsx`
Input that formats card number as `xxxx xxxx xxxx xxxx`.  
- Only numbers  
- Auto-insert spaces  
- Show error if total digits ≠ 16. [web:6]

---

### Q29. Multi-Step Form – `MultiStepForm.tsx`
3 steps:  
1. Personal Info  
2. Contact Info  
3. Review & Submit  

- Validate each step before allowing navigation to the next.  
- Show progress and final summary. [web:6]

---

### Q30. Dynamic Form with Types – `DynamicForm.tsx` + `formTypes.ts`
Create a dynamic form generator:  
- Define `FieldConfig` type in `formTypes.ts` with:  
  - `name`  
  - `label`  
  - `type` (`"text" | "email" | "number" | "password" | "textarea"` etc.)  
  - `validation` rules (e.g., required, minLength, maxLength)  
- `DynamicForm` takes an array of configs and renders inputs dynamically.  
- Perform validation based on config. [web:6]

---

## 🧪 Evaluation Criteria

- **Functionality (40%)**  
  All components work as described, including state updates, event handling, hooks, and validation flows. [web:1]

- **Code Quality (25%)**  
  Clean structure, meaningful naming, reusable components, and minimal duplication. [web:1]

- **TypeScript Usage (15%)**  
  Proper interfaces/types for props, state, and custom hooks where used. [web:1]

- **Best Practices (20%)**  
  - Follow the Rules of Hooks  
  - Keep components small and focused  
  - Avoid unnecessary re-renders using memoization where appropriate [web:2][web:8]

---

## ▶️ Getting Started

- Initialize app (example): `npm create vite@latest` or `npx create-react-app` with TypeScript template. [web:1]  
- Install dependencies and start dev server:  

