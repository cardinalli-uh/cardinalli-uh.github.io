---
layout: essay
type: essay
image: 
title: Coding Standards
# All dates must be YYYY-MM-DD format!
date: 2019-02-06
labels:
  - Coding Standards
  - IDE Plugins
---




<blockquote>“some birds are not meant to be caged that's all their feathers are too bright their songs too sweet and wild so you let them go or when you open the cage to feed them they somehow fly out past you and the part of you that knows it was wrong to imprison them in the first place rejoices but still the place where you live is that much more drab and empty for their departure.” <footer> Stephen King, <i>Different Seasons</i></footer></blockquote>

Despite it being written by a famous writer, the above passage was probably a bit painful to read.  The reason should be obvious - there is no punctuation; that is, I rewrote the passage without adhering to the English standards of punctuation.  The actual passage reads:

<blockquote>“Some birds are not meant to be caged, that’s all. Their feathers are too bright, their songs too sweet and wild. So you let them go, or when you open the cage to feed them they somehow fly out past you. And the part of you that knows it was wrong to imprison them in the first place rejoices, but still, the place where you live is that much more drab and empty for their departure.” <footer> Stephen King, <i>Different Seasons</i></footer></blockquote>

Considering the given passage, it should be clear why punctuation is required by the English language.  Punctuation allows for increased clarity.  What may be less clear, is why that need is echoed by programming languages.  This visualization might help:

```javascript

//this is an example of code with poor standards

const stooges = ['Curly', 
'Larry', 
'Moe'];
function helloeverybody(stooges) { for (let i = 0; i < array.length; i++) {
console.log("Hello " + array[i] + "!");}}
```

```javascript

//this is an example of code with good standards

const stooges = ['Curly', 'Larry', 'Moe'];

function helloEverybody(stooges) {
    for (let i = 0; i < array.length; i++) {
        console.log("Hello " + array[i] + "!");
    }
}
```

<h2></h2>
Guidelines, or rules that dictate how code should be formatted are known as “coding standards.”  Similar to good literature that has been improperly punctuated, code that doesn’t adhere to basic coding standards can be near illegible; however, like punctuation, coding standards can be relatively loose.  That is to say, an author or coder may adapt a certain style of their own.  As code goes, it may seem fine enough as long as the compiler can piece it together and function appropriately; but not adhering to some type of standard - even just an internal one - will eventually be cause for confusion.  When coding, a program rarely comes together in the first try - debugging is a matter of course for a coder.  And it is while debugging and reviewing code that the benefits of coding standards really become evident.  Namely, it is a matter of readability.  Familiarity with a standard means knowing when and where code elements should be; in turn making it much simpler for any coder to spot potential errors or understand how code executes within a code-snippet.

<h2></h2>
Over the past week I have been coding using the IntelliJ IDE (Integrated Development Environment) with ESLint - an automatic code-standard inspection tool.  The advantage of tools like ESLint is that they inform the coder when their code is not up to the set standard.  The disadvantage is that becoming accustomed to one standard can make changing standards a bit tedious.  For instance, the coding standard I am using currently allows for significantly less ‘white’ space than previous coding standards I have used; and I often find myself removing blank lines before ESLint gives me the all-clear.  However, that blank lines are all I have to change is testament to the other benefit of coding standards.  They ingrain a certain technique and help a coder immediately recognize their mistakes - thus, no need to wait for the compiler to realize any minor mistakes.  In that process, the coder is able to actively recognize their bad habits.  Despite their usefulness, even the best coding standards can’t do always do much for flawed math or logic; but their ability to aid in the recognition of syntax errors frees up time for debugging more complicated problems.  In that way, ESLint and other coding standards plugins are fantastic utilities for increasing productivity.

