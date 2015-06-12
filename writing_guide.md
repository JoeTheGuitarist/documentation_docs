# How to Write a User's Guide

## Introduction

Welcome to mbed's not-as-short-as-expected writing guide. This guide should help you write your own user documentation. 

It covers:

* General writing tips.

* Mapping your document for writing and reading.

* Fleshing out your map. 

* How to explain things so that people understand.

* How to give examples.

* How to edit yourself.

And a few other topics.

For advice about publishing your documentation, see [the publishing guide](/publishing_guide/).
Our style guide is for internal use only. To community members we recommend [the Guardian](http://www.theguardian.com/guardian-observer-style-guide-a) and [the Economist](http://www.economist.com/styleguide/introduction) for British English and the [Chicago Manual of Style](http://www.chicagomanualofstyle.org/16/contents) for American English.

## General Writing Tips

* Don’t use more words than you need - some poor soul has to read them all.

* You get no extra credit for using long or obscure words - use little ol’ English.

* Don’t let your sentences run away from you - keep them short and simple.

* If you have a sense of humour - use it. In a pinch, [link](http://xkcd.com/1348/) [to](http://xkcd.com/195/) [xkcd](http://xkcd.com/386/).

## Document Maps - Writing v Reading

Here is an important distinction: where you start writing and where the user starts reading are not the same place. The user will start at the beginning. You will not. This means you'll need to know:

1. [What your'e going to write](#The-Writing-Map).

2. How to put it together to be read.

We'll create a map, list, coggle or interpretive dance routine for each before we start working. If we just improvise as we go along we'll get lost, forget things, double-up and generally take three times as long as we need to.

### The Writing Map

Before you start writing you should know what you'll need to cover. If you just improvise as you go along you'll forget things. So make a map:

1. You start at the most important point. It's like marking the X, then drawing the treasure map around it. With software, this will normally be all available features and their options, for example all of the options of a command-line tool.

2. Now list what you need to install your tool - including all dependencies. 

3. Think of all the technical background required to understand steps 1 and 2.

4. Steps 1 to 3 have mapped out all of the technical ground you need to cover. Start fleshing it out bit by bit.

5. Think of some examples showing how to use your tool and some of its best features.

6. If there's additional material you want, like FAQs and a problem solving section, now's the time to outline them. 

7. Finally, write an introduction. This should explain what your tool does and why I should bother using it. If you're writing for a new version of the tool, you'll address version differences either in the introduction or in the section after the introduction.


### The Reading Map

When you're done writing, please don't forget to put the text in reading order. For example, it makes very little sense to give a full explanation of all commands before bothering to explain what the general purpose of the tool is. A general guideline:

1. The introduction.

2. The version highlights, if you wrote them.

3. The installation instructions (start with a list of dependencies). 

4. How to use the tool, feature by feature, with the technical background each one requires. Please think carefully about the order of features.

5. Examples can be stand-alone, or you can mix them in with the previous step by giving an example for each feature.

6. Additional materials.

## How to Flesh Out - the Plan

Now you have a map of features and their sub-functions or options. Assuming it's not enough (don't assume - for some things it may well do), how do you turn that map into a text? You measure every feature on your list against a checklist.

### Checklists

Every feature your tool offers (probably) has the following:

1. A purpose.

2. A mechanism.

3. Options and sub-functions.

4. One or more results.

5. One or more failure scenarios and ways of handling them.

You can flesh things out by going over each item in your list and checking it off as you explain it. For some items, you'll have to do quite a bit of writing (this is why you listed all sub-functions earlier - so that you don't forget any now).

You may have noticed by now that I'm a huge fan of working to a list. You should list every section's content before you start writing it. If you think of something as you write, add it to the list rather than divert yourself by writing it (or forgetting about it). So, for example, make a list of failure scenarios, and a list of solutions for each one. Then write into that list.

You'll sometimes find that you want to mix things up a bit, like putting failure scenarios with the sub-functions that generate them. This isn't necessarily a bad idea, but it isn't necessarily a good one, either. If you mix things up too much you create something that's hard to follow. Pulp Fiction isn't a good outline for a user's guide.

### Organising the Features for Reading

Please think carefully about the order if which you present features. There are two considerations here, and they often conflict:

1. You can't start people off at the most complex features. The basis of Hello World is that we start people at the simple things and then work our way up. 

2. It's instinctive to start people off at the most interesting bits: the most useful features or the features we want to show off the most. 

Sometimes the most interesting features are quite simple and it's a win-win. Sometimes they're very complex and require a lot of knowledge that the reader might not have; by deciding to start off with these you'll create either a very complicated - even exhausting - guide, or one that leaves out most of the information the reader needs.

This is a balancing act, but if you look at programming guides you'll notice that they go for gradual build of complexity rather than being useful right off the bat. This means they're boring as all hell to start with, so many developers shy away from writing that way. But it's a good model to keep in mind when you write.

### Scalability

The nice thing about this method is that it's equally valid for all sizes of text. Sometimes you'll find that the map is enough (you'll just have to put it in reading order and add a short introduction), sometimes you'll find that it takes pages and pages to explain every single feature. Either way, you follow the same method from start to finish. 

It's also valid for different kinds of text, although it might at times lack elegance. So even if you're explaining a general concept like debugging, security or connectivity, you can think of every concept you're trying to get across as a feature or tool and work from there.

How do you know how detailed your docs should be? Some of it is gut feeling, some of it is common sense (it's a fine line between the two). Either way: write it out, give it to someone, and ask them if they understood and managed to follow it and use the tool. If they didn't, it was either too short or too messy (or both). There is a third option, but then it's your fault for picking that person as your doc's tester, so either way you learned a lesson.

## How to Flesh Out - Explaining Things

You can start [here](http://arkinwriting.com/2014/02/21/dont-dumb-it-down-layer-it-up-writing-tips-for-engineers/).

### Connecting the Dots

There is one thing I keep seeing in developers’ writing: all the dots, without a single line to connect them. You need to do three things: list your ideas, put them in a readable order, and specify whether they are linked by causation, contrast or continuation. So don’t write “A, B, C, D, E” (and certainly not "E, C, A2, A3, B, A1, D"). Write “A and B, therefore C. Oh, and D, therefore not E”.

There are two easy ways of spotting the dots:

* The Why/So What method: my name for the Inductive Order approach. This is similar to the way Sherlock Holmes speaks: give a conclusion, then the facts proving it, one by one. You do this by asking yourself is “what’s the bottom line”, then “why”. Keep asking “why” until you’ve reached the basic concepts we all agree on. Invert that list, and you have a fully structured argument. Then ask “so what” so that you remember to do something with all the information you just gave me - like connect it to the next dot.

* The Need/Meet method: everything is either something you need or a way to meet that need (I’m sorry if I sound like Ayn Rand). If you pair these out, you’ll end up understanding what everything in the story does.

Then there are several ways of organising the dots:

* Inductive order: you used this earlier to spot dots. Now you can use it to organise them. How handy!

* Increasing difficulty: start at the basics and move on. This works equally well in a single paragraph and in a full-fledged book. The Why/So What method builds this for you per dot, and sometimes even connects dots for you.

* Problem and solution: this matches the need/meet method which provides a list of problems. You'll just have to put them in a logical order. What "logical" means changes depending on what you're writing.

* Inverted pyramid: the way a newspaper article works. You start with a summary of the whole idea, and then you give out the facts in descending order of importance.

Don’t mix and match ideas, explaining bits and pieces of each in a random order; explain one thing fully, then explain another thing fully, then tie them together. It’s very easy to follow a zigzag pattern when you already know the conclusion, but your reader will have to deconstruct it and put the ideas in order for you.

Last, please remember to clearly link the dots: causation, contrast or continuation.

### Guessing at Prior Knowledge

How much prior knowledge can you assume when writing? The easiest way to figure it out is to pretend you’re writing a chapter for a book. Where in the book will your chapter come? If it’s the very first chapter, you can’t assume any prior knowledge. If it’s in the middle, everything that would have come before can be assumed to be prior knowledge. 

Of course, guessing how much your readers know is the easy bit (I mean, it's a guess - it's going to be wrong). Sticking to it when you write is much harder. Developers tend not to understand how little an agreed readership actually knows (if they knew this much, they wouldn't be reading), how unintuitive some of their intuitive leaps are, and how dense some of their "simple introductions" are. When writing, it's better to aim lower; readers can skim and skip much more easily than they can fill in the gaps.

### Technobabble

Look, you deal with hardware, so maybe you'll find a good reason to reverse the polarity of the neutron flow. But until you do, please could you speak English?

You have to notice when you’re throwing out odd bits of vocabulary as if they’re common knowledge. Some may very well be; others will not. Usually the problem is that within the context of a sentence, you don’t stop and think about all of the words you’re using and how many of them don't make sense to anyone who doesn't already know the material. You certainly don't think about the possibility that a google search will bring 100 irrelevant results, so at least do google it for the reader.

On first use, give the meaning of initials, then the initials in parentheses. For example, it’s Bluetooth Low Energy (BLE), not BLE (Bluetooth Low Energy). Don’t bother doing this with things that are more commonly known by their initials, like BBC. You can put the full term in italics if you like: Bluetooth Low Energy (BLE).

### Writing an Instruction

If you're giving a one-step instruction, you just write "x to y". So:

> "Select Compile > Update Docs to regenerate the program documentation".

If you have more than one step, start with the expected result, then the steps as a numbered list. So it's:

> "To create a new program:

> 1. Select New > New Program to open the Create New Program window.

> 2. Another action.

> 3. You get the point."

When giving keyboard shortcuts:

* Use “press” for a physical button or key (like the power button on the boards, or keyboard keys).

* Give the short form with a capital letter: Del, Cmd.

* If more than one key is required, use + without spaces: Ctrl+Alt+Del.

When talking about on-screen buttons:

* Use “click” for something in a GUI (like the compile button).

* If the button has a name (written on it) you can refer to it directly (with the capital letter, and you can also use bold font if you want): “click Compile”. But if there’s just an icon, it’s best to use a few more words: “click the search button” (no capital, and using an article, because there’s no name for the button).

Fun fact (it's not a fact, just a preference): we use bullets if a list can come in any order and numbers if the list can only come in the order in which it's presented. Instructions will therefore tend to be numbered.

It's better to tell people what they should do, not what they shouldn't do. If you're worried about damage to hardware: add a warning, then be as negative as you want. Note that warnings are not a step in the instructions; they're a formatted paragraph before all steps or before the relevant step. The formatting should stand out from the list, but not be too jarring.

### Screen Caps

Go [here](http://arkinwriting.com/2014/02/26/screen-cap-tips-for-beginners/).

## Giving Examples

Our basic assumption is that readers should be able to perform the examples themselves, so we should provide a full process, not just a pretty result. From this assumption we reach the following wild conclusions:

* Don't start in the middle or skip steps; if they were obvious, we wouldn't be writing a guide to begin with. For example, it might make sense to you that your command-line tool requires you navigate to the relevant directory, but some users assume tools are global and will have a "work with this directory command". So tell me that you opened the CMD and navigated to a particular directory.

* Tell me how you do everything, not just that you did it. What command did you use? How did you reach it?

* Tell me why you do everything. Why is this the next step? Why did you choose that particular sub-option?

* Tell me about things like long processing times (or I'll think I did something wrong) and questions I'll need to answer (and what each possible answer means).

* Don't dump some new tool on me at step 17. Tell me before you start the example what I'll need to complete it myself.

* If you find that you're giving me a lot of background information in one of the steps, it probably means your original explanation omitted too much.

* Don't cover too much material in any example. Show one or two big things, and another couple of small things. Move on to a fresh example to show other things.

* A single step should include only one sequential action, or all simultaneous actions. Do not group sequential actions or separate simultaneous actions.

* Don't forget the screen caps.


## Additional Material

Additional material can be problem solving, FAQ, links to other resources and anything that you couldn't shove into the main body of the text. You don't have to include it, but if you do it's important you don't treat it as a catch-all; you should put stuff within the main body if at all possible, resorting to the additional material section only for things that cannot possibly fit anywhere else. 

FAQs are often a repetition of the main body. In a sense they're highlights, rather than new information. That's fine. They're also often a dumping ground for things you don't want to say in the main body because you're mildly embarrassed. That, too, is fine.

## Writing an Introduction

An introduction has two main jobs: tell me what your tool does, and tell me why I should use it (instead of some other tool). To do its job, an introduction will usually cover:

1. What the tool is supposed to do.

2. How it manages to do it.

3. Perhaps a couple of features, to highlight the awesome capabilities of your tool.

4. Sometimes version differences (see next section).

## Version Differences

If this isn't the first version of the tool, it's polite to highlight the differences between the current version and the previous one:

* If it's only a couple of new things, put them in the introduction.

* If there are many differences, put them in their own section right after the introduction. 

Wherever you put the differences, it's helpful to readers if you flag them with "what's new in version x" or something similar. Readers who are already familiar with your tool are fishing for the version differences, they don't need the full guide.

## Cross Referencing

It's helpful to cross reference - with links. Do note that the information in your document should be introduced in the order in which a reader is expected to learn it; readers shouldn't have to jump between sections to put the story together. Cross-references should therefore link back (to things the reader is expected to have read already), not forward. However, there are times when forward referencing is correct:


* In an introduction, where it allows people to skip to the interesting bits (it functions like a table of contents).

* When you're telling people "if x then you can skip to y", giving knowledgeable readers a handy bypass of the beginners' stuff.

* When saying "this is all you need for now, but we'll go further into this at a later section". Here the purpose of the reference is to allow curious readers to see ahead, not to provide essential information.

* If you're sending readers to an appendix.

* If you're pointing to a figure in the next page.

A couple of notes:

* Don't say "below" or "above" or anything like that unless you're one paragraph away from where you're pointing to. You're making the user guess, and anyway you may reorder the text. Give the name of the section and a link. 

* It's good to introduce (at least as a list) all the sections of a guide in the introduction. Link to them.

## Editing Yourself

This is one of the hardest things you have to do in writing. Editing yourself requires spotting your own mistakes, but since you know what you meant to say it's hard to realise you didn't actually say it. 

### Editing a Complete Text


Some tips:

* Read very slowly. This will help you spot typos that you gloss over when you're reading quickly. It will also help you get a feel for how your text reads to slower readers (like many non-native readers).

* Focus on order: did you put the information (even within a single paragraph) as A to Z, or do you go from C to B via R without passing through A? And did you make the relationship between the different bits clear?

* Try to spot leaps of knowledge. Where did you require more information than the reader is assumed to have? Where did you think a connection between two concepts you introduced is intuitive? It isn't.

* Try to spot ambiguous sentences. You're writing in English, so you should be able to find plenty of them. But it's hard work to find them in your own writing, since you know what the sentence should mean so you'll not fall for the ambiguity. You have to force yourself to check if your word choice, or word order, can give the sentence two meanings that are not clarified by the context.

### Editing as You Write

It's the same as editing when you're done, only less effective. In general, the longer the break between writing and editing, the better the edit.

### Backwards Editing

Anyone who writes a long document without ever going back and revising what he has already written is not paying attention. But - try to make a note of it and get back to it later, not when you think about it, because you'll lose the thread that made you think about it in the first place. 

The above paragraph, by the way, is a good example of how *not* to explain things.

## Examples (Good and Bad)

Example time! Some of these are from this guide, some from the BLE Intros.

### Example One

> "Introductions (to the document or sections in the document) are the only places that can link ahead, unless you're specifically telling people "you can skip this if…". Everything else should only link to something that came before it (and that the user is therefore expected to have read). Otherwise, it's likely that you're telling readers that information that's essential to understand now is explained at a later point in the document. This is a good hint that your document is not organised logically. Do not make the readers jump around."

This text is quite messy. The main point is near the end, the thing you shouldn't do is in the middle and the thing you're allowed to do is at the beginning but its wording is confused. There is no clear context to this text (even when you put it under the heading of "cross-referencing"), and because everything was mixed it wasn't clear that the exceptions to the rule are missing. This is somewhat better:

> "The information in your document should be introduced in the order in which a reader is expected to learn it; readers shouldn't have to jump between sections to put the story together. Cross-references should therefore link back (to things the reader is expected to have read already), not forward. However, there are times when forward referencing is correct:

> 1. In an introduction, where it allows people to skip to the interesting bits (it functions like a table of contents).

> 2. When you're telling people "if you're already familiar with x, skip to y", giving knowledgeable readers a handy bypass of the beginners' stuff.

> 3. When saying "this is all you need for now, but we'll go further into this at a later section". Here the purpose of the reference is to allow curious readers to see ahead, not to provide essential information.

> 4. If you're sending readers to an appendix.

> 5. If you're pointing to a figure in the next page."

### Example Two

> "There are two ways to treat names of functions, APIs etc: as proper nouns or as common nouns. I tend to go with treating them as proper nouns, because a proper noun is one that names a specific thing, and it doesn’t get more specific than BLE_API, does it? So we “use BLE_API”, not “use the BLE_API” (but you can say “we use the BLE API, not the WiFi API”, and you’ll note the missing underscore - we’re not using the real names here).

>Note that you can use proper nouns as common nouns. For example, if you’re using a function in a sentence, you can use just its name: “call waitForEvent()”, but if you’re reminding people that it’s a function, you need to use an article “call **the** waitForEvent() **function**”."

This is, again, a mess. Why isn't the rule fully explained before an example is given?

> "Quick flashback to school (stop screaming, it will be over soon!): there are two kinds of nouns, proper and common. A **proper** noun points to a unique thing, and it therefore takes no article (unless the article is part of the name, like the Rolling Stones). A **common** noun, on the other hand, points to a class or a non-specific instance of a class, and therefore takes an article. 

> When you're referring to APIs, functions, services and so on, the structure of the sentence is how you'll know if they're proper or common nouns. "We use BLE_API" - this is a specific API. It's a proper noun, and therefore takes no article. "We use the BLE, not WiFi, API" - you're talking about two kinds of API, and the focus is on the API. The two kinds - BLE and WiFi - are treated as common nouns, and they take the article "the". You'll note that we didn't use their proper names (BLE_API has an underscore, "the BLE API" doesn't).

> The difference is more obvious in the following two sentences: "we call waitForEvent()" and "we call the waitForEvent() function". The reason you needed the article "the" in the second sentence is that you used the word "function", rather than just the name of a specific function."

This is now much longer, but it's actually covering only the ground covered by the original example - it just does it with all the details that the original example glossed over.

### Example Three

> "Before saying what the program should do (the function), we tell it when to do it. We've created a WHILE loop that will keep going so long as the condition it's checking returns the value TRUE. For the function to stop running, then, the condition it's checking will have to become false."

This is from an intro to non-developers, so I should explain what loops and conditions are before explaining how a loop uses a condition:

> "Before saying what the program should do (the function), we tell it when to do it. We use two tools to determine this: 

> * A condition that determines when to start the function, for example "when you get a new value from the thermometer". 

> * A definition of how many times to run when the starting condition is met. We can tell a function to run once, twice, to infinity or until the condition suddenly fails.

> In this example, we use the same condition to determine both when to start running and when to stop. To do this:

> * We created a WHILE loop, which is a way of saying "start this function when a condition is met, and don't stop until the condition is false". 

> * We said that the condition is that the value of ``triggerSensorPolling`` is TRUE rather than FALSE. That value is determined inside the loop. 

> If the value of ``triggerSensorPolling`` becomes FALSE, the condition will fail and the function won't run any more. This is called "exiting the loop"."

### Example Four

> "Usually, _Handle Value Notifications/Indications_ are used by the server to send updated values to a subscribed client or for signalling a client that a subscribed read attribute has been updated. Because _Handle Value Notifications_ can carry the same payload as any other BLE message, is sent at the server’s discretion, and doesn't generate a response from the client, _Handle Value Notifications_ can be repurposed for transmitting low latency data from server to client."

This is the edited version:

> "Usually, the server uses ``_Handle Value Notifications/Indications_``  to send updated values to a subscribed client, or for signalling a client that a subscribed read attribute has been updated. But we can repurpose ``_Handle Value Notifications_`` for transmitting low latency data from the server to the client because ``_Handle Value Notifications_``:

> * Can carry the same payload as any other BLE message.

> * Is sent at the server’s discretion.

> * Doesn't generate a response from the client."

The two main changes are a move from passive to active voice, and bullet points instead of a long sentence. You'll also note that I moved the result ("we can repurpose…") ahead of the cause ("because it..."). This is an easier structure to follow.

## Writer's Blocks Aren't Just for Fiction Writers

Got writer's block? Trying to edit yourself but keep reverting back to the original? Not to worry - generations of writers have successfully dealt with these same issues with little more than these helpful tips (and alcohol, consumption and criminal behaviour):

* Look away from the text for a while - work on something else, take a walk, make a cup of tea.

* Put bits of your text through Google Translate a few times. It should give you an interesting view of it (and a good giggle).

* Move to a different part of the text. 

* Try explaining it out loud to someone. They don't actually have to pay attention.

* Listen to a song you like for its lyrics.

* Spit it out, no matter how bad it is. You can edit later. Note: I don't approve of this method, because I think a first draft stays with you forever; it influences all future edits, no matter how bad it is.

## A Final Word of Warning
Do not leave your own notes in the text when you publish it, especially if you tend to be less than entirely polite when talking to yourself (and your collaborators). Always preface them with the same bit of text, like TBD or WTF, and do a search on it before publishing.
