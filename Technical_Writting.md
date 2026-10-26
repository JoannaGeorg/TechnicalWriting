# Technical Writing

## Parts of Speech

### Noun

A person, place, concept, or thing.

Eg. "In the **framework**, an **object** must copy any underlying **values** that the **object** wants to change. The **protocol buffers** in the **codebase** are huge, so copying the **protocol buffers** is unacceptably expensive."

In programming, classes and variables can be considered as the program's nouns.

### Pronouns

Pronouns are pointers to or substitutes for other nouns or sentences.

Eg. "The cafeteria featured peanut butter and plum jam on rye toast. Employees found **it** awesome and wished **they** could eat **this** every day."

### Verbs

A verbs is an action word or phrase. It is used to represnet the relationship between two nouns. Each sentence must contain atleast one verb.

Eg. "Samantha **is coding** Operation Bullwinkle in C++. This project currently **consumes** over 80,000 lines of code. She previously **used** Python, but recently **gravitated** to C++. Samantha **leads** a team of four software engineers, which **will grow** to six software engineers next quarter."

### Adjectives and Adverbs

Adjectives modify/describe nouns.

E.g. "Tom likes **red** balloons. He prepares **delicious** food. He fixed **eight** bugs at work."

Adverbs modify/decribe a verb. They acn also modify adjectives or other adverbs.

Eg. "Jane **efficiently** fixes bugs." annd "Jane fixes bugs  **efficiently**."

### Preposistions

Preposistions specify the relationship between two things.

They can refer to the place of the object such as "under", "next to", and "within".

They can refer to time with "before" and "after".

They can refer to the relationship between one object to another.

Eg. "Parameters may optionally appear **within** a URL, **after** the path."

### Conjuctions and Transitions

Conjuctions connect phrases or nouns within a sentence while transitions connect sentences themselves.

The most importtant and common conjections are:
  - And
  - But
  - Or

Eg. "Olivia writes great internal code **and** documentation **but** seldom works on open-source projects."

In technical writing the most important trasisitons are:
  - However
  - Therfore
  - For Example

Eg. Juan is a wonderful coder. **However**, he rarely writes sufficient tests. **For example**, Juan coded a 5,000 line FFT package that contained only a single 10-line unit test.

## Words

### Define New or Unfamiliar Terms

When writting or editing, recognize terms that might be unfamiliar to some or all of the terget audience.

If the term already exists, link to a good existing explanation.

If the term is being introduced, define the term.
  - If many terms are introduced in a document, collect the definations into a glossary.

### User Terms Conssitantly

Do not change the terms used, apply the same unambigous word consistenetly thorughout the document.

Example of renaming: "Protocol Buffers provide their own definition language ... And that's why protobufs have won so many county fairs."

The correct way of the above example would be applied as: "Protocol Buffers (or protobufs for short) provide their own definition language ... And that's why protobufs have won so many county fairs."

### Use Acronymns Properly

On the initial use of an infamiliar acronym within a document or a section, spell ou the full ther and then put the acronymn in parentheses.

Teh acronymn, then, can be used as is.

Eg. "This document is for engineers who are new to the Telekinetic Tactile Network (TTN) or need to understand how to order TTN replacement parts through finger motions."

Do not cycle back and forth between the full form and the acrpnym.

### Recognize Ambigous Pronouns

Consider the pronoun guidelines:
  - Only use a pronoun after the noun has been introduced, never before.
  - Place the pronoun as close to the referring noun.
    - If more than 5 words seperate the reffering noun from the pronoun, repat the noun instead of using a pronoun.
  - If a second noun is intoduced between the refernced noun and the pronoun, reuse thr noun instead.

## Active Voice vs Passive Voice

In an active voice the actor acts on a target.

`Active Voice = Actor + Verb + Target`

Eg. The cat sat on the mat.
  - Actor: cat
  - Verb: sat
  - Target: mat

A passive voice the target is the main focus.

`Passive Voice = Target + Verb + Actor`

Eg. The mat was sat on by the cat.
  - Actor: cat
  - Verb: sat
  - Target: mat

Some passive voice sentences can omit the actor altogether.

Eg. The mat was sat on.
  - Actor: *unknown*
  - Verb: sat
  - Target: mat

## Clear Sentences

### Choose Strong Verbs

Examples of weak and strong verb usage:
|Weak Verb|Strong Verb|
|---------|-----------|
|The exception **occurs** when dividing by zero|Dividing by zero **raises** the exception|
|This error message **happens** when ...|The system **generates** this error message when ...|
|We **are** very careful to ensure ... |We carefullt **ensure** ... |

Use different verbs to make the prose more interesting, ie, Sprinkle in different verbs to make the prose more apetizing.

### Reduce "There is" and "There are"

Sentences that start with "There is" or "There are" are very generic.

Often, just removing those phrases automaitically make the sentence more interesting.

Eg. 
Instead of "There is a variable called `met_trick` that stores the current accuracy."
Write: "A variable named `met_trick` stores the current accuracy."

Sometimes, moving the subject is better.

Othertimes, creating a subject to replace the phrase is more clear.

## Short Sentences

Generally, it is better to minimize the number of sentences:
  - Shorter documentation reads faster.
  - Shorter documentation is typically easier to maintain.
  - Extra line of documentation introduce additional points of failure.

### Focus Each Sentence on a Single Idea

The focus of each sentence must be on a single idea, thought, or concept.

Example of a sentence with multiple ideas:

"The late 1950s was a key era for programming languages because IBM introduced Fortran in 1957 and John McCarthy introduced Lisp the following year, which gave programmers both an iterative way of solving problems and a recursive way."

Ideal sentences:

"The late 1950s was a key era for programming languages. IBM introduced Fortran in 1957. John McCarthy invented Lisp the following year. Consequently, by the late 1950s, programmers could solve problems iteratively or recursively."

### Convert Some Long Sentences Into Lists

Example of a long sentence:

"To alter the usual flow of a loop, you may use either a break statement (which hops you out of the current loop) or a continue statement (which skips past the remainder of the current iteration of the current loop)."

Breaking it into a list:

"To alter the usual flow of a loop, call one of the following statements:
  - break, which hops you out of the current loop.
  - continue, which skips past the remainder of the current iteration of the current loop."

### Eliminate or Reduce Extraneous Words

Many sentences contain filler words.

Eg. "An input value greater than 100 **causes the triggering** of logging."

A better form of saying the same sentence is present.

Eg. "An input value greater than 100 **triggers** logging."