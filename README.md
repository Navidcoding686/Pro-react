<h2>Dev Stack Builder Website</h2>
<p>A simple and interactive React application where users can explore available technology stacks and build their own stack by adding and removing technologies.</p>

<h2>Technologies Used</h2>
<li>
React
TypeScript
Tailwind CSS
React Toastify
JSON data
</li>

<h2>Features</h2>
<li>
<p>Browse Technology Stacks — Users can view different technology options.</p>
<p>Build Your Own Stack — Users can add technologies to their personal stack.</p>
<p>Remove Technologies — Users can remove technologies from their selected stack with a notification.</p>
</li>

<h2>JSX</h2>
<p>JSX is a syntax that lets us write HTML-like code inside JavaScript or TypeScript. It makes React components easier to write and understand.</p>

<h2>Props and State</h2>
<p>Props are data passed from a parent component to a child component. State is data managed inside a component that can change over time.</p>

<h2>useState</h2>
<p>useState stores and updates data inside a React component. I used it to manage the user's selected stack and update it when technologies are added or removed.</p>

<h2>useEffect</h2>
<p>useEffect runs code after a component renders. I used it to load the technology data from the JSON file when the application starts.</p>

<h2>React key prop in .map()</h2>
<p>React uses the key to identify each item in a list. A unique key helps React understand which items changed, were added, or were removed.</p>

<h2> Conditional Rendering</h2>
<p>Conditional rendering means showing different UI depending on a condition.
I used it for the empty stack message:<br>
selectedStack.length === 0 ? <p> Your stack is empty. </p> : selectedStack.map((item) =>.....<br>
The message is shown only when there are no technologies in the user's stack otherwise it maps an array using key. </p>

<h2>Passing data between child and component</h2>
<p>A parent passes data to a child through props. A child can send something back by calling a function that the parent passes as a prop. In this project, the parent passes stack data and functions to child components. The child can call the provided function to tell the parent that an item should be removed.</p>
