## 🔐 **Captcha Validator**

---

### 🧠 Goal

Build a React component that displays a 5-letter **random uppercase captcha**, lets users type it, and validates it on submission.

---

### ✅ Features to Implement

1. **Captcha Generation**

   * On load, generate a random 5-letter **uppercase** captcha (like `ABZPQ`)
   * Display it using a styled `div` or `canvas`
   * Use `data-testid="captcha-canvas"` for testing

2. **User Input**

   * Provide an input field with placeholder: `"Enter Captcha"`

3. **Buttons**

   * **🔁 Refresh Button**

     * Regenerates a new captcha and clears the input
   * **Submit Button**

     * Validates the entered input against the displayed captcha (case-sensitive)

4. **Result Feedback**

   * If correct: ✅ `Captcha Verified`
   * If incorrect or empty: ❌ `Incorrect Captcha`

---

### 🔎 Constraints (Used in Test Cases)

| Element        | Constraint                     |
| -------------- | ------------------------------ |
| Captcha Box    | `data-testid="captcha-canvas"` |
| Input Field    | Has class `captcha-input`      |
| Submit Button  | Has class `submit-btn`         |
| Refresh Button | Has class `refresh-btn`        |

---

### 🧪 Test Coverage

| **Test Case** | **What to Validate**                         |
| ------------- | -------------------------------------------- |
| TC1           | Captcha box and form render correctly        |
| TC2           | Refresh regenerates captcha and clears input |
| TC3           | Correct input shows “Captcha Verified”       |
| TC4           | Wrong input shows “Incorrect Captcha”        |
| TC5           | Empty input shows “Incorrect Captcha”        |
| TC6           | Buttons and input have correct CSS classes   |
| TC7           | Layout is responsive on different screens    |

---

### 💡 Hints

* Think about how to generate a random string of 5 uppercase letters using JavaScript.
* Consider using the `<canvas>` API or a styled `<div>` to visually show the captcha.
* Ensure that captcha comparison is case-sensitive when validating.
* Don’t forget to clear the input field when the captcha is refreshed.


