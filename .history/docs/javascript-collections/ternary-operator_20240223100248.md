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
  const [user, setUser] = useState("Iqmal");

  function changeUser() {
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
