# Emergence of Agile as Evolutionary Epistemology
Karl Popper describes Evolutionary Epistemology as acquisition of knowledge that improves upon previous ideas by refining them through the elimination of error. He expresses that through the formula:

PS<sub>1</sub> => TT<sub>1</sub> => EE<sub>1</sub> => PS<sub>2</sub>

We start with a problem situation PS<sub>1</sub>; tentative theories TT<sub>1</sub> are systematically subjected to attempts of falsification, and error elimination EE<sub>1</sub> selects the theories that best fit objectives over PS<sub>1</sub>. Their application leads to a different problem situation PS<sub>2</sub>, from which the cycle can start over. However, PS<sub>2</sub> is considered an ideal situation until new difficulties are identified.

In the publication titled [The New Methodology](https://martinfowler.com/articles/newMethodology.html), Manifesto for Agile Software Development signer Martin Fowler gives his account of what led him and his peers to devise and adopt agile practices. Due to the purpose of the text, his account leaves out the error elimination process, but we can identify all other elements in the emergence of agile practices.

In this account we can clearly identify the initial problem spaces, and Martin Fowler also identifies some of the difficulties found after the application of agile values and practices, thus indicating a new cycle of discoveries was or is needed. Due to his purpose in writing the article, he does not give an account of specific practices. But if Evolutionary Epistemology lies in the origin of agile practices, one should find support to this thesis and opposition to the antithesis when Fowler or other Manifesto signers talk about their origin or application. And this can be abundantly found in sources such as:

* [Scrum is simple, just use it as is!!](https://kenschwaber.wordpress.com/2017/11/11/scrum-is-simple-just-use-it-as-is/)
* [InfoQ Interview: Kent Beck on Agile Adoption & Values](https://www.infoq.com/articles/kent-beck-interview-2006)
* [Is TDD dead?](https://martinfowler.com/articles/is-tdd-dead/)
* [Agile is Dead](https://youtu.be/a-BOSpxYJ9M)

Thus we have confirmation that agile practices emerged and are correctly applied as a restatement of Popper’s model: a goal, a practice that achieves it, and verification that the goal was in fact achieved. One common criticism of failed adoption of agile practices is that practitioners lose sight of the goal and fail to achieve it by applying practices with no expected outcome.

>"Would you tell me, please, which way I ought to go from here?"

>"That depends a good deal on where you want to get to," said the Cat.

>"I don’t much care where—" said Alice.

>"Then it doesn’t matter which way you go," said the Cat.

>"—so long as I get somewhere," Alice added as an explanation.

>"Oh, you’re sure to do that," said the Cat, "if you only walk long enough."

>-- Alice in Wonderland, Chapter 6: Pig and Pepper

Clearly, every practice was devised with a goal in mind. One measured either objectively or subjectively, qualitatively or quantitatively, but a goal nonetheless. Which is the same as to say that one needs a valid theory to get from PS<sub>1</sub> to PS<sub>2</sub>.

## Error elimination as dialectics
In contemporary science and Popper’s Evolutionary Epistemology, error elimination is not a linear process. Falsification is in itself a dialectical process, for it relies on comparing the expected results of thesis and antithesis. In the previous section, we can see statements that reflect this same process, with agile practices for software development being created by deriving a falsification test from the goals at hand. Finding new processes can be summarized into a series of questions:

- What is our goal? What do we value? What do we want to achieve?
- What is the current practice (either intentional or incidental)?
- What are both the desirable and undesirable consequences of this practice?
- What new practice is proposed?
- How does it improve upon the current one? Is the value of its consequences higher than that of the current practice?

If we organize this into a dialectical model, we have all elements of Evolutionary Epistemology: an initial problem space, tentative theses (practices), a process of error elimination, and a resulting problem space.

While Sabherwal and Newman (2003) describe dialectics moved by personal or subjective interests (possibly inspired by evidence), we argue for one moved by realist evidence or, as Boghossian (2002) describes, applying the Socratic Method based on empirical evidence for the dynamics of interests. The objective is to refine the interests of parties involved in decision making by discovering objectives through socratic dialogue.

## Evolution of complexity

As Tentative Theories are selected, problems become more intricate. Sabherwal and Newman (2003) note that interests from different influencers conflict as new practices or solutions are proposed. This effect is illustrated by the discussion Is TTD Dead? already mentioned in this paper. The problem approached by the series of conversations is that a practice (replacing dependencies with mockups) addresses a number of issues in the problem space (such as feedback time and problem insulation) and at the same time creates other issues (usefulness of tests, effort required). That creates a multidimensional domain which an isolated set of practices and their goals alone does not approach. Involved parties may be influenced, due to their limited scope, by decision-making heuristics ([Kahneman, 2010](https://en.wikipedia.org/wiki/Thinking,_Fast_and_Slow)), to choose an approach that does not benefit them or other parties in the big picture.

A dialectic approach, on the other hand, being the set of propositions and their validation, may cover the full effect of changes -- as far as they are knowable. It is a framework upon which process change can be built. If the dialog that led to the adoption of a practice is recorded, i.e., the goals and how adopted practices are known to achieve them, and a practice change is proposed, the whole dialog can be processed again to check what issues the change solves and if new ones are introduced.

In a way, suggesting the persistence of the practice-emergence dialogue is analogous to regression test automation in that introducing a change to existing practices allows for the detection of what goals are affected even if they are not in the intended scope of the change.
