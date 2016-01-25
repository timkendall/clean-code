# clean-code

In this repo you can find my notes for [Clean Code](http://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882/ref=sr_1_1?ie=UTF8&qid=1452837629&sr=8-1&keywords=clean+code) as I read through it. This is primarily to act as a learning tool and reference for me but I hope others will find it beneficial as well. Other repos that were trying to do this were not organized well and had either too much or too little information. Here I will keep everything in a single file and stick to concise bullet points. 


## Sections

* [`Naming`](#naming)
* [`Functions`](#functions)

<a name="naming"></a>
### Naming

- Change names when you find better ones
- A name should tell you why something exists, what it does, and how it is used
- Avoid disinformation  *(ex. don't name something `personList` if it is not a `List`)*
- Avoid similarly shaped names for dissimilar concepts
- Don't name things to satisfy a compiler or interpreter (if possible)
- Avoid meaningless distinctions *(ex. `ProductInfo` vs `ProductData` both mean the same thing but look different)
- Use pronounceable names
- **The length of a name should correspond to the size of its scope**
- Avoid mental mapping
- Methods should have verb names *(ex. `createPayment()`)*
- Accessors, mutators, and predicates should be prefixed with `get`, `set`, and `is`
- Don't be cute (i.e don't use slang or colloquialisms)
- *Pick one word per abstract concept and stick with it *(ex. `get`, `retrieve`, `fetch` are all equivalent so pick one)*
- Consistent lexicon == good
- The author is responsible for making his code clear
- Prefer drawing names from the solution domain (i.e Computer Science). This way developers don't have to be domain experts to know what something means.
- When there is no technical (i.e solution domain) term for something, borrow from the problem domain. Code that has more to do with the problem domain should have names drawn from there anyways.
- Few names are meaningful in and of themselves - make sure you place names in context by enclosing them in well-named classes, functions, or namespaces
- *Add prefixes as a last resort*
- Shorter names are generally better than longer ones - add no more context to a name than is necessary 
- Choosing good names requires good descriptive skills and a shared cultural background


<a name="functions"></a>
### Functions
- **Keep very small (hopefully < ~10 lines)**
- A function should lead you to the next function in a compelling order
- Extract conditionals to functions (ex. `isLoading()`). This increases readability and helps keep functions small
- **Do a single thing**
- The "thing" a function is doing should include steps *one level of abstraction below* the name of the function
- Statements within a function should be on the same level of abstraction. For example, `getUser` and `parseInt(45)` are not on the same levels of abstraction. Using different levels of abstraction in a single function creates confusion for the reader. Is a particular expression an essential concept or a detail? It's hard to know when mixing levels of abstraction.
- Code should read like a top-down narrative. Each level of abstraction leads to the next.
- Switch statements should be buried in a low-level class and not repeated.
- Long and descriptive function names are acceptable
- Choosing function names may take time. **Don't be afraid to try multiple names** (find and replace is trivial).
- **Keep function arguments between 0 and 3**
- Think hard about using three arguments.
- **Keep functions pure (no side-effects!)**
- Don't use flag arguments. This immediately indicates that the function is doing more than one thing. You should split the function up instead.
- Reduce the number of arguments by creating objects instead (ex. `makeCircle(Point: center, int: radius)`)
- Be careful of dyads (2 arguments). Many arguments don't have a natural ordering and can easily cause confusion as to which comes first (ex. `assertEqual(expected, actual)`).
- Arguments are inputs to functions, don't manipulate them
- Functions should **either do something or answer something, but not both**.
- Prefer exceptions over returning error codes. Returning error codes forces the developer to handle that code immediately (ex. `if (deleteUser() === OK)` and mixes command and query. Exceptions allow error handling to be separated cleanly from the "happy path". 
- **Don't repeat yourself**
- No one starts by writing a perfect function. Usually the first version is a long mess that takes effort to cleanup and break into separate components - just like writing.
- Systems are stories to be told rather than programs to be written.
