# Can Cucumber serve as the base API?

## Recap

We are working from the conclusion that there is an ontology to talk about continuous improvement. While this has not yet been established, there is also a hierarchy of ontologies so that when we talk about continous improvement we are also talking about testable hypotheses ([Karl Popper’s Critical Rationalism in Agile Software Development](https://www.researchgate.net/publication/221648881_Karl_Popper's_Critical_Rationalism_in_Agile_Software_Development)). In this whole endeavour, we need a tool to express any ontology using the critical rationalist approach.

Any improvement is the move from one state of affairs to another, from a tested hypothesis to a testable hypothesis with different or additional components. A hypothesis is a tentative explanation (cause and effect) for a set of observable facts. There are different ways of expressing a hypothesis, one of the most common being propositional logic. The language of propositional logic is long stablished and thus we know it works for expressing testable hypothesis. Continous improvement is a specialization of propositional logic, in that we need two hypotheses with the same initial conditions and different practices in order to bring about a desired fact.

The question at hand then is: is there a tool that can be used to express hypotheses? In [Dialogue as structured language](research/structured_dialogue.md), we suggest that such a tool is possible if we can express three or four terms through it: measurable facts, practices, and influences.

## Cucumber

Cucumber is a tool for automating functional tests -- which are the product of interactions between stakeholders. For our current purposes, focus only on the tool. It seems possible to express propositional logic in Gherkin (Cucumber's definition language):

```gherkin
Given [premise 1]
And [premise 2..N-1]
When [premise N]
Then [conclusion]
```

Premises in the form _all As are Bs_ are usually external to the tested hypothesis. For instance, if we had a hypothesis such as:

```gherkin
Given all mammals have body hair
And dogs are mammals
When a veterinarian inspects a dog
Then they will find body hair
```

The first premises are descriptives of no particular instance and thus not particularly measurable, though they are facts. We could summarize the hypothesis above to the last two particles and we would not lack any of the information we need to verify it.

```gherkin
Given the gravity on Earth
And in a vacuum chamber
When an object is thrown upwards with at a initial speed of 10m/s
Then it will reach a maximum height of 5.1m
```

In this hypothesis, there are several hidden premises, such as the laws of classical Mechanics. However, all declared premises are necessary to reach the conclusion. It would be silly to keep the first premise if there is no possibility of being on another planet, but let us assume that we could.

## Apply domain-specific language

It seems that Gherkin can be used to express hypotheses; the corollary is that we can use Cucumber to continually verify them. But what kind of hypotheses are we talking about? Well, let's take one simple example. We all know this never happens, but let's pretend that a given IT consulting company currently only provides manpower to customers ("body shop"). It ends up with no intellectual property rights (IPR) over anything it creates on behalf of customers, and thus no possibility of offering aggregated value to future customers. The underlying thesis here is:

```
Given P proposals
When N people are required
Then we can expect a profit margin of N * K
```

Where `K` is roughly the proportion between cost to the company and the billed man-hours. If we add value added by IPR, then we can reprhase this to something like this:

```
Given P proposals
When N people are required
And C components can be reused
Then we can expect a profit margin of N * K + Vc
```

Where `Vc` is the value added by the components (to which the company holds IPR) being reused. Notice that all of these are measurable facts. The number of proposals (or contracts), the number of people and their cost, the components that were (or are going to) reused, and profit margin are all numbers that can be retrieved, whether from tools or by interviewing people. We could break this into two thesis, one for proposals and one for delivered products. But let's focus on the means to automate this so that we can continuously measure the degree to which the thesis holds true:

The number of proposals (or contracts) can be verified through a tool -- database, web service, or web application. The number of people is an information in the contract. The number of components reused is limited by what is in the contract (if stated) and the number of available components. If something is not readily available through some electronic interaction, it can ultimately be asked of people through electronic forms, such as e-mail or Google Forms. Any electronic interaction (i.g. web applications) can be automated (e.g. SeleniumHQ).

The challenge becomes how to extract these theses (and hypotheses) from conversations with stakeholders (Cucumber will be in that conversation as well). For the time being, it seems that Cucumber can work as a base solution instead of creating a new one.