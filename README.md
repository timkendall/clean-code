# clean-code

In this repo you can find my notes for [Clean Code](http://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882/ref=sr_1_1?ie=UTF8&qid=1452837629&sr=8-1&keywords=clean+code) as I read through it. This is primarily to act as a learning tool and reference for me but I hope others will find it beneficial as well. Other repos that were trying to do this were not organized well and had either too much or too little information. Here I will keep everything in a single file and stick to concise bullet points. 


## Sections

* [`Naming`](#naming)

<a name="naming"></a>
### Naming

- Change names when you find better ones
- A name should tell you why something exists, what it does, and how it is used
- Avoid disinformation  *(ex. don't name something `personList` if it is not a `List`)*
- Avoid similarly shaped names for dissimilar concepts
- Don't name things to satisfy a compiler or interpreter (if possible)
- Avoid meanigless distinctions *(ex. `ProductInfo` vs `ProductData` both mean the same thing but look different)
- Use pronounceable names
- **The length of a name should correspond to the size of its scope**
- Avoid mental mapping
- Methods should have verb names *(ex. `createPayment()`)*
- Acessors, mutators, and predicates should be prefixed with `get`, `set`, and `is`
- Don't be cute (i.e don't use slang or colloquialisms)
- *Pick one word per abstract concept and stick with it *(ex. `get`, `retrieve`, `fetch` are all equivalent so pick one)*
- Consistent lexicon == good
- The author is responsible for making his code clear
- Prefer drawing names from the solution domain (i.e Computer Science). This way developers don't have to be domain experts to know what something means.
- When there is no technical (i.e solution domain) term for something, borrow from the problem domain. Code that has more to do with the problem domain should have names drawn from there anyways.
- Few names are meaningful in and of themeselves - make sure you place names in context by enclosing them in well-named classes, functions, or namespaces
- *Add prefixes as a last resort*
- Shorter names are generally better than longer ones - add no more context to a name than is necessary 
- Choosing good names requires good descriptive skills and a shared cultural background
