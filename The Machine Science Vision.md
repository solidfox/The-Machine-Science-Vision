# The Modular Science Vision

By Daniel Schlaug ーl July 2017

Science is unnecessarily too hard. It should be very different.

I am no scientist and so I must admit to feeling a bit naive to start meddling in the fundamentals of meta-science. I belong, however, to the group of people that might be argued to be handling the largest amount of information in the world and I cannot help but be vexed by the current state of scientific writing.

In computer science we are drilled to do even the smallest things formally, reproducibly and with as little duplication as possible. We obsess about authenticity to the extent where even what you ate for breakfast will be fed through complex cryptographic math to ensure that it was actually you who posted that peanut butter pizza. We go out of our way to carefully log every step of the way in even our silliest work. And we have an enormous infrastructure in place to comment on, propose changes to and concurrently alter everything from the most specialised and obscure piece of logic that probably never will be used to the fundamental frameworks through which almost all information flows.

Looking at the scientific community from this programmer’s perspective, it is astonishing to see how the most consequential information of humanity is produced, processed and collaborated on using the same communicational toolkit used hundreds of years ago. While scientists are still writing reports and articles like it's 1665, programmers are reinventing their tools every other year.

I believe science would greatly benefit from taking advantage of adapted and evolved versions of the tools programmers use everyday, such as version control, package management and cryptography. These tools enable the lone developer to leverage decades worth of previous programming work and this is exactly what scientists constantly do, only in science has been improved upon for centuries, not decades. Computer scientists will contest that they are in fact already using these very tools for science. While partly (and only partly) true, those who do some of the most important science, like physicians, are still emailing around Excel datasets and *everyone* is publishing on paper (or it's digital counterpart - pdf).

## Scientific text

Science is an altogether social enterprise. Its arduously carful knowledge generating methods would likely be rendered much too unwieldily without the sharing, validation and competition that run so deep within its veins. Although the personal interaction in conferences, academies and institutes play an undeniable role in this community it is in scientific text that most encounters with new science happen. Although popular science reporting is keeping up well with recent medial developments I would argue that the scientific social medium has been left behind in the dusty remnants of a format that had its glory days back in the 17th century.

And yet the responsibility of scientific communication is immense. The better we communicate science, the more new knowledge will spread and the faster will this knowledge be corrected, refined and extended. The implications of this grandest of mankind's undertakings has no thinkable bounds. The failure to communicate science will bereave the individual of health and happiness, the society of sound politics, equality and peace, and the earth of the very balance of nature. With the massive human population that currently strains our planet it would be no overstatement to say that the effectiveness and efficiency of scientific communication is the tipping point between order and chaos. Scientific communication is certainly not something that deserves to be left in dusty journals while the rest of the world is tweeting, Facebooking and Youtubing more efficiently by the hour.

## The main problem

The original thought of this article was to investigate the feasibility of using web technologies instead of Word, LaTeX, PDF and paper as the platform for scientific writing. This has been explored before, to name a few approaches language-wise there’s [Scholarly Markdown][1], [Markua][2] and the [GitHub endorsed][3] [ASCIIDoc][4], in the realm of word processors there are the likes of [Authorea][5] and [substance.io][6]. The problem with all of these is that they still try to replicate the traditional way to write science. I’ve had too much time to obsess over what good science is and how to perform it and my intuition is that the problem with academic writing is not in the syntax, platform or software but rather in the very structure we barbarically smear science onto.

Scientific results are already being published by the thousands every day, growing at a rate of about 4% per year according to [Science growing too fast][7]. That’s exponential, which is great but how is anyone to get an overview of this? Is it really feasible to continue recording these findings in loosely structured natural language reports that, each of them, reiterate descriptions of the previous work? Would it not be better to find the essence of what these reports are communicating and establish a strict, albeit heavily extendible language that only communicates this essence? The magnitude of different kinds of information that we currently mash together into scientific reports is quite astounding. These are but a few:

- Declarations of work that the current work is based on.
- Pedagogical reiterations or alternative perspectives on previous work.
- Relationship between previous and current work.
- Data and how it was collected.
- How data has been processed.
- Results of the data processing.
- New knowledge that may or may not be inferred from the results.
- Explaining the implications of the new knowledge.
- Ethical considerations regarding the work.
- Ideas about how to continue the research.

Some of these parts, such as pedagogical text and graphics, are targeted at humans. Other parts, such as the full data, is almost always processed by computers in some way before it is consumed by humans and thus should be viewed as targeted at machines. Yet other parts, like the connections to previous work, could well be consumed both by humans and machines but in very different forms. The loose structure of scientific publication that we currently use is only really aimed at humans, severely limiting our ability to exploit the unique potential of machines in processing, compiling and verifying its contents, meaning and implications.

Natural language makes it too easy to entangle these different parts, omit necessary details, create ambiguity and let mistakes slip through. This makes publications very difficult (if not impossible) for computers to automatically and accurately parse and process. It also makes it difficult to propagate and make clear the implications that new findings or retractions have on previous science. Furthermore it makes a lot of raw science inaccessible to anyone but the experts in the field, leading not only to inhibited inter-disciplinary work but also to the many misinterpretations that we see in media today and subsequently to public misinformation and sometimes even loss of confidence in science.

Then there is the pain of writing lengthy reports. While the puzzle of programming often mesmerises even the least tech savvy people I have seen attempt it, authorship generally tends to be considered a more arduous business. Quite rightly so, composing an enjoyable text takes quite a bit of skill and experience while a sufficiently clear piece of code requires little more than familiarity with the syntax or the right tools and an understanding of the thing to be communicated. Code tend to communicate relevant information as succinctly as possible, just as scientific text should but too often fails to do. This is what should be expected of a scientist, not a long, wearisome and less parsable text. There certainly exist those who can’t seem to put a sane sentence together but nevertheless excel in chemistry, abstract algebra or bayesian machine learning. As long as you can communicate the structure of your work, maybe with a few technical comments where needed, you can be a scientist. The work of making it all comprehensible to different audiences is undoubtedly important and should be done but needn’t necessarily be done by the creator or explorer of the theory or method.

## A format that can evolve with science?

So how does one go about wrangling science into it a sweet spot with enough expressivity to encompass the most novel of future ideas and projects while still keeping things formal enough to be machine-readable and making it difficult or impossible to make methodological, statistical or logical mistakes. The Semantic Web was (or is) an effort toward a similar goal. That effort seems to have slowly died out while machine learning has been taking off as the method by which computers make sense of the world’s information. Whereas the Semantic Web was about manually creating structure by hand, mostly through ontologies, machine learning is deriving it from example. There’s really no reason we could not use machine learning to distil ontologies or use ontologies to power up machine learning, thus combining the two but looking at the [Google trends][8], the semantic web seems to be the hype of the last decade, or even the pre-Google era. Nevertheless ontologies are fantastic ways of describing concepts and how they are related, and in a scientific setting I believe both the demand for such structure and the technical capabilities of those who would create them to be far greater than for the general use case of the web.

### Ontology

The first deliberate definition of ontology in computer science was coined by Tom Gruber in the early 1990;

> An ontology is a description (like a formal specification of a program) of the concepts and relationships that can formally exist for an agent or a community of agents. This definition is consistent with the usage of ontology as a set of concept definitions, but more general. And it is a different sense of the word than its use in philosophy.

Thus an ontology in computer science describes concepts and how they relate to each other. It is similar to a schema in that it allows us to constrain the structure of information. But unlike for example an SQL schema it does not (necessarily) deal with the technicalities of how the information is physically stored (e.g. 32 bit Integer or Unicode string). Technical implementation details are not part of the scientific structure and should probably be stored separately so that the structure may be represented through many different technical implementations. That said, nothing prevents an ontology from using concepts from programming languages such as classes, subclasses and interfaces.

Ontologies are obviously extremely flexible and enable many different ways to model the same set of concepts. While this does indeed produce issues similar to those of the natural language it also allows us to establish formal and parseable models of both science and meta-science. These models could then, like frameworks or packages in any programming language, be imported and referred to in new models. 

Even tough it adds complexity and potentially inhibits interoperability it would, for the sake of improvement through competition, seem necessary to refrain from limiting oneself to one “master” ontology of science. As we have seen previously, e.g. in the battle between foundationalism and coherentism, allowing fundamentally different views on what knowledge is prevents us from locking into intractable terrain. In the case of ontology it is not just on the nature of the knowledge that opinions may differ but also on the best way to structure it. And tens of different largely accepted structures must still be seen as better tan no standardised structure at all.

Then again, there is nothing to prevent us from building an ontology of the relations between the different “fundamental” ontologies, thus indeed combining them all into one master ontology. This may also be quite useful for the purposes of comparing or converting between paradigms. The point is rather that this may not be entirely necessary and it should be easy to try out major paradigm changes - without first relating them to current ones.

### Evidence

Evidence - the threads through which any theory levitates. The observations of the world from which we derive all that we know. When evidence is forged or otherwise misrepresented that which we derive will not be knowledge but rather the most devastating of confounders. The authenticity, representation and understanding of evidence is therefore of dire consequence. Recently a few studies have begun employing unbiased observers to inspect and authenticate the data collection. Still, many - probably most - have never heard of such practices. And while the amount theory available on how to correctly perform data collection, representation and analysis is certainly abundant far from every scientist has mastered this. I would claim that is as it should be, incidents like the recent reproducibility crisis indicate that science is difficult enough for it to be misused not only by media, politics and your average citizen but also by formidable scientists. Science should therefore be structured in a way that makes it really hard to make mistakes. Such a change should take a lot of unrelated meta-science work off the mind of scientists while asserting that rigid authentication and meticulous use of meta-science is ubiquitous. Or at the very least any data produced without meeting these standards could be automatically flagged as such. Today it is often not. For all our efforts with peer review and replication a considerable amount of bad science still make it through the filters.

Considering the extensive meta science we have at hand, I believe the path we should take is one of formal and automatic checking. This requires a formal language for describing data. And by describing data I do not mean that it needs to actually contain the data. This kind of metadata could certainly be aware of the actual data and how to read it, be it csv, json, a binary database, images, movies or some future unknown format, but the focus should be on describing every known detail about the structure of the data and how its collection was planned and carried out from a meta-scientific standpoint. Some examples of what could be detailed:

- Whether any parts of the collected data has been discarded.
- Checksum of the intended data.
- Method of generation including technology, questionnaires, algorithms and the best known scale, domain and accuracy of these methods.
- Auxiliary hypotheses of any used methods as well as if and how these have been considered.
- Any assumptions required by the method as well as if and why these assumptions can be made for the study at hand.
- Any causes for bias within the team or the explicit lack thereof.

Having this kind of structured metadata as a standard would make it easy to impose requirements that would make the work fail verification when important considerations like whether outliers have been removed are not explicitly stated. Even though such verification is important it should not be expected that every study will be able to provide all this information and therefore “unknown” should also be accepted as an answer. The presence of “unknown" would still assert that the author has considered the aspect but been unable to detail it and future readers or parsers would be able to communicate this flaw in a manner appropriate to its severity in any given case. Finally authors, observants and reviewers should be able to vouch for any metadata by placing digital signatures on it, thereby becoming liable if the metadata should prove to be incorrect.

One example of such a process could authenticate evidence by having neutral or opposing parties present as evidence is being collected so they can verify that data has not been fabricated and the stated methods (such as double blinding) were correctly applied. As mentioned above this kind of authentication is already being carried out but having a formal language defining which properties can and should be signed and a standard for electronic signing would make it much easier to quickly identify and communicate concerns about evidence reliability.

Another example could be a specialist statistics department reviewing the use of statistics and the following inferences, placing a signature on their validity along with their comments or possible reservations.

## The vision of a world with machine-readable science

This section takes on quite liberally and concretely imagining what the scientific world could look like if it was structured enough to be easily machine-readable.

Some may contend that some of these things are too fantastic and would be unreasonable to build. Consider, however, the startling pace at which the open source community is advancing and how both individuals and organisations of all sizes are donating their time contributing to this. It would seem that when humans are enabled to easily advance all of humanity this creates an enormous motivation. Pouring science straight into this sprawling pot of wonders may well produce quite unbelievable results indeed.

### Autocomplete Science

This text ended up being on a higher level than that of editors for scientific text but it should be mentioned that if this is to have a chance of being all-encompassing it needs an editor (or toolkit) that non-programmers feel comfortable with. I imagine it would be an engine that takes constraints from the user while exploring ontologies to display possible ways to further constrain and build the report.

You might start by indicating that you want to check if a causational relationship exists between two concepts. The engine finds you the meta-scientific frameworks currently supporting drawing causational conclusions, you pick one and the engine goes on to display different existing methods for drawing these conclusions. Next the engine checks all the requirements for the method, asking you how you intend to fulfil each one. It then either asks you for the input and results of the method or simply asks for the input data and automatically generates the results along with any known concerns that should be declared.

That's how simple science should be (in many cases).

Now, if someone finds an issue with the method above it will be immediately clear what knowledge or which projects are compromised by the issue and, if the method is fully automatic, it could be amended and rerun to see what results are is affected.

### Beliefs and Bayesian nets

With science structured into ontologies or a format from which an ontology can be easily derived there's also the opportunity to insert cause relationships and beliefs thus enabling us to automatically creating and updating likelihoods of certain facts being true. This could clearly illustrate which theories are shaky due to limited data or unreliable research methods. It would also help in resolving the misconception that science does not produce absolute truth but only the most likely truth given the data available at the time.

### Conformance checking

There exists too many mathematical notations in bleeding edge science. Reading some of the more shady ones is often a real bother, especially to someone new to the field. As far as conventions exist their use certainly should be encouraged but searching for reading conventions while dashing to meet the deadline for a conference is not only stressful and unlikely to happen but also not the most exciting process. In software development this is solved by having the editor do automatic checks that you are sticking to your chosen (or the default) convention. Are you using the correct variable names? Are things laid out in a way that people will recognise? With a more formal language of science this kind of technology could also be carried over.

### Walking the international edge

With the pace science is currently unraveling new knowledge one might rightfully pose the question "do we know what we know?" Indeed finding out what we have already found out is a project in itself, as is evident from the many and popular meta-studies and literature reviews currently being carried out. But at thousands of published papers each day even such studies must quickly become obsolete. In order to do valuable research one needs to be able to find the edge of what we know and the possible ways of extending it. Currently this is rarely even possible due to language barriers leading to examples where findings important enough to receive Nobel Prices have been obscured by foreign (mostly asian) languages and brought to light only after the same findings where by chance repeated by an English team that subsequently received the Nobel price. 

Furthermore, with ever growing specialisation initially diverging fields may be converging on similar issues without realising it due to limited inter-disciplinary exchange, differences in vocabulary etc.

If science was structured finding the edge of what we know could be done more or less algorithmically, creating a public and live dashboard of the state of science, similar to that each scientist tries to keep in their mind for their own field by keeping up with journals and conferences. Language barriers are much less of an obstacle to code than it is to natural language and if everyone would build on the same, multilingual ontology it would be more evident when potentially vital new research has yet to have it’s comments or notes translated since this would likely be marked up as solving existing issues or being otherwise related to hot topics. Finally, concepts that are similar enough to be potentially identical could possibly even be automatically identified and marked as synonymous, alerting scientists to the fact that they might have valuable colleagues in another field. Even if this could not be done automatically there certainly are a few inter-disciplinary individuals who must occasionally be noticing these similarities. Simply providing a simple and standardised way for these individuals to alert the entire society might go a long way.

## Conclusion

The information science produces is the most important information humanity has. Making it more modularised and machine readable is likely to bring enormous benefits both to scientists and the general public through outcomes such as more reliable evidence, more intelligent authoring tools, better and instant localisation, adaption to different audiences and identification of converging fields of research. One way to achieve this would be to shift the way science is reported from natural language texts to entries and amendments to formally declared ontologies. Rather than taking this approach current developments are focusing on making it easier to write and process the current form of scientific texts. This does nothing to improve structure or encourage/enforce the use of best practices in studies. Rather, work should be done to establish standards for a modularised science taking care to make these easy to bootstrap with stubs of previous research and tools good enough to motivate scientists to take the plunge into an entirely new paradigm of scientific communication.

[1]:	http://scholarlymarkdown.com
[2]:	http://markua.com
[3]:	https://hackernoon.com/living-the-future-of-technical-writing-2f368bd0a272
[4]:	http://asciidoctor.org/docs/what-is-asciidoc/
[5]:	https://www.authorea.com/
[6]:	http://substance.io
[7]:	http://blogs.discovermagazine.com/neuroskeptic/2012/09/30/science-growing-too-fast/ "Science growing too fast, Discover Magazine"
[8]:	https://g.co/trends/Y69A1