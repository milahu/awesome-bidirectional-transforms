# awesome bidirectional transforms

bidirectional transformations, bidirectional programming, symmetric compilers, lenses, optics, ...

TLDR: i was looking for something like [Facebook CodeGen](#facebook-codegen)
= AI source-to-source transformer

https://en.wikipedia.org/wiki/Bidirectional_transformation

> More general is a lens language, in which there is
>
> a distinguished **forward direction ("get")** that takes a concrete input to an abstract output, discarding some information in the process: the concrete state includes all the information that is in the abstract state, and usually some more.
>
> The **backward direction ("put")** takes a concrete state and an abstract state and computes a new concrete state.
>
> Lenses are required to obey certain conditions to ensure sensible behaviour.

http://bx-community.wikidot.com/relatedpublications

https://kidneybone.com/c2/wiki/BidirectionalCompiler

https://en.wikipedia.org/wiki/Source-to-source_compiler

https://www.geeksforgeeks.org/source-to-source-compiler/

## machine learning

### tensorflow transformer

https://www.tensorflow.org/text/tutorials/transformer

> A Transformer is a sequence-to-sequence encoder-decoder model

> Transformers are able to capture distant or long-range contexts and dependencies in the data between distant positions in the input or output sequences. Thus, longer connections can be learned. Attention allows each location to have access to the entire input at each layer

### Self-Attention

How Transformer is Bidirectional - Machine Learning

https://stackoverflow.com/questions/55158554/how-transformer-is-bidirectional-machine-learning

#### Attention is All You Need

paper https://arxiv.org/abs/1706.03762

#### BERT

NLP transformer

NLP = natural language processing = human languages

> BERT, or Bidirectional Encoder Representations from Transformers, is a new method of pre-training language representations which obtains state-of-the-art results on a wide array of Natural Language Processing (NLP) tasks.
>
>Our academic paper which describes BERT in detail and provides full results on a number of tasks can be found here: https://arxiv.org/abs/1810.04805

> BERT is a method of pre-training language representations, meaning that we train a general-purpose "language understanding" model on a large text corpus (like Wikipedia), and then use that model for downstream NLP tasks that we care about (like question answering). BERT outperforms previous methods because it is the first unsupervised, deeply bidirectional system for pre-training NLP.

https://github.com/google-research/bert/issues/15

> core Transformer implementation is in modeling.py
>
> based on the one from tensor2tensor (but with less abstraction) and Attention is All You Need

#### tf-transformer

TensorFlow 2 implementation of Transformer (Attention is all you need).

https://github.com/chao-ji/tf-transformer

> long-distance dependence relationships, which is key to recent breakthroughs in methods for text representation learning such as BERT and GPT-2.

> At the core of Transformer is the Self-Attention mechanism, where the goal is to compute a contextualized representation of each token in a sequence by letting them "pay attention" to each other.

### machine learning tree transformations

aka: machine learning source to source compiler

#### Facebook CodeGen

aka: Facebook TransCoder

an AI source-to-source compiler

https://github.com/facebookresearch/CodeGen

> processors are based on TreeSitter parsers

https://github.com/facebookresearch/TransCoder

> This repository is deprecated, please now refer to : https://github.com/facebookresearch/CodeGen

https://www.geeksforgeeks.org/facebook-transcoder/

paper https://arxiv.org/abs/2006.03511

#### Facebook TransCoder

Unsupervised Translation of Programming Languages

https://github.com/facebookresearch/CodeGen/blob/main/docs/transcoder.md

https://github.com/facebookresearch/CodeGen/blob/main/docs/transcoder.md#training

#### Facebook TransCoder-ST

Leveraging Automated Unit Tests for Unsupervised Code Translation

https://github.com/facebookresearch/CodeGen/blob/main/docs/TransCoder-ST.md

### machine learning autocompletion

autocompletion = extrapolation

https://www.kdnuggets.com/2021/07/github-copilot-open-source-alternatives-code-generation.html

> GitHub's Copilot code generation tool is currently only available via approved request. Here are 4 Copilot alternatives that you can use in your programming today.

#### GPT-3

https://en.wikipedia.org/wiki/GPT-3

> Generative Pre-trained Transformer 3 (GPT-3; stylized GPT·3) is an autoregressive language model that uses deep learning to produce human-like text. Given an initial text as prompt, it will produce text that continues the prompt.

= autocompletion

#### GPT-Code-Clippy (GPT-CC)
 
GPT-Code-Clippy is a code-generation tool which employs a GPT-3 model for generation.

https://github.com/ncoop57/gpt-code-clippy

> GPT-Code-Clippy (GPT-CC) is an open source version of GitHub Copilot, a language model -- based on GPT-3, called GPT-Codex -- that is fine-tuned on publicly available code from GitHub.

#### Second Mate
 
Second Mate is a code-generation tool for Emacs, leveraging a GPT model.

https://github.com/samrawal/emacs-secondmate

> An open-source, mini imitation of GitHub Copilot using EleutherAI GPT-Neo-2.7B (via Huggingface Model Hub) for Emacs.
>
> This is a much smaller model so will likely not be as effective as Copilot, but can still be interesting to play around with!


## bidirectional scalar transformations

### svelte

two way binding

## bidirectional array transformations

### bistring

Bidirectionally transformed strings

https://github.com/microsoft/bistring

> The bistring library provides non-destructive versions of common string processing operations like normalization, case folding, and find/replace. Each bistring remembers the original string, and how its substrings map to substrings of the modified version.

## bidirectional tree transformations

### ROSE compiler framework

a source-to-source compiler framework

written in C

http://www.rosecompiler.org/

https://en.wikipedia.org/wiki/ROSE_(compiler_framework)

https://github.com/rose-compiler/rose

https://github.com/rose-compiler/rose/wiki/How-to-create-a-translator

> Translator basically converts one AST to another version of AST. The translation process may add, delete, or modify the information stored in AST.

### DMS Software Reengineering Toolkit

a source-to-source compiler framework using explicit pattern-directed rewrite rules

closed source

https://en.wikipedia.org/wiki/DMS_Software_Reengineering_Toolkit

### showdown

A bidirectional Markdown to HTML to Markdown converter written in Javascript

https://github.com/showdownjs/showdown

### monocle

a bidirectional code generation library

https://news.ycombinator.com/item?id=31001922

https://blog.luitjes.it/posts/monocle-bidirectional-code-generation/

https://github.com/snootysoftware/prototypes/tree/main/monocle

> with lenses you generally define them through a DSL. Monocle lets you define them through example code. The goal was to make it as easy as possible for a decent programmer to write a lot of them

> back in the 90's it was called "round-tripping"
>
> https://www.ibm.com/docs/en/rhapsody/8.2?topic=developing-roundtripping-code

> https://en.wikipedia.org/wiki/Round-trip_engineering
> Round-trip engineering (RTE) is a functionality of software development tools that synchronizes two or more related software artifacts, such as, source code, models, configuration files, and even documentation.[1] The need for round-trip engineering arises when the same information is present in multiple artifacts and therefore an inconsistency may occur if not all artifacts are consistently updated to reflect a given change. For example, some piece of information was added to/changed in only one artifact and, as a result, it became missing in/inconsistent with the other artifacts.

> Source-to-source_compiler > See also > #ROSE, : https://en.wikipedia.org/wiki/Source-to-source_compiler

> several projects by builder.io have some overlap. Most notably [Mitosis][1], but I’d be shocked if [TS-Lite][2] isn’t using similar techniques. Potentially [Qwik][3] as well but I’m not sure, I would have bet that’s using Mitosis but it looks like that’s the other way around.
>
> [1]: https://github.com/BuilderIO/mitosis
>
> [2]: https://github.com/BuilderIO/ts-lite/tree/main/packages/core
>
> [3]: https://github.com/BuilderIO/qwik

> bidirectional code gen for no-code tools was our use case too (there's a demo video in the post if you're interested). I saw a bidirectional no-code platform called Vision X the other day, people are definitely working on it. Are the prototypes you worked on online somewhere? It sounds interesting!
>
> There are a bunch of ideas for dev tools in the original post. For example if you integrate with linters, you could define more complex code smells without all the AST juggling. Upgrading rails apps (or other frameworks that have a similarly well-defined structure) to new versions might work, by defining monocles for old the old and new version.

> A very popular Scala optics library is also called Monocle. I’ve been a happy user for a few years:
>
> https://github.com/optics-dev/Monocle

> For regular languages (not templating), if they have good tooling for converting to/from AST it's quite possible. The codebase isn't very flexible right now, but it's also not very big. In fact monocle itself is less than 900 lines of code.
I'm not sure if it makes sense for monocle to support multiple languages, or if each language should have its own port. Someone writing monocles in a specific language probably wants to do custom scripting in the language they're used to.
>
> Templating languages are trickier, because they usually don't have great tooling. In fact, we wrote our own tooling to convert from ERB to builder (a template system where you generate HTML through Ruby methods) and back. So for any templating language you would probably write a tool that converts from that language to builder, and back.
>
> On the other hand, ERB is about as free-form as it gets. Templating languages that are more strict are probably easier to add. For more info on how ERB is supported, I wrote another post that goes into detail: https://blog.luitjes.it/posts/erb2builder/

## lenses

https://news.ycombinator.com/item?id=31890781

### lenses in javascript

#### partial.lenses

https://github.com/calmm-js/partial.lenses

https://github.com/calmm-js/partial.lenses#transforms

https://www.npmjs.com/package/partial.lenses

Partial lenses is a comprehensive, high-performance optics library for JavaScript

> Lenses are basically an abstraction for simultaneously specifying operations to update and query immutable data structures. Lenses are highly composable and can be efficient. This library provides a rich collection of partial isomorphisms, lenses, and traversals, collectively known as optics, for manipulating JSON and users can write new optics for manipulating non-JSON objects, such as Immutable.js collections. A partial lens can view optional data, insert new data, update existing data and remove existing data and can, for example, provide defaults and maintain required data structure parts

#### jslens

Bidirectional transformation with lenses

https://github.com/vmx/jslens

> This is an implementation of lenses for the bidirectional transformation of strings. It's based on the dissertation "Bidirectional Programming Languages" by John Nathan Foster.

#### monocle-ts

Functional optics: a (partial) porting of Scala monocle

https://github.com/gcanti/monocle-ts

## unidirectional transfomers

### unidirectional tree transfomers

#### c2rust

Migrate C code to Rust

https://github.com/immunant/c2rust

#### unifiedjs

framework for abstract syntax tree (AST) transformations

https://github.com/unifiedjs/unified

#### putout

https://github.com/coderaiser/putout

Pluggable and configurable JavaScript Linter and code transformer with built-in ESLint and Babel support for js, jsx typescript, flow, markdown, yaml and json. Write declarative codemods in a simplest possible way

#### jscodeshift codemods

https://github.com/facebook/jscodeshift

#### typescript compiler

## multi target compilers

### haxe

compiles to

ActionScript3, JavaScript, Java, C++, C#, PHP, Python, Lua

### Cerberus X

compiles to

JavaScript, Java, C++, C#

## annotations

goal: lossless transformations

### sourcemaps

### magic comments

## keywords

* bidirectional
* bidirectional transpiler
* bidirectional compiler
* bidirectional source to source compiler
* symmetric
* optics
* lenses
* syncing
* synchronization
* dialog
* feedback
* source-to-source transformers
* source-to-source compilers
* program transformers
