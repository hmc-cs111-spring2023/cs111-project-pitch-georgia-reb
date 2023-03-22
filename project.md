# Project proposal

## The user and a language

This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?

_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help
them?_

I have been crocheting for a few years now, and as I have gotten more advanced, I have
run into a frustrating problem. When I am following a crochet pattern and I want to make
changes that are differnet to the pattern, it is difficult to keep track of these changes.
Additionally, when I have created my own crochet patterns, I have really struggled to
keep track of the steps that I have taken. Writing down the steps in my notes app, it gets
confusing very quickly!

These concerns made me think about the greater problems within crochet pattern creation. I
want to help people who are creating crochet patterns, or editing already existing patterns,
to have a smooth process in which they can create documents that contain crochet patterns.
Currently, someone creating a pattern must use a text editor, like Microsoft Word, that is
not created with crochet pattern creation in mind. Then, when someone purchases a crochet
pattern, they typically recieve a PDF. Because PDFs can't be directly edited by the user,
if someone wants to make changes to the crochet pattern, they must keep track of them in
their own notes. When this project comes in to help, someone creating a crochet pattern can
use my crochet markdown language to create beautiful PDF outputs of crochet patterns. This
markdown language will have built in features that enhance the PDF output and create
shortcuts for the crochet pattern writer. Additionally, I hope to add the ability to create
output in a variety of file formats. When the pattern writer publishes their pattern, they
can also upload the crochet markdown file. This means that when someone is using their pattern
and wants to make a slight change, they can download the markdown file and edit it. This
allows the user to easily edit the project with a crochet specific language, and then recompile
the output to a file format like a PDF.

### Why a language?

_Why is a DSL appropriate for your user(s)? How does it address the need?_

Writing a crochet pattern has a language of it's own, there are domain specific abbreviations,
required sections of a pattern, and each step aligns with a physical movement that the
crocheter must do with their yarn and crochet hook. A non-specifc text editor does not about
these domain specific aspects of crochet patterns, and therefore does not provide assistance
related to these attributes. A DSL is appropriate for crochet pattern writers because it will
allow them to have access to specific text editing components that will make writing crochet
patterns a more accessible and faster process.

### Why you?

_What excites you about this idea? How did you come up with it?_

Like I discussed in the first question, as I have gotten more advanced in my crochet skills
and crochet projects, I have run into problems when creating or changing crochet patterns. 
When I am following a crochet pattern and I want to make changes that are differnet to the
pattern, it is difficult to keep track of these changes. Additionally, when I have created
my own crochet patterns, I have really struggled to keep track of the steps that I have taken.

I came up with this idea because I would like there to exist an easy way to write up crochet
patterns, and I aleady have practical experience in this domain. I also think this project is
exciting because there is a pre-existing language within crochet, the crochet step 
abbreviations! It only makes sense to take this already well-defined domain, and create a helpful
DSL for it.

### Domain

_Describe the project's domain in five words._

Crochet pattern writing and editing.

### Interface (syntax)

_How might the user interact with the language? What does programming look
like? Why is this the right way to interact with the problem domain?_

The user would interact with the language by directly editing a file written in
the crochet markdown language. There would be documentation provided to the
user for them to understand the rules of this language and how it works. Then,
the user would compile this crochet markdown file to either a regular markdown
file, a PDF, or other file formats (scale will be determined as I make progress
on the project). Because the project domain is focused on creating crochet pattern
files, I think that the markdown format is the most logical format to follow as it
is an easy way to write information to be beautifully formatted for users to visualize.
Then, once this file is created, it can be converted to commonly used languages
and file formats like markdown and PDF files.

### Operation (semantics)

_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

When the program runs, a crochet markdown file is compiled into the desired output
format. This program can either successfully run, or fail with errors that will
help the user solve the problem. The users main way to interact with the program
is to go back an make edits, recompile the program, and look at the output to see
what changes they would like to make. This is the same as writing into a markdown
file like I am doing right now.

Potential errors would include if the user did not provide enough information for
the a specific section of the pattern to be created. For example, if someone includes
an image but the image file is missing, there would be an error. There might also be
warnings where the compilation completes, but the user is warned that important
sections of the crochet pattern are missing.

### Expressiveness

_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

In this language it should be easy to write clear and easy to read crochet patterns
that contain all of the important parts of a crochet pattern. It should also be
easy to recieve a crochet markdown file and then edit it to update the crochet pattern.

Because this is a markdown file, there are limits on one the user can do, so I can't
think of any aspects of the language that are possible but difficult to do.

It would be impossible to do any computation with the DSL, this is purely a program
for formatting crochet pattern documents.

### Related work

_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

Markdown already exists, and while it is specific to document creation, it is not
specific to crochet pattern writing.

There are crochet apps that help you work on a pattern, but I have not come across
any apps that help you create your own pattern. See [link](https://hearthookhome.com/best-free-crochet-apps/) for some existing
crochet apps. 

Additionally, there is crochet shorthand that is used descripting steps in crochet patterns.
In order to write a crochet pattern one uses this shorthand, but again there is no programming
language to writeup crochet patterns. I would like to use this shorthand in my crochet pattern
writeup language.

## The Project

This section examines whether the idea makes for a good CS 111 project.

### Suitability

_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

This project will be focused on writing a parser and a compiler. First, the crochet markdown
language must be parsed used the rules of the language that I create. Second, I will need
to write a compiler that will convert crochet markdown into a regular markdown file. From here,
I can either use something like [Pandoc](https://pandoc.org/) to convert to a PDF or many other
types of documents, or I can write my own additional compilers to other languages.

Based of off this plan, I don't expect for there to be any systems aspects of this project, I
will be heavily focusing on language design.

### Scope

_How big an idea is this? How ambitious is this project?_

I think this idea is a good size. By working on the parser and compiler to markdown, I will have
a good amount of work, but also a contained abount of work. From here, I can go back and add more
complicated features to the language, but this will only be done once I have the basic aspects
of the language completed. Then, I will also be able to work on creating output to additional formats,
which can be a small or larger amount of working depending on what approach I take.

### Benefits and drawbacks

_Why might this be a good idea for a project? Why might this not be a good idea
project?_

I have both enjoyed writing parsers and compilers, so this project focuses on two parts of writing
programming languages that I enjoy. Additionally, it is about a domain that I care about and am
already familiar with. This means that it will be easier for me to come up with practical and helpful
language design ideas. I also believe that this is a new project, and is not something that is already
accessible to people writing crochet patterns.

This project might not be easy for those new to crochet to understand, therefore it might be complicated
for both new users and my classmates to understand the details of.
