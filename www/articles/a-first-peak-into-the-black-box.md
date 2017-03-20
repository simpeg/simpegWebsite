There are some funny expressions used for the geophysicists who do not know what they are doing, like "bump pickers" and "black box geophysicists." You know what I mean: open a proprietary software, load the data, tweak parameters, invert, and voila-a picture.

Not wanting to go down this road, I have made a point in my final year as an undergraduate to try to learn as much as I can about geophysics in a professional context. It is a clear goal, but not an easy one. University does a great job of providing a solid theoretical framework. We cover the necessities, but there is a gap between what goes on in academia and what happens in industry. It is surprising to see the disparity between what is discussed in lecture halls when compared to a technical talk or a conference. And many undergraduate geophysicists leave university lacking knowledge in areas that are fundamental to our trade: things like inversion, optimization theory, or even the basics of how to set up a survey and do field work. So I have been looking for ways to remedy the situation-to take a look inside the black box.

In short, there are aspects in our field of study that apply directly to our working lives that are not addressed with the focus they deserve. I am not saying this to be disparaging of the educational system. The problem is simple. Time is a finite resource, and there is a trade-off between how much material you can cover versus how well. It is a tough call to make. At one extreme you run the risk of not having a broad enough overview of a particular topic. At the other, you get hand-waving explanations and rabbit-out-of-the-hat derivations. Both can be frustrating. Moreover, as a particular field of research develops and expands, it becomes harder to prioritize what is essential. The upshot is that it is up to the student to decide what matters and to make it happen. After taking EOSC 350, a geophysics course for geologists and engineers I was offered the chance to take a short, 3 credit, directed studies to cover some of the basics of geophysical inversion at the UBC GIF. The goal was to produce a short series of learning modules that would help make the basics of inversion accessible to the average fourth year undergraduate. The following is not so much a summary of what the modules contain, but it is rather an expression of what I have learned, how I got there, and what I believe is necessary for success at the undergraduate level to train students for the future.


###A jump discontinuity on the learning curve


Finding the right resources for self-study proves to be a challenging task. Existing materials tend to be one of two end members. On the one hand there are resources tailored for the non-geophysicist. These are useful for getting a sense of some of main concepts, and they are excellent for providing engineers and other geoscientists with enough basic vocabulary to carry on a discussion with geophysicists, but they do not provide, to put it metaphorically, a key that fits the lock to the black box. On the other hand, there are resources for those already well-versed in the craft. These materials are useful in that they enable the practicing geophysicist to obtain deeper insight and refine his or her skills, but for the person looking to gain access to that level if understanding, they are largely inaccessible.


A common weakness in both cases is the tendency to gloss over key points: in the former situation it is done so as to not intimidate the reader, and in the latter case to not get bogged down in unnecessary detail. The result is a gap in available resources for the person in the middle, and it is a challenge to move from one state of knowledge to the other. That is not to say, however, that no good materials exist, but they have been hard to find. I have found a few sources of particular value that I feel are at the right level: John Scales *Introductory Geophysical Inverse Theory*, German A. Preito's *Geophysical Inverse Theory*, and a set of lecture notes by Randall M. Richardson and George Zandt from the University of Arizona: *Inverse Problems in Geophysics, GEOS 567*. From among these, in my opinion, Richardson and Zandt have made the text that my tutorials should have been, the only thing missing being a computational component. Their work is thorough, lucid, and self-contained.


###Prerequisite knowledge

In order to understand inversion basics, there is a certain amount of prerequisite knowledge required for the task. At the very least one needs a solid background in linear algebra and matrix calculus, some optimization, and statistics. Knowing that I lack certain areas of prerequisite knowledge meant that some side reading was necessary. That is, of course, a natural part of learning anything, but its downside is that it decreases the quantity of output per unit time.

The statistics that are employed in the modules are rudimentary: variance, normal and chi-squared distribution. And even there they are only touched upon and not discussed in any detail. Such a treatment of the topic is insufficient. Error estimation and noise (with all that it entails) is important. As MIT Professor Walter Lewin says in his first year physics lectures, repeatedly and emphatically: "Any-measurement that does not include an estimate of uncertainty is absolutely meaningless." Both Scales and Richardson offer chapters that cover the basics. Scales' discussion on determining the mass of a chunk of kryptonite is an excellent example of how to convey ideas in an accessible manner.

To derive the objective function, the properties of matrices and matrix differentiation are necessary. For this, again, Scales and Richardson do an adequate treatment, but also a short handout by Randal J. Barnes "Matrix Differentiation (and some other stuff)" provides an excellent summary. In a side module, now discarded from the final version, I used this handout significantly and made up some simple, pen-and-paper style examples to illustrate matrix properties.

Regarding optimization, there are several texts that do the topic justice, but for basic things like Tikhonov regularization, Prieto's short text helped enormously at clarifying concepts, and he discusses topics like the "smoothing norms," "fitting with tolerance" and the "L-curve" in a manner that has proven extremely helpful.

###A problem of choice

The decision of what should go into a set of tutorials is perhaps the most important one, and this is perhaps where I have had the most difficulty. If there is one area that I would have needed more clarification, it was here. This was originally to be a set of tutorials to showcase how to work with SimPEG, and in that light the tutorials are not successful by any measure. I sometimes felt a bit torn between what I thought should go into such a set of tutorials and what the stated goal of the exercise was to be.  As I was reading and working on things over the course of the semester, I would often query my peers in an attempt to gauge what they knew in order to see what would be needed. This lead to some interesting discussions and produced a great deal of meaningful insight. But the challenging part in this, however, was to try and balance what I thought should go into the work without going astray, and at a certain point I did.  I have since abandoned the material I was working on regarding mathematical foundations, and in the final version I have tried to reproduce as best as possible what was discussed during meetings and sessions.

