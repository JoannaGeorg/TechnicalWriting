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

## Lists and Tables

Good lists can result in an orderly documentation.

### Choose the Correct Type of List

The different types of list are as follows:
  - *Bulleted Lists:* Used for unordered items, i.e., if the order of the listed items change the meaning of the list remains the same.
  - *Numbered Lists:* Used for Ordered items where a change in list items fundamentally changes the maining of the list.
  - *Embedded Lists:* Are list of items that are in a sentence. Ideally, the sentece should be converted into a bulleted or numbered list.

### Keep List Items Parrallel

All items in a parrallel list look like they belong together. They should match in:
  - Grammar
  - Logical Category
  - Capatilization
  - Punctuation

The first item in the list establishes the patter that a reader expects to see repeated.

### Start Numbered List Items with Imperitive words.

An imperative words is a command, such as *open* or *start*.

Eg. "How to:
  1. Download the Frambus app from Google Play or iTunes.
  2. Configure the Frambus app's settings.
  3. Start the Frambus app."

### Create Useful Tables

Consider the following guidelines:
  - Label each column with a meaningfull header.
  - Avoid putting too much text into a table cell. No more than two sentences.
  - Strive for parallelism within individual columns.

### Introduce Each List and Table

AKA, give the list or table context. Terminate the introductory statement witha colon rather than a period.

Use the word *"following"* in the introductory sentence.

## Paragraphs

### Write a Great Openeing Sentence.

The Opening sentence is the most important part of the pragraph. It is the focus and the rest of the content is structured around it.

A good opening sentence establishes the paragrph's central point.

Eg. "A loop runs the same block of code multiple times. For example, suppose you wrote a block of code that detected whether an input line ended with a period. To evaluate a million input lines, create a loop that runs a million times."

### Focus Each Paragrph on a Single Topic

A paragraph should represent an independant unit of logic. No description of a future or past topic.

### Don't Make Paragraphs Too Long or Short

Long Paragrphs are visually intimidating that readers may ignore.

Conversely, too short paragraphs makes for faulty organization.

### Answer What, Why, and How

Good paragraphs answer the following 3 questions:
  1. What is the content?
  2. Whay is it important to know?
  3. How should the knowledge be used? or How is the point true?

## Audience

`Good Documentation = knowledge and skills the audience needs to do a task - the sudience current knowledge and skills`

Thus, make sure that the document provides the information the audiences needs but dosen't already have.

### Define the Audience

Serious documentation efforts spend considerable time and energy on defing their audience. These efforts maight involve:
  - Surveys
  - User Experience Studies
  - Focus groups
  - Documentation testing.

Begin by identifying the audience role as they tend to share certain base skills and knowledge.

Eg. Most software engineers know the popular sorting algorithms and big O Notation. Thus, it is expected they already have this knowledge.

Consider thier proximity to the knowledge documented.

Eg. A heart sugeon knows more about the human ear than the average software engineer but not more than the average audiologist.

### Determine What the Audience Needs to Learn

List everything that the audience needs to know to learn. It can also include the tasks that they need to perform.

Also note the order of study for the tasks. What should be learnt before taskling the nest problem.

### Fit the Documentation to the Audience

Create Explanations that satisfy the audience's curiosity.

Match the vocabulary to the audience.

Use simple words over rare and complex words.

Keep the writting culturally neutral. Idiom's would not make sense to someone of different background like saying "Someone's looking a little green" means the same as "Someone's drinking vinegar". The difference is the background and language of the people using it.