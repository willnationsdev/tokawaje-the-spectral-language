# Tokawaje: The Spectral Language

##### Author:

Will Nations

##### Publication Date:

April 17th, 2017

---

# Preface

Let it be known at the outset of this venture that I am not a linguist (far from it, in fact). I am a programmer who enjoys the field of creative writing and game design, among other things. As such, although the entire purpose of this book is to provide an introductory instruction to a language of my own invention, I dare not assert that the choices I have made in designing the language are well-informed. Those with more experience in the field of linguistics will likely have much to say in communicating faults with my technique; I welcome such criticism.

This section of the book shall merely attempt to relay my motivations, so that those who bare their criticism at the project will do so with an informed and constructive spirit. Should you believe there is an issue with the designs herein, I look forward to reviewing your suggestions on how to evolve tokawaje into a more suitable tool for our target environment.

Tokawaje, at its core, is the product of my efforts to create a unified language between the following entities:

- writers: those who write stories who could benefit from a computer understanding the content.
- virtual designers: those who detail the flow of events or describe the content of virtual experiences.
- programmers: those who script behaviors for game engines or story-oriented software.
- players: those who participate in virtual experiences.
- modders: those who wish to edit the content of virtual experiences after they are published.
- software applications: programs that must interpret narrative or abstract information.

In game development, narrative content is generally something that writers create; however, many writers are unable to manipulate gameplay as level or UI designers without first learning about the tools of those trades: a scripting language or a GUI editor. Likewise, designers must learn the ins and outs of a scripting language in order to translate the thought of "I want X to do Y under Z conditions" into actual behavior. Furthermore, all of the assets for this content generally have to be handcrafted by the content creators.

Outside of the development team, we've had great success in subsections of content creation: The advent of games like Minecraft have enabled players and modders to create geometric content mid-game while computers have become better at generating the same type of content. However, abstract concepts have not achieved the same fruition of digital creativity. It's not as if players can enter a game, begin describing ideas, and automatically have a computer system bring those assets and mechanics to life in the virtual space. Why is that? The simple reason is that the language people use to describe abstract concepts currently has no simple translation into a computer-readable language.

To bridge this gap, I am implementing a novel framework for linking language semantics to computer functionality, known as Wyrd (pronounced "weird"). Its parser allows one to link a dialect consisting of a set of phonemes and alphabetic or hieroglyphic writing to a dictionary of abstract concepts. An interpreter converts these syntactic concepts into semantics, allowing a level of indirection so that multiple statements can be associated with the same narrative idea. Finally, a narrative engine accepts the semantics as input and converts them into instructions that a game engine (and other applications) can understand. This modular approach should keep the language as flexible as possible so that people of all backgrounds can use it in whatever manner works best for them.

Given a system like this, you could...

- Create your own dialect so that voicing different sounds or inputting different symbols results in the same dictionary of abstract concepts.
- Create your own dictionary produced by the parser to define the mappings between phrases.
- Create your own interpreter allowing you to define the semantics associated with a statement structure.
- Create your own narrative engine to interface with an application and link semantics to in-app behavior.

Tokawaje is but one illustration of a dialect/dictionary/interpreter triplet. It contains an alphabet and svg-based hieroglyphs both matched to phonemes, a dictionary of vocabulary terms and grammar tags as well as an interpreter to define word relationships and their corresponding semantics. What's more, it is designed with players in mind: a user-friendly set of phonemes and a minimal vocabulary intended for accessible learning while the language's interpreter leverages a spectrum-based system to maximize the available semantics for such a minimal language. This will enable people who have never semantically communicated with or modded a game to quickly learn how to do so.

Any game that takes a systems-based approach to designing content can take Wyrd instructions from a narrative engine and plug them in to procedurally generate content. The instructions themselves are generated from people (players, modders, designers, etc.) simply stating what they wish to do.

What follows is an explanation of the tokawaje triplet, and the semantics it will be able to make available to narrative engines. Many aspects of tokawaje have been derived from other constructed languages such as toki pona and Lojban, but you may also find that the language itself has a high number of English cognates (similar-sounding words) to simplify others' adoption of it.
