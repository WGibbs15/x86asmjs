# x86asm JS
Turns x86 code into a working example with a stack.

## Getting Started

Clone the repo and place the x86asm.js file in your project

##Prerequisites

You don't need anything else for this to work, but I would highly recommend downloading the necessary [highlight.js](https://highlightjs.org/download/) file and adding it to your project to make your x86 look nice
.
### Example

```
	<stack>
		<data>...,,,...,Garbage</data>
		<regs>eax: 0xa, ebx:, esp: 0x10000</regs>
		<pre><code>push eax
pop ebx</code></pre>
	</stack>
```

Make sure That everything is enclosed by the <stack> tag

The <data> tag should contain your comma separated initial stack values and size. The size is also automatically adjusted if your run out of room.

The <regs> tag is for your registers as well as their initial values. Make sure that the values for each register is separated by a colon even if there isn't a starting value.

The <pre><code> tags should contain your formatted assembly code. Make sure to add the addresses of the instructions as comments if you want the eip to function.

```
    push ebp              ;0x8048394
```

## Authors

**Wil Gibbs**
