
Today’s Focus:
1.	What is the Document Object Model (DOM)?
DOM is like map of webpage that computer can understand and mutates. It represents the structure of a webpage as a tree of objects, where each element (like <div>, <h1>, <p>, etc.) is a node in that tree. JavaScript can use the DOM to read, modify, add, or delete elements and attributes dynamically making web pages interactive and dynamic.

2.	Selecting, Adding, and Removing Elements in the DOM?
Selecting Elements: 
	By ID - document.getElementById('heading')
	By Class Name - document.getElementsByClassName('item')
	By Tag Name - document.getElementsByTagName('p')
	Query Selector - document.querySelector('.item') or document.querySelectorAll('.item')

Adding Elements:
	const list = document.querySelector('ul');
const newItem = document.createElement('li');
newItem.textContent = "New List Item";
list.appendChild(newItem);
Removing Elements:
	Direct remove - para.remove();
	Remove child from parent - list.removeChild(item);
	Replace an Element - old.replaceWith(newEl);
			
3.	What is Event Propagation?
When an event (like a click) happens on an element, it doesn’t just affect that element it travels through the DOM tree. This process is called event propagation. There are 3 phases Capturing Phase, Target Phase, Bubbling Phase.

4.	Explain 3 phases?
1.	Capturing Phase (Event Capturing - Top → Target) - The event starts from the root (document) and travels down to the target element.
2.	Target Phase - Event reaches the actual element clicked - The target element is the one where the event actually occurred.
3.	Bubbling Phase (Event Bubbling - Target → Top) - After the event reaches the target, it bubbles up back through its ancestors.

5.	What is Event Delegation?
Event Delegation is a technique where you add a single event listener to a parent element instead of adding separate listeners to each child element. When a child element is clicked the event bubbles up to the parent and the parent can detect which child triggered it using “event.target”.


