# About the Style Guide

A style guide is a collection of fussy complaints about the way people write. It exists because, [in this description of reality, I am the pragmatist](http://www.smbc-comics.com/index.php?id=3761). It covers some vocabulary, grammar, punctuation and style choices that are either good or bad (mostly bad). It is by no means a full guide to the English language, but it should help you think about how you use it and avoid some of the more common mistakes.

Just so that you know I'm not making it up: our style guide is heavily influenced by [the Guardian](http://www.theguardian.com/guardian-observer-style-guide-a) and [the Economist](http://www.economist.com/styleguide/introduction). If you want to read those instead of this one, you're very welcome to. They're more comprehensive and accurate, and much funnier. It is further boosted by [Grammar Girl](http://www.quickanddirtytips.com/grammar-girl), [xkcd](https://xkcd.com/) and [the Oatmeal](http://theoatmeal.com/). 

The style guide has two parts:

1. [General English tips](#english).

2. [mbed-specific tips](#mbed).

The trick with a style guide isn’t to remember the right way of using all of these, it’s to remember that you need to look it up.

# About Writing

This is not a full writing guide. It doesn’t tell you how to write a full text, but where to put a comma and exactly where the rules of Latin grammar belong (spoiler: in Latin texts. There, now you don’t need to read the rest of this). However, since you’re not writers, I’ve written a few words to get you on your way:

* Don’t use more words than you need - some poor soul has to read them all.

* You get no extra credit for using long or obscure words - use little ol’ English.

* Don’t let your sentences run away from you - keep them short and simple.

* If you have a sense of humour - use it. In a pinch, [link](http://xkcd.com/1348/) [to](http://xkcd.com/195/) [xkcd](http://xkcd.com/386/).

If you want more information about writing, see our [writing guide](writing_guide.md). It deals with things like writing examples and instructions, ordering your text and self-editing.

______

<a name="english">
# English
</a>

Brilliant language, I love it. But it’s completely bonkers.

## Learning from Our Betters

If you’re not sure, follow this emergency procedure:

1. Ask [the Guardian](http://www.theguardian.com/guardian-observer-style-guide-a).

2. If that doesn’t work, ask [the Economist](http://www.economist.com/styleguide/introduction).

3. Note that when those two disagree we follow the Guardian, unless we like the Economist’s advice better.

4. When all else fails, ask Google. Try to remain with fairly recent sources; you don’t want Advice from the Period of English when all Nouns got a Capital.

## A Word About American v British English

ARM uses the [Chicago Manual of Style](http://www.chicagomanualofstyle.org/16/contents) and [Merriam-Webster's Collegiate Dictionary](http://www.merriam-webster.com/). Both of these are in American English (or International English, which follows the American spelling). But mbed's style guide is in British English (it's based on the Economist and Guardian). Why?

Well, it's not because I'm a snob. It's because I don't expect developers to learn to spell in a particular system just to write a little readme file. I did a quick headcount (I didn't really) and concluded that the Cambridge office is the biggest. So by popular vote, we're going with British spelling.

However, I also don't intend to waste time on hunting down American English (it's better armed, anyway). So if you're American, or if you've learned American English, you can make a rude noise and ignore me when I say that the verb ending is "-se".

## Spelling

* Put all your text into something that can check your spelling. Do not trust yourself.

* Do not trust the spellchecker.

* Okay, that was a bit unfair. If you’re not sure you’ve got the correct spelling, you can do two things: google the spelling you have and see what the dictionary says, or google both forms (“x or y?”) and see if anyone explains the difference. If the only difference is that one is British and one is American, use whichever one you’re used to (if you’re not used to either, please use British).

* Do not use all-caps unless that is the legal form of a name (so it's ARM, not Arm).

## Grammar (and Similar Considerations)

* Feel free to ignore Latin grammar that’s been shoved down English’s throat (to boldly split where no infinitive was split before, as they say).

* The rule that you can’t use a noun as a verb is only here to give snobs something to snob about (see what I did there?). Of course you can - an estimated 20% of English verbs are nouns doing double-duty.

* Don't use &, /, # and so on. There's enough room for the words and you don't know how someone might understand the symbol. Remember the lesson of "I don't have a key called Any". Besides, it’s ugly and I hate it - and I edit your texts.

* I distinguish “which” and “that”, though some might say it’s fussy of me. “Which” comes after a comma, and denotes a non-essential bit of information (from the point of view of the sentence, not the universe). “That” comes without a comma and the information following it should be vital to the sentence.

* Double negatives are not grammatically wrong, but they’re often very confusing. This isn’t because people can’t read, it’s because double negatives are used differently in different languages and English dialects - they can either cancel each other out or intensify each other - and you have an international audience; best to stick to single negatives or develop a positive mindset. Good luck with that.

* For the a/an before H or abbreviations issue, I'll just [quote the Guardian](http://www.theguardian.com/guardian-observer-style-guide-a): "Use an before a silent H: an heir, an hour, an honest politician, an honorary consul; use a before an aspirated H: a hero, a hotel, a historian (but don't change a direct quote if the speaker says, for example, "an historic"). With abbreviations, be guided by pronunciation: eg an LSE student." This is one of the many ways in which it's impossible to learn English until you know English.

* It's OK to talk to the reader: "you can select your..." etc. Never use the third person; you'll sound like a creepy lawyer.

* You can use “we” instead of “you”, if you like. “We” is seen as friendlier, as if you’re going through this with the reader, rather than watching from the sidelines.

* Try to use positive rather than negative sentences. Users (even when they’re reading) expect positive actions (“do x”, not “don't do y”) and might work based on that expectation (without bothering to read the whole sentence, of course).

* Use active rather than passive constructions. "You can x", not "x can be". But use the passive when:

	* The active sounds like it's shouting at the reader.

	* There is no specific entity performing the action, so you don't have a pronoun around which to construct an active sentence.

	* If there's no way to control something, it's better to use the passive voice rather than mislead the reader. For example, don't create an illusion that something is under the user's control when it's actually hardcoded.

* When texts are related (such as bulleted lists), try to make them very similar, so that the differences stand out; this helps readers scan the text and pick out the differences, rather than read the whole text. If part of the text of all options is identical, it should be moved to the section label, rather than be used again and again in every option.

* I don’t have many pet peeves, but the “and/or” construction drives me nuts (using just / drives me even crazier). In 99.99% of the cases (no, I didn’t count) one of them is enough. If not, English has been kind enough to give you plenty of nice ways to indicate choices and constraints. The point is that people should know for certain whether you meant "or", "and" or "one or both", and the stroke leaves too much room for error.

* If, whether, whether or not: [Grammar Girl has it](http://www.quickanddirtytips.com/education/grammar/if-versus-whether).

* Plurals: use [common sense](http://www.theguardian.com/media/mind-your-language/2015/jul/17/two-whoppers-junior-please-with-hashes-brown-on-the-side).

## Vocabulary

Here is the correct form of several terms you shouldn’t be using: I couldn’t care less (unless you could); gobbledegook (not gobbledygook); groundbreaking (don’t flatter yourself); hovercraft (although if you find a legitimate reason to use this in mbed documentation, I’m sure we’ll all appreciate it); knowhow (it’s not two words, just an ugly one); morris dancing (as in “technical writing is the morris dancing of the writing world”); ongoing (not two words; not a word, either - it’s jargon, so don’t use it); Tardis (but see the note about hovercrafts).

### In General

* Don't give the same thing two different names. This is not a cryptic puzzle.

* Don’t give two different things the same name. That’s just mean.

* Do not make up words. If there is no un- or in- form for your word, it's not up to you to create it. If I google your word, I want to find it.

* Latin's nice and all, but if you can find an English equivalent, please use it. Normally “a” would do for “per”: “200 users a year”, not “200 users per annum”. This also applies to ie, eg and etc, which many of you sprinkle over your texts like chocolate buttons over a cake.

* Make sure your sentence doesn't include the same word more than once, hiding behind different forms. A common mistake is to use two words that mean “and a few others like this”. If you write “Such as x, y, z and more”, then “and more” and “such as” are doing the same job. “Including a, b, c etc”: “including” and “etc” are doing the same job.

* Don’t use slang or regional English unless it’s very well known, and even then remember that it can make your text sound flippant - best to use it when you’re trying to get your audience to loosen up. Remember that you have an international audience, so what constitutes “well known” is anyone’s guess (but the Texas office can probably keep saying "y’all").

* On first use, give the meaning of initials, then the initials in parentheses. For example, it’s Bluetooth Low Energy (BLE), not BLE (Bluetooth Low Energy). Don’t bother doing this with things that are more commonly known by their initials, like BBC. You can put the full term in italics if you like: *Bluetooth Low Energy* (BLE).

### Verbs

* There is a difference between the verb and noun forms of many words in software. For example, login is the noun, log in is the verb. So the window is Login, but the button is Log In (yes, buttons are verbs). Other pairs: setup/set up; startup/start up; takeoff/take off.

* You give someone a licence (noun), but you license (verb) an item.

* You invite someone to the practice room (noun), where you practise (verb).

* Log into (two words, not three).

* The [Guardian says](http://www.theguardian.com/guardian-observer-style-guide-g) Google is the correct form of the verb; I write google. Pick one and stick with it (hint: the Guardian knows more than I do).

* Don't say an option enables or allows x, because that implies not that x will be performed, but that x is now available for selection. Unless that’s what you meant, of course.

### Counting Things

* If you can count it, it's “fewer”. If you can't count it, it's “less”. This applies even if you can't, in practice, count it. This often doesn’t matter to readers, but sometimes choosing the wrong word makes a mess of your sentence. For example, you may modify a noun to be weaker (less) rather than smaller in number (fewer): “you’ll need less powerful boards” (weaker boards are enough) v “you’ll need fewer powerful boards” (if you use powerful boards, you won’t need as many).

* In a sentence, it’s:
	
	* One to ten and first to tenth.

	* 10-999,999 and 10th to 999,999th.

	* Then 1m, 5bn, millionth etc, unless you’re counting users, then it’s always “million” or “billion” (spelled-out).

	* If you're mixing numbers below and above ten, go with numerals: 4, 9 and 17 (not four, nine and 17).

	* If you're using a unit of measure, use a numeral. I often don't (I tend to write "four KB" rather than "4KB"), but I'm wrong about it.

	* If it’s the first word of a sentence, it’s always spelled out. If you don’t want to spell it out - change your sentence.

	* When you're referencing steps, it's in numerals, not words (step 2, step 14). I often get this wrong.
	
* Thanks to the Economist, we know that [last year is 2014](http://www.economist.com/styleguide/l#node-21534682). If you mean the 12 months up to now, you mean past year. This applies to month and week, too. Generally, it’s easier to give an exact date (or range of dates), so that your dates don’t become outdated.

### Now I'm Really Nitpicking

* Cannot is a single word. It's separated into two (can not) when you want to stress one of the words or when giving the option not to do something. This often makes you sound like a parent arguing with their child, so be careful.

* You may think that “whom” is dead and good riddance to it, but it has its uses: in some sentences it’s the only way to clarify who did what to whom. There’s an [easy way to remember the difference](https://www.youtube.com/watch?v=zBZgZ4e36IU#t=38). And a slightly more helpful one over at [The Oatmeal](http://theoatmeal.com/comics/who_vs_whom). Too lazy? Then rewrite your sentence so that it's clear without "whom".

* The Economist has a nice explanation of when [may might mean might](http://www.economist.com/style-guide/may-might).

* Please remember that “alright” and “all right” mean different things.

* So do “as” (causal) and “since” (temporal). I almost never obey this rule. But also note that using "as" when you mean "because" can confuse non-native speakers, so it's best to avoid it.

* And it’s “any more”, not “anymore”.

* Some readers expect "once" to mean "only one time". Use "when" if you mean "as soon as" (please don't use "as soon as" - it creates expectations of prompt results).

* Many words that time-stamp your sentence (temporal words) are unnecessary or even confusing.   

* You're supposed to use "therefore" at the start of a sentence and "so" in the middle of it. I almost always use "so". And when I do get round to using "therefore", I tend to stick it in the middle of a sentence (but between two commas; I'm not a total slob).

* Substitute by, with and for are different ideas. Be careful.

* Bottleneck (one word).

* The Guardian says: [Continual: repeatedly, but not constantly. Continuous: unbroken sequence](http://www.theguardian.com/guardian-observer-style-guide-c).

* Data is plural. Feel free to ignore that, because most Latin plurals have long-since become singular and data will not be an exception for long.

* Mass nouns (water, furniture) are followed by the singular form of the verb. So the verb following "data" is "is", which is another reason you don't need to remember that it's a plural in Latin. The easiest way to know if something is a mass noun is to try to count it: if you have to add a unit of measurement, it's a mass noun. Going back to water, it'll have to be in litres or glasses to be counted.

* Speaking of measuring: "loads of", and every rude variation of it, are not appropriate units of measurement.

* Always google “comprise”, “consist”, “compose” and “constitute” if you want to use them correctly. Or just [wait for someone to edit your texts](http://www.theguardian.com/commentisfree/2015/feb/05/why-wikipedias-grammar-vigilante-is-wrong).

* Onto is usually one word.

* Safest to say “different from”, not “different to”. Never say “different than” or “differs to”.

* [Centred on, not around or in](http://www.economist.com/styleguide/c#node-21532488). Also: [in the circumstances](http://www.economist.com/styleguide/c#node-21532496), not under them (for British English; if you’re American you can use either. So basically, you can use either).

* Foolproof is one word, and a fantasy.

* Nevertheless, nonetheless (one word).

* Oriented (not orientated) and disoriented (not disorientated).

* Identical with (not to).

* Password (one word).

* Generally, “starting with” is for when the order doesn’t actually matter, we just pick a starting point at random. “Starting from” implies that there is a logical order. So with versions, we might expect it to be “starting from”. Probably.

* The plural is antennae, though no one will be confused by antennas.

* And again from the Guardian: [Systematic: methodical. Systemic: relating to a system](http://www.theguardian.com/guardian-observer-style-guide-s).

* Try to, not try and.

* Usable, not useable.

* User-generated content.

* v, not vs.

* Under way (two words).

* Pixelated (but pixilated means drunk, so you may well be using it correctly).

## Capitalisation

For capitalisation of units of measurement, [see the last section](#capumeas).

Capitals are distracting, so when in doubt - don’t use one.

* For headers and titles, use sentence case (only the first letter and names of things are capitalised), even though as you can see I tend to use title case. This will save you the trouble of figuring out if “from” is capitalised in title case.

* If you really want to use title case that’s fine. Just <del>remember that some words are only capitalised if they’re at the head of a sentence, even when using title case. These include (but are not limited to): a, an, and, be, for, from (depending on who you ask; I asked the Guardian), in, is, of, off, on, or, the, to, too.</del> use [http://titlecapitalization.com/](http://titlecapitalization.com/).

* When referring to a keyboard key, use the short form and capitalise the first letter of every word in the name: Tab, Del, Enter, Page Up, Num Lock.

* There is a difference between initials and acronyms:

	* Initials: when you pronounce each letter. Do not use spaces or dots between the letters: BLE, API.

	* Acronyms: pronounced as a single word. Capitalise only the first letter and do not add spaces or dots: Nasa, Nato (no, I couldn't think of a relevant example).

	* LED or Led? Well, people pronounce them both ways, but for now we’ll stick with LED. That means that the article is *an*, not *a* (to fit the pronunciation “el ee dee”).

	* Companies get to name their own stuff and determine its spelling; always follow official spelling, ignoring the rules I just specified. So it’s GATT, not Gatt. Also gif and pdf, not GIF and PDF. What do you care how gif is pronounced? This is a writing guide.

* Do you use a capital letter after a colon? That sort of depends on what follows it. So the easy answer is “if you want, just be consistent”. If you want the complicated answer, google it. Then be consistent.

* Do not use a capital letter after a semicolon.

## Punctuation and the Such

Punctuation is the worst problem in many texts: it changes the meaning of a sentence, so if you don’t punctuate correctly you may [end up in a book](http://www.amazon.co.uk/Eats-Shoots-Leaves-Lynne-Truss/dp/0007329067).

The short story: punctuation is here to help the readers. So if a punctuation mark helps - use it. If it doesn’t - don’t use it, because it just clutters up the view. In other words: use the rules as a guideline only; they’re [not that clear-cut](http://xkcd.com/1167/) anyway.

If you want to, you can write an entire readme file with only commas and periods - but I think you'll have less fun. So with that in mind:

* Periods, or full stops: very helpful. Short sentences are easy. But - they give you an odd staccato. Don't overuse.

* In the interest of not using too many periods, there’s a move away from using them inside or at the end of words like eg, etc and ie. You can use them if you really like them, but don’t get confused if you don’t see them.

* Commas are used to give readers a chance to inhale, so if you let the little voice in your head tell you where to put the comma, you should be fine. But be careful: a comma can change the meaning of a sentence, and the little voice in your head may be trolling you (or, like mine, slightly asthmatic).

* Regarding the Oxford Comma: I use it only when it helps clarify the sentence, sticking to the principle of removing unhelpful punctuation.

* The semicolon is the most awesome of the punctuation marks (and Vonnegut will [pardon me](http://www.goodreads.com/quotes/17178-here-is-a-lesson-in-creative-writing-first-rule-do)). By all means, use it. [However](http://theoatmeal.com/comics/semicolon), please remember that since the semicolon is used to connect ideas, it shouldn’t be followed by a connecting word (conjunction), so no “and”, “but”, “or” etc. If you think the relationship between the parts isn’t clear without a conjunction, change the semicolon to a colon or period and use the conjunction. Also: no capital letter after a semicolon, since you’re not starting a new sentence.

* Exclamation marks are the written equivalent of laughing at your own jokes. Don't.

* Quotes are wrongly used at least half of the time; don’t use them to draw attention to a word or to emphasise anything.

* I encourage you to use colons when you’re introducing things like lists or bits of code. Or as Fowler put it (quoted by [the Guardian](http://www.theguardian.com/guardian-observer-style-guide-c)): “[Use a colon] to deliver the goods that have been invoiced in the preceding words”.

* I love dashes, and probably overuse them. Here’s [the Economist](http://www.economist.com/style-guide/dashes): “Use a dash to introduce an explanation, amplification, paraphrase, particularisation or correction of what immediately precedes it. Use it to gather up the subject of a long sentence. Use it to introduce a paradoxical or whimsical ending to a sentence. Do not use it as a punctuation maid-of-all-work.” (Gowers). In pairs, they can be used more or less like parenthesis.

	Please remember that a dash and a hyphen are not the same: if you put a space on either side, it’s a dash; if you don’t put any spaces, it’s a hyphen; if you put one space, you’re doing it wrong.

* Hyphens:

	* I tend to overuse them, so you might want to listen to someone else ([the Guardian](http://www.theguardian.com/guardian-observer-style-guide-h)): “Most adverbial phrases do not need hyphens. Never use them after adverbs ending in -ly, eg constantly evolving newspaper, genetically modified food, hotly disputed penalty, wholly owned subsidiary.

		For adverbs that do not end in -ly, use hyphens only when there would be a possibility of ambiguity without one, eg an ill-prepared speech. 

		But phrases such as ever forgiving, near fatal, now defunct, once popular, etc do not need hyphens.

		Exceptions: much and well when used before a noun, eg a much-loved character (but a character who is much loved), a well-founded suspicion (a suspicion that is well founded), etc.”

	* Avoid using them when the word is formed by one word and a short prefix, such as bi-, de- and neo-.

	* But the Guardian warns: “Use re- (with hyphen) when followed by the vowels e or u (not pronounced as "yu"): eg re-entry, re-examine, re-urge. Use re (no hyphen) when followed by the vowels a, i, o or u (pronounced as "yu"), or any consonant: eg rearm, rearrange, reassemble, reiterate, reorder, reread, reuse, rebuild, reconsider, retweet. Exceptions (where confusion with another word would arise): re-cover/recover, re-creation/recreation, re-form/reform, re-sent/resent, re-sign/resign”.

	* Use them in fractions.

	* Switching for a moment to [the Economist](http://www.economist.com/style-guide/hyphens), use them for most words that begin with anti-, counter-, half-, inter-, non- and semi-.

	* Use them to avoid ambiguities: mbed-enabled boards (boards that have mbed bits) and mbed enabled boards (mbed did something to boards) are different sentences. But do note that it's now "mbed Enabled", so you don't need the hyphen to avoid the ambiguity. 

* Use a question mark only when you’re asking a question, not to indicate uncertainty. And please use a proper question, not a statement - those are different constructions in English.

* Don’t use ellipsis... it's almost never useful in a technical text.

* Lists (numbered or bulleted) need a period or question mark at the end. Don’t use a semicolon or comma.

* Where do you put the punctuation mark for a sentence that ends with parentheses? I put it after the parenthesis, always, even though that’s only half-correct. If you want to get into the area of “well, that depends on what goes in the parenthesis”, both of our reference style guides can explain it.

* Please don’t use apostrophes to make plurals. It’s UUIDs, not UUID’s. And it’s dos and don’ts, not do’s and dont’s (and the plural of no is noes).

* To avoid looking funny, don't use the possessive form for an abbreviation, because that puts the apostrophe just where I told you not to put it (the UUID's job is to…). Better to rearrange the sentence to a slightly clunky form (the job of the UUIDs is to…).

* For other uses of apostrophes: if you're confused, reword your sentence so that you no longer have to figure out whether or not you need one. Please note the difference between "rewording" and "just ignoring it".

## Ambiguity

Ambiguity is English's superpower. The sentence structure is flexible, but the words don't always indicate their role in the sentence. Words have dozens of meanings, and often several of them can fit the sentence - making perfect grammatical sense while changing reality. Compound nouns abound ("National Basketball Association slam dunk championship all-star tournament finalists". And you dare make fun of German?). You are not going to eliminate all ambiguity from your writing, but you can make an honest effort not to be Hamlet.

Read each sentence twice (at least), giving the words their different possible meanings and linking them differently. Did the meaning change? Here's an example:

> "I saw it in England. It is so common there is a store on every corner."

This example is based on the two possible meaning of the word "there": it can mean "in Germany" and it can be the first part of "there is". Which meaning did you give it the first time you read the sentence? Obviously this sentence resolves itself as you read it to the end, but it would help the readers if it didn't catch them out (for example, by writing "there's" or using a comma).

Here's [an example](http://www.itv.com/news/meridian/update/2013-12-31/southeastern-run-late-trains-for-new-years-eve/) that can be fixed with a hyphen:

> "Southeastern trains are running extra late night services."

They meant late-night, not extra-late. Probably.

Sometimes, as in the first example, the context of the sentence makes the meaning clear. In that case all the reader has lost is the two seconds it took to switch meanings. But some sentences are completely undecipherable without extra information. Consider this [miraculous example](https://en.wikipedia.org/wiki/List_of_linguistic_example_sentences):

> "Did you ever hear the story about the blind carpenter who picked up his hammer and saw?"

This sentence is only clear to the writer. You can spot these sentences by changing your inner voice to put stress on different words than you normally do; this will flush out possible readings that you hadn't thought of. Here's [another example](https://en.wikipedia.org/wiki/List_of_linguistic_example_sentences):

> "I saw her duck".

Putting the stress on "her" makes the duck either a noun or a verb, but if it's a verb then who didn't duck, and what happened to them? Putting the stress on "duck" makes it a verb without giving a hint that there's anyone who didn't duck. A far less interesting story.

This is not an exhaustive list of the ways English writing can trip up readers. Be mindful of the different ways a sentence can be interpreted as you write.

## Using Jargon

[Don’t](http://www.amazon.co.uk/Who-Touched-Base-Thought-Shower/dp/1444781847).

Never confuse field-specific vocabulary with jargon. The first is necessary to all fields and specific to each one, the second is useless and identical in all fields (although the self help people are driving a goals-oriented approach to markedly distinguish the essence of their individual personalities by meticulously crafting a holistic communication experience that is both unique and networking-supportive). Use the simplest word that accurately describes what you’re trying to say, and don’t use more words than you need.

Every style guide you’ll read will, at this point, quote [Bill Bryson](http://www.theguardian.com/guardian-observer-style-guide-j): “[Jargon is] the practice of never calling a spade a spade when you might instead call it a manual earth-restructuring implement”.

Here’s a handy way of identifying jargon: imagine a politician saying your sentence. If you rolled your eyes, it’s jargon.

________

<a name="mbed">
# mbed
</a>

## Proper Nouns

Quick flashback to school (stop screaming, it will be over soon!): there are two kinds of nouns, proper and common. A proper noun points to a unique thing, and it therefore takes no article (unless the article is part of the name, like the Rolling Stones). A common noun, on the other hand, points to a class or a non-specific instance of a class, and therefore takes an article.

When you're referring to specific APIs, functions, services and so on, the structure of the sentence is how you'll know if they're proper or common. "We use BLE_API" - this is a specific API. It's a proper noun, and therefore takes no article. "We use the BLE, not WiFi, API" - you're talking about two kinds of API, and the focus is on the API. The two kinds - BLE and WiFi - are treated as common nouns, and they take the article "the". You'll note that we didn't use their proper names (BLE_API has an underscore, "the BLE API" doesn't).

The difference is more obvious in the following two sentences: "we call waitForEvent()" and "we call the waitForEvent() function". The reason you needed the article "the" in the second sentence is that you used the word "function", rather than just the name of a specific function

This is not 100% consistent. Nothing in English is, though, so I’m not too worried.

## Processors

You can only use processor names as adjectives or adverbs. For example, refer to the ARM926EJ-S processor, not the ARM926EJ-S.

## The rest

* mbed OS, not mbedOS or mbed-OS. And if you're adding a trademark, it comes after OS: mbed OS™.

* ARM mbed (two words).

* mbed Enabled (to match the name of the partner program).

* No capital letter in mbed, even at the start of a sentence. Be careful with this - autocorrect will change it.

* Also not capitalised: yotta.

* micro:bit, no capitals and with a punctuation mark in the middle of the word.

* mbed TLS (two words).

* Runtime (one word).

* Microcontroller (one word).

* Online (one word).

* Read/write, despite my habit of separating them.

* In ARM documentation, PC stands for "program counter", not personal computer. So use either "Windows workstation" or "Linux workstation".

* Silicon. If you add an E at the end, you’re in the wrong industry (you could be earning loads more).

* sim, not SIM. Many people object to this; go with SIM if you prefer.

* I have no idea where the word breadboardable came from, but I love it.

* Wap (note the W, not w) phones.

* world wide web, despite worldwide usually being one word. Cause it’s English, that’s why.

* Wi-Fi or WiFi. Pick one, I give up.

* Ethernet, not ethernet.

* micro-USB, but if you really want Micro-USB you can roll with it.

* Smartphone, smartwatch (one word).

* Point-to-point, with all those hyphens.

* It’s possible, so we’ll go with it, that “plug and play” is the technology, and any other spelling is either wrong or a brand name. So use plug and play, not Plug And Play, Plug’N’Play or anything like that.

* Normally (by which I mean - when I write) we use “press” for a physical button or key (like the power button on the boards, or keyboard keys) and “click” for something on the screen (like the compile button).

* If the button has a name (written on it) you can refer to it directly (with the capital letter, and you can also use bold font if you want): “click **Compile**”. But if there’s just an icon, it’s best to use a few more words: “click the search button” (no capital, and using an article, because there’s no name for the button).

* Downstream.

* Program (for software; it’s programme in every other context).

* Memory map, not memory-map. But the adjective is hyphenated: memory-mapped.

* flash memory, not Flash memory.

* Laptop (one word).

* BlackBerry and BlackBerrys, not berries.

* If you’re using someone else’s stuff specify it on first mention. Link to it, too; it’s the polite thing to do.

* Services and Profiles or services and profiles? That depends on context. If you’re talking about a specific profile or service and giving its full name, it’s probably Profile or Service. If you’re talking about the general concept, or if you’re referring to a previously-mentioned profile or service without giving the full name again, it’s profile or service.

* Boot loader, not bootloader. Not everyone agrees with me on this, so you can ignore me.

* GATT, despite the fact that it’s pronounced Gatt.

* SoftDevice.

* FOTA (not FOtA).

* LED (although many people pronounce it like the past tense of lead). The article is an, not a, since we assume people pronounce it “el ee dee”.

* mbed BLE, not mbed/BLE.

* mKIT.

* High frequency and low frequency (no need for a hyphen).

* High power and low power (probably).

* Power up and power down (not on and off) for the verbs. Powerup and powerdown for the nouns.

* I/O (not IO).

_____

<a name="capumeas">
# Capitalisation of Units of Measurement
</a>

* Remember the good ol’ days when computer terms were set by computer people? Well, those days are over. [So now KB, MB and GB mean “1,000”](https://xkcd.com/394/). A nice, round number, to be sure, but missing the sciency feel of two to the power of ten.

	If you want to say 1,024 you’ll now have to use KiB, MiB and GiB.

* b == bit.

* B == byte.

* MB/s (megabyte), Mb/s or Mbps (megabit).

* Gb == gigabits.

* GB == gigabytes.

* 𝜇A == microamps.

* W watts, kW kilowatts, mW miliwatts, MW megwatts.

* J joules, kJ kilojoules.

* Hz, MHz.

* dB for decibel.

* The short form of minutes is min, not m (because m stands for meter).

* But seconds is s, not S.

* When talking about signal states, it's HIGH and LOW. I also like TRUE and FALSE for binaries.
