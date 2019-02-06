---
layout: essay
type: essay
image: 
title: coding standards title
# All dates must be YYYY-MM-DD format!
date: 2019-02-06
labels:
  - Coding Standards
  - IDE Plugins
---



<h2>p1 title</h2>
<blockquote>“some birds are not meant to be caged thats all their feathers are too bright their songs too sweet and wild so you let them go or when you open the cage to feed them they somehow fly out past you and the part of you that knows it was wrong to imprison them in the first place rejoices but still the place where you live is that much more drab and empty for their departure.” <footer> - Stephen King, <i>Different Seasons (edited from source)</i></footer></blockquote>

Despite it being a famous passage written by a renowned author, the above passage probably read a bit monotonously.  That's because there is no punctuation.  Because I edited the passage to remove all standardized punctuation.  The actual passage is entirely different, despite being the same, and reads:

<blockquote>“Some birds are not meant to be caged, that’s all. Their feathers are too bright, their songs too sweet and wild. So you let them go, or when you open the cage to feed them they somehow fly out past you. And the part of you that knows it was wrong to imprison them in the first place rejoices, but still, the place where you live is that much more drab and empty for their departure.” <footer> - Stephen King, <i>Different Seasons</i></footer></blockquote>

Considering the given passage, it should be clear why punctuation is important in the English language.  Punctuation grants a pace and tone to writing, along with increasing clarity by cutting ambiguity.  Used properly, punctuation helps to better convey the information within the text.  Used improperly, punctuation may cause a passage to become completely unreadable.  What may be less clear, is why that need is echoed by programming languages.  This visualization might help:

```javascript

//example 1:

const stooges 
= ['Curly', 
'Larry', 
'Moe'];
function 
helloeverybody
(array) 
{ for (let i = 0; 
i < array.length; 
i++) 
{console.log("Hello " 
+ array[i] + "!");}}

console.log(helloeverybody(stooges));
```

```javascript

//example 2:

const stooges = ['Curly', 'Larry', 'Moe'];

function helloEverybody(array) {
    for (let i = 0; i < array.length; i++) {
        console.log("Hello " + array[i] + "!");
    }
}
console.log(helloEverybody(stooges));

```

<h2>p2 title</h2>
Guidelines, or rules, that dictate how code should be formatted are known as “coding standards.”  Note that the above code examples have identical content; only their formats are different.  They both compile perfectly and return the desired results.  Still, the second example is much easier on the eyes.  Very much like good literature that has been improperly punctuated, code that doesn’t adhere to basic coding standards can be near illegible; however, like punctuation, coding standards can still be relatively loose.  That is to say, an author or coder may adapt a certain style of their own into their code.  This should be fine as long as the more ubiquitous standards are observed, and the format is consistent throughout the program.  As code goes, it may seem fine enough as long as the compiler can piece it together and function appropriately; but not adhering to some type of standard - even just an internal one - will eventually be cause for confusion.  When coding, a program rarely comes together in the first try - debugging is a matter of course for a developer.  And it is while debugging and reviewing code that the benefits of coding standards really become evident.  Namely, it is a matter of readability.  Familiarity with a standard means knowing when and where code elements should be; in turn making it much simpler for any coder to spot potential errors or understand how code executes within a code-snippet.  This is an obvious advantage in terms of collaboration.  Keeping code standardized also helps the coder spot things like a missing curly bracket, close-parenthesis, and etcetera.  These are just minor type-errors; but they will prevent a code from compiling and potentially cause wasted time if the problem isn't located promptly.

<h2>p3 title</h2>
To help minimize those pesky type-errors, over the past week I have been coding using the IntelliJ IDE (Integrated Development Environment) with ESLint - an automatic code-standard inspection tool.  The advantage of tools like ESLint is that they inform the coder when their code is not up to the set standard.  The disadvantage is that becoming accustomed to one standard can make changing standards a bit tedious.  For instance, the coding standard I am using currently allows for significantly less ‘white’ space than previous coding standards I have used; and I often find myself removing blank lines before ESLint gives me the all-clear.  However, that blank lines are all I have to change is testament to another benefit of coding standards.  They ingrain a certain technique and help a coder immediately recognize their mistakes - thus, no need to wait for the compiler to realize any minor mistakes.  In that process, the coder is able to actively recognize their bad habits.  Despite their usefulness, even the best coding standards can’t do always do much for flawed math or logic; however, their ability to aid in the recognition of syntax errors frees up time for debugging more complicated problems.  In that way, ESLint and other coding standards plugins are fantastic utilities for increasing productivity.

