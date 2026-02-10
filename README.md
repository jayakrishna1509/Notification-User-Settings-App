# 📋DAY 3 TASK: Notification & User Settings App

## 🎯Objective
Build a small app that practices:

• Portals

• Error Boundaries

• Controlled vs Uncontrolled Components

• useState

• useEffect

• useContext & Context API

## 🧩Requirements
### 1. Notification Modal (Using Portals):
• Create a Notification Modal that pops up outside the main root DOM node (using React Portals).

• It should have a simple "Close" button to dismiss it.

### 2. Error Boundary:
• Wrap parts of the app with an ErrorBoundary.

• If a specific component throws an error (simulate it with a button like "Crash App"), the boundary should catch it and show a friendly error message.

### 3. Controlled vs Uncontrolled Components:
• Create two forms:

o A Controlled Form: Inputs are controlled by React state (useState).

o An Uncontrolled Form: Use useRef to directly access input values.

### 4. State Management:
• Use useState to handle form inputs, modal open/close, etc.

### 5. Side Effects:
• Use useEffect to:

o Log a message when the modal opens.

o Auto-close the modal after 5 seconds.

### 6. Context API (useContext + Provider):
• Create a Theme Context:

o Theme options: "Light" and "Dark".

o Provide a toggle button to switch the theme.

o Use useContext in multiple components to apply the current theme style.

## Sample App Behaviour:
- [Show Notification Button] → (Opens a portal modal)
- Theme: [Light / Dark Toggle]
- [Form - Controlled] (Inputs binded with state)
- [Form - Uncontrolled] (Inputs accessed via refs)
- [Crash App Button] → (Triggers an error and shows fallback UI from ErrorBoundary)

```
Theme Toggle Button

| Show Notification Button |

(Notification Modal appears on top when open)

| Controlled Form |

Name: [] Email: [] [Submit]

| Uncontrolled Form |

Username: [] Password: [] [Submit]

| Crash App Button |

(Shows ErrorBoundary fallback UI if crashed)
```

## 🎁Bonus (Optional)
• Animate the notification modal (fade in/out).

• Save the selected theme in localStorage using useEffect.

• Provide a "Retry" button inside ErrorBoundary to reset the crashed part.