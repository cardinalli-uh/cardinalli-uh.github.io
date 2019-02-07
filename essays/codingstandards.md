---
layout: essay
type: essay
image: 
title: Great Expectations
# All dates must be YYYY-MM-DD format!
date: 2019-02-06
labels:
  - Coding Standards
  - IDE Plugins
---



<h2>Unexpected Dickens</h2>
<blockquote>“That was a memorable day to me for it made great changes in me but it is the same with any life imagine one selected day struck out of it and think how different its course would have been pause you who read this and think for a moment of the long chain of iron or gold of thorns or flowers that would never have bound you but for the formation of the first link on one memorable day.” <footer> - Charles Dickens, <i>Great Expectations(edited from source)</i></footer></blockquote>

Despite this passage being written by the renowned Charles Dickens, it was probably a bit monotonous to read.  It was probably fairly confusing at times, too. And probably just not what anyone would expect of a world-famous author.  That's obviously because there is no punctuation though; which is because I edited the passage to remove all standardized punctuation.  The actual passage is entirely different, despite being the same, and reads:

<blockquote>“That was a memorable day to me, for it made great changes in me. But it is the same with any life. Imagine one selected day struck out of it, and think how different its course would have been. Pause you who read this, and think for a moment of the long chain of iron or gold, of thorns or flowers, that would never have bound you, but for the formation of the first link on one memorable day.” <footer> - Charles Dickens, <i>Great Expectations</i></footer></blockquote>

If you're like me, that second passage is at least a little bit more stirring.  It is a strange thing, how such a small difference can make such a profound change.  It's partly because punctuation grants a pace and tone to writing.  And also because, when used properly, punctuation helps to better convey the information and focus of text.  If used improperly, however, punctuation can cause a passage to become almost unreadable - and otherwise frustrating to read.  And any frustration would be forgivable.  Since that is - in large part - the point of punctuation standardization; that is, to eliminate frustration by keeping the written word in-line with expectations.  This isn't actually about punctuation at all though.  And it isn't about Dickens, nor even the English language.  It's about expectations, and how they apply to code. 


<h2>Coding as Expected</h2>
The need for punctuation exists in programming languages for the same reasons it exists in English; except, code is pretty much just punctuation marks and operators anyway.  So unlike in English, erroneous punctuation typically prevents code from compiling in the first place.  Therefore, the actual use of punctuation marks is typically well-specified within code. In software development, expectations regarding how code should be formatted are known as “coding standards,” which work for code a lot like punctuation works for English.  Here's a visualization which may convey this point better:

```javascript

//example 1:

const stooges = 
['Curly', 
'Larry', 
'Moe'];

function 
helloeverybody
(array) 
{for 
(let i = 0; 
i < array.length; 
i++) 
{console.log
("Hello " + array[i] + "!");}}

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

Note that the above code examples have identical content; it is only their formats that are different.  They both compile perfectly and return the desired results.  Nevertheless, and I think even someone who has never seen code would agree, the second example looks better.  Very much like good literature that has been improperly punctuated, code that doesn’t adhere to the basest expectations of coding standards can be near illegible.  Here, the second example conforms to general coding standards, whereas the first example merely works - similarly to how the second Dickens excerpt was compelling, whereas the first was merely coherent.  Like punctuation, these basic standards were developed for a reason.  Also like punctuation, coding standards can still be relatively loose.  That is to say, an author or coder may adapt a certain style of their own into their code; for instance, as you may have noticed, I use a lot of semi-colons in my writing.  In coding, as in English, some leeway is fine - assuming the more ubiquitous expectations are observed, and the format is consistent throughout the program.  Clarity is the key in either case.  As code goes, it may seem fine enough as long as the compiler can piece it together and function as desired; but not adhering to some type of standard - even just an internal one - will eventually be cause for confusion.  When coding, a program rarely comes together in the first try - debugging is a matter of course for a developer.  And it is while debugging and reviewing code that the benefits of coding standards really become evident.  Namely, it is a matter of readability.  Familiarity with a standard means knowing when and where to expect elements of code; in turn making it much simpler for any coder to spot potential errors or understand how code executes within a code-snippet.  This is an obvious advantage in terms of collaboration.  For instance, keeping code standardized helps the coder spot things like a missing curly-bracket, close-parenthesis, or semi-colon - and etcetera.  These are just minor type-errors; but they will prevent a code from compiling and potentially cause wasted time if the problem isn't located promptly.  

<h2>Expect the Expected</h2>
To help minimize those pesky type-errors, I have been coding using the IntelliJ IDE (Integrated Development Environment) with ESLint - an automatic code-standard inspection tool.  The advantage of tools like ESLint is that they inform the coder when their code is not up to the set standard.  The disadvantage is that becoming accustomed to one standard can make changing standards a bit tedious.  For instance, the coding standard I am using currently allows for significantly less ‘white’ space than previous coding standards I have used; and I often find myself removing blank lines before ESLint gives me the all-clear.  However, that blank lines are all I have to change is testament to another benefit of coding standards.  They ingrain a certain technique and help a coder immediately recognize their mistakes - thus, no need to wait for the compiler to realize any minor mistakes.  In that process, the coder is able to actively recognize their bad habits.  Despite their undeniable usefulness, even the best coding standards plugins can’t always do much for flawed math or logic; however, their ability to aid in the recognition of syntax errors frees up time for debugging more complicated problems.  In that way, ESLint and other coding standards plugins are fantastic utilities for increasing productivity, by keeping everything in line with expectations.

