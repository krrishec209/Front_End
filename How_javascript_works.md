You write 5 lines of JavaScript. Your computer does a whole lot more. 😅

Alex writes:

console.log("Start");
setTimeout(() => {
  console.log("Hello");
}, 1000);
console.log("End");

Alex expects:

Start → Hello → End

JavaScript says:

Start → End → Hello 💀

Why?

Because JavaScript isn’t simply “running your code line by line.”

There’s an entire runtime working behind the scenes.

🧠 The basic flow

1️⃣ JavaScript Engine

The engine parses your code, optimizes it with techniques such as JIT compilation, and executes it.

2️⃣ Web APIs

Things like timers, network requests, and DOM events can be handled outside the main JavaScript execution path.

3️⃣ Callback / task queues

When asynchronous work finishes, callbacks can be queued for execution.

4️⃣ Event Loop

The event loop coordinates when queued callbacks get a chance to run.

That’s why this:

console.log("Start");
setTimeout(() => console.log("Hello"), 1000);
console.log("End");

prints:

Start
End
Hello

And JavaScript has more interesting characteristics:

→ Functions are first-class values
→ Types are dynamic
→ Objects use prototypes for inheritance
→ Memory is managed through garbage collection
→ Async programming enables non-blocking workflows

So the next time someone says:

“JavaScript is just a scripting language.”

Remember:

The syntax may look simple.

The runtime underneath is doing a lot of work. ⚙️

<img width="800" height="835" alt="image" src="https://github.com/user-attachments/assets/7f5525e1-0cb6-46bc-907e-95ce258a74aa" />

https://lnkd.in/p/dxm9cJvi


