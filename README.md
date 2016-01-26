# clean-code

In this repo you can find my notes for [Clean Code](http://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882/ref=sr_1_1?ie=UTF8&qid=1452837629&sr=8-1&keywords=clean+code) as I read through it. This is primarily to act as a learning tool and reference for me but I hope others will find it beneficial as well. Other repos that were trying to do this were not organized well and had either too much or too little information. Here I will list the handfull of notes I think most important for each section. 


## Sections

* [`Naming`](#naming)
* [`Functions`](#functions)
* [`Comments`](#comments)
* [`Formatting`](#formatting)

<a name="naming"></a>
### Naming
- Change names when you find better ones
- A name should tell you why something exists, what it does, and how it is used
- The length of a name should correspond to the size of its scope
- Pick one word per abstract concept and stick with it *(ex. `get`, `retrieve`, `fetch` are all equivalent so pick one)*
- The author is responsible for making his code clear
- Add prefixes as a last resort
- [View More](/naming.md)


<a name="functions"></a>
### Functions
- Keep very small (hopefully < ~10 lines)
- Do a single thing
- The "thing" a function is doing should include steps *one level of abstraction below* the name of the function
- Code should read like a top-down narrative. Each level of abstraction leads to the next.
- Long and descriptive function names are acceptable
- Keep function arguments between 0 and 3
- Keep functions pure (no side-effects!)
- Functions should *either do something or answer something, but not both*.
- Don't repeat yourself
- [View More](/functions.md)

<a name="comments"></a>
### Comments
- Comments are for compensating for our lack of ability to express ourselves in code
- Comments are hard to maintain, think hard before you add some
- *Inaccurate comments are far worse than no comments*
- *Don't leave commented out code.* Others will be confused and afraid to remove it.
- Connection between the code and it's comment should be obvious
- *Comments shouldn't need their own explanation*
- A good function name is usually better than a comment header
- [View More](/comments.md)

<a name="formatting"></a>
### Formatting
- Stick to a common set of style rules
- **Style and discipline survives even if your code doesn't**
- Try and keep files between 200 and 500 lines
- **Vertical Formatting** - High to low-level, separate groups of related lines by a blank line, tightly-related code should be vertically dense
- Caller functions should be above their callees (ideally). *This gives the program a natural flow.*
- Low-level functions should come last 
- Keep lines short (~120 characters)
- Use horizontal whitespace to associate strongly related things
- [View More](/formatting.md)
