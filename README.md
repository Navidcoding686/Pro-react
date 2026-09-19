Dev Stack Builder Website
A simple and interactive React application where users can explore available technology stacks and build their own stack by adding and removing technologies.

Technologies Used
React
TypeScript
Tailwind CSS
React Toastify
JSON data

Features
Browse Technology Stacks — Users can view different technology options.
Build Your Own Stack — Users can add technologies to their personal stack.
Remove Technologies — Users can remove technologies from their selected stack with a notification.

JSX is a syntax that lets us write HTML-like code inside JavaScript or TypeScript. It makes React components easier to write and understand.
Props are data passed from a parent component to a child component. State is data managed inside a component that can change over time.
useState stores and updates data inside a React component. I used it to manage the user's selected stack and update it when technologies are added or removed.
useEffect runs code after a component renders. I used it to load the technology data from the JSON file when the application starts.
React uses the key to identify each item in a list. A unique key helps React understand which items changed, were added, or were removed.

Conditional rendering means showing different UI depending on a condition.
I used it for the empty stack message:
{stack.length === 0 && <p>Your stack is empty.</p>}
The message is shown only when there are no technologies in the user's stack.

A parent passes data to a child through props. A child can send something back by calling a function that the parent passes as a prop. In this project, the parent passes stack data and functions to child components. The child can call the provided function to tell the parent that an item should be removed.