And here is where I will not hide one reason for disappointment: it is only now, at the end of the exercise, where I feel I have gathered, read, and reviewed the available resources sufficiently where I could begin to produce a set of tutorials that could cover the mathematical, theoretical and practical aspects of basic inversion theory to a satisfactory degree.


###Things I have gained

I have recently been rereading papers and I am realizing that I have made progress. True, in many cases there are details that are still too advanced for my understanding, but I have reached a level of geophysical literacy that I did not possess before. As with language, with practice comes fluency, and that comes with effort and time. But I now understanding the majority of what I hear at technical talks, and papers that seemed impenetrable three months ago are now almost-but still just almost-within my grasp. And for this I am grateful.

###Things I have lost

As I mentioned in my introduction, the price to pay by taking a slow, thorough road means that there are many things that I had wanted to cover that I did not. I had plans to look at real data, go beyond a 1D example, and maybe delve into different geophysical surveys, particularly working with potential fields. In that respect the greatest thing I did not achieve in this session was acquire the computational know-how regarding methods to implement inversions effectively. It is one thing to make code work for a toy problem; making it work for real data is another matter entirely. This, I know, will be a challenge that I am faced with soon enough.  Another thing that I feel is lost is that many things that I have explored did not make the cut, so when reviewing the tutorials, I get the feeling that there is much left unsaid.

###Suggestions for the future

There are two things I would highly suggest.

First, I would design a short, web-based course in the mathematical foundations for geophysics. Most undergraduate geophysicists (myself included) do not possess enough background to approach geophysical inversion, and to be truthful, other topics in geophysics. The result is that we learn these subjects from a position of weakness rather than from a position of strength. The experience of the undergraduate is one of always playing catch up, and given time constraints, outside responsibilities, and other courses, we often fall into a pattern of "hoop-jumping" where we are compelled to do what is necessary to get by, and we miss the beauty that underlies much of what we do. One reason for this is that the mathematics courses that we take are largely for a general audience of geoscientists, engineers, physicists, and math majors. And while the courses themselves are very good in what they do, it would be a major step up if there were something tailored specifically to our needs.

It is difficult to grasp higher concepts when one is bogged down in the nitty gritty details of the maths. Moreover, I say, very specifically, it would be very handy to have a web-based short course for specific reasons. First, it circumvents an administrative hurdle that would involve wedging yet another course into a complex schedule, getting approval for such a course, having meetings about what content the course would contain, deciding who would teach it, and so on. Making an online, free, open-source course removes administrative hassles and does not tax an already tight schedule. Second, having a resource like this empowers the professor with an easy and immediate place to refer students to the background needed for a particular topic. If, say, professor x is teaching a particular topic that involves, for example, magnetic fields using spherical coordinates, then he or she could simply refer the students to a particular section of the web-based course if they are in need of a review of the topic (by the way, ask your geophysics undergraduates where the unit vectors in spherical coordinates lie, and you will be surprised at what you find). Third, there is a huge movement of free online materials offered by universities, from Stanford to MIT to smaller colleges. These have been an integral part of my learning over the past five years, and it only seems natural that UBC geophysics would be part of that community.

In a similar vein, I would create a clean, expanded version of Doug's EOSC 454 course materials for public use. The course notes are very good, and a good part of Module 2 is lifted from the "Discretization 2.0" notes. There are two things that I would do with them: (1) transfer the existing notes from hand written to a clean, typed LaTeX version, and (2) expand them with some explanation. These are designed as a complement to a lecture component, and in that regard they are sufficient. But the set of notes is not quite a standalone document. Work could be done to render them into a self-contained set of approximately 100-150 pages, which would make an excellent booklet. With the benefit of hindsight, this alone would have made an excellent directed studies project for me, but the idea came to me shortly after reading week and I did not want to propose a change of tack half way through the term. That said, this may also be a great directed studies project for a future student.

###Final thoughts

I am extremely grateful for what I have learned over the course of this semester, and for the time that was taken by members of the UBC GIF to guide me, answer questions, and prepare materials. This one semester course has been a challenging but positive experience. And although I do not think that these modules are in a state ready for general use, the exercise of doing the background work and building them has helped me gain valuable new knowledge.

###Resources for Further Reading

Check out my tutorials on GitHub:
[Beginner Geophysics Tutorials](http://nbviewer.ipython.org/github/jokulhaup/directed_studies/tree/master/Final%20Drafts/)

In addition to the Inversion for Applied Geophysics Website and Inversion for Applied Geophysics: A Tutorial, here are links to materials for learning inverse theory that I feel are worth sharing.


1. [Inverse Problems in Geophysics](http://www.physics.arizona.edu/~restrepo/577/Richardsons.pdf) lecture notes by Randall M. Richardson and George Zandt from the University of Arizona
2. [Introductory Geophysical Inverse Theory](http://mesoscopic.mines.edu/~jscales/gp605/snapshot.pdf) by John Scales et. al is another short booklet that does a fair beginner treatment of the topic
3. [Geophysical Inverse Theory](http://wwwprof.uniandes.edu.co/~gprieto/classes/compufis/inverse/inverse_theory.pdf), a short, 50 page set of notes by George A. Prieto
4. [Matrix Differentiation](http://www.atmos.washington.edu/~dennis/MatrixCalculus.pdf), a short handout by Randal J. Barnes