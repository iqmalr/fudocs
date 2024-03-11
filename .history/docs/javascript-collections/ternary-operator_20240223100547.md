---
sidebar_position: 2
---

# Ternary Operations

In programming, "ternary" refers to the "ternary" operator, also known as the conditional operator. This operator provides a concise way to write conditional expressions. The general form of the "ternary" operator is:

```jsx title=".jsx"
condition ? expressionIfTrue : expressionIfFalse;
```

This means that if the condition is `true`, the first expression (`expressionIfTrue`) will be evaluated; if the condition is `false`, the second expression (`expressionIfFalse`) will be evaluated.

Here's an example of using the ternary operator in JavaScript/React:

```jsx live
function Ternary() {
  // State variable to track the current user
  const [user, setUser] = useState("Iqmal");
  // Function to change the user's name using a ternary operator
  function changeUser() {
    // Toggle between 'Iqmal' and 'Riffai' based on the current user
    setUser((prevUser) => (prevUser === "Iqmal" ? "Riffai" : "Iqmal"));
  }

  return (
    <>
      <h1>{user}</h1>
      <button onClick={changeUser}>changename</button>
    </>
  );
}
```

The `changeUser` function utilizes the ternary operator to toggle between the usernames 'Iqmal' and 'Riffai'. Here's a breakdown of the code:

- The component uses the `useState` hook to manage the user `state`, initially set to "Iqmal".
- The `changeUser` function is triggered when the button is clicked. It utilizes the `setUser` function with a callback to update - the user `state` based on the current value (`prevUser`). If `prevUser` is "Iqmal", it changes to "Riffai"; otherwise, it changes to "Iqmal".
- The JSX renders the current username (`user`) within an <h1> element, and a button labeled "Change Name" triggers the `changeUser` function when clicked.
  In summary, this component showcases the use of the ternary operator to dynamically change the displayed username based on the current `state`. When the button is clicked, the username alternates between "Iqmal" and "Riffai".
