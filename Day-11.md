Today’s Focus:
1.	Debouncing in JavaScript?
Debouncing is a programming technique that ensures a function is executed only after a certain period of inactivity. Imagine typing in a search bar where an API request is made on every keystroke. Without debouncing, every key press will trigger an API call wasting bandwidth and slowing performance.
With debouncing, the function runs only after the user stops typing for a given time.
When an event is triggered (like a keyup in a search box):
	A timer starts for a specified delay (e.g., 500ms).
	If another event occurs before the timer ends, the timer is reset.
	Only when there are no more events for that delay period, the function finally executes.

2.	What is Throttling?
Throttling ensures that a function is executed at most once in a specified time interval, no matter how many times an event occurs. Imagine a scroll event that triggers an animation or fetches data. If it runs on every scroll movement, it can execute hundreds of times per second hurting performance. With throttling, the function executes at fixed intervals (like every 1 second), regardless of how many scrolls occur.
When an event fires continuously:
	The function executes immediately (or after a short delay).
	Further calls within the defined time period are ignored.
	After the time period passes, the function can run again.

