## Jeremy's comments (numbered); my initial responses (bulleted)

1. I'm not really clear on what it takes to argue for or against a distinction. The most natural interpretation is that a sufficient condition for a distinction is that two things are not necessarily identical (for every relevant sense of necessary). This is extremely weak and against it your arguments surely fail. So can we refine the claim that you are arguing against? Perhaps you are arguing that the distinction is not required (so there are approaches on which the distinction does not exist) and there are no arguments for the distinction, hence no arguments against those views.
  + **I agree and will change the dialectic to the more positive "What Shannon information really is"; give a definition that ties it to the measure of *surprisal* and then discuss the other measures (entropy, relative entropy, mutual information) in that light; the two misconceptions that are at the core of the paper will arise and be corrected in the process of giving the positive account.**
2. Discussion of first motivation mostly made sense to me. But 2.4 and 2.5 were clearly important but a bit messy. What exactly are your claims? What exactly is the role of teleosemantics in the argument? Surely, you are not supposing teleosemantics. But perhaps a premise that teleosemantics is a coherent and plausible theory is enough?
  + **The argument could work without teleosemantics but would simply be an appeal to how scientists (read: mathematicians and engineers) pretheoretically describe symbols as signifying the source states; teleosemantics provides the theory that justifies that pretheoretic talk and confirms for philosophers that these things really are representations. In light of this, it's not totally clear to me how to refine the dialectic in 2.4 and 2.5, though I admit they aren't as clean as the previous subsections in sec 2.**
3. Something isn't quite working in the way you are introducing surprisal and entropy. You want the primary definitions to be in terms of the number of symbols, but entropy is used to define the optimal code. I think probability distribution is still primary. If there is a way to do it without probability distribution as primary, that would be cool, but I don't think you have done that.
  + **Surprisal is the cost of a message given the best code *for the entire distribution*, so surprisal can't be justified as a useful measure without entropy.**
4. I don't think you have properly separated what is definitional of mutual information / channel capacity and what is the consequence of noisy channel theorem. I know we have talked about this before. Roughly, I think the definitional concept is the rate of success and error guessing symbol for symbol sent over a noisy channel. The theorem relates this to the minimal redundancy rate required to achieve arbitrarily good (i.e. approaching certain) reconstruction of code sent in arbitrarily large blocks. Turns out, the redundancy rate is the success rate. That was not obvious before the theorem. May have been that redundancy rate required would be infinite. E.g. suppose you improved your certainty simply by repeating symbols. Now redundancy required grows with log of how close to certain one is. (e.g. With r = 10% error on binary symbols, and repetition code, how many symbols required to get at least 1 - q = 99% certain reconstruction? We decode with majority rule so incorrect when at least n/2 symbols are flipped. Pr(at least n/2 symbols flipped) = (n choose n/2) \*r^(n/2) = (2r)^(n/2)  . Want this to be less than q. Take negative logs: So want n such that n/2 > -log(q)/-log(2r). \[Or something like that… you get the idea… redudancy required grows without bound with q for any r > 0. \] )
  + **Yep, in line with the changes to the dialectic I will be presenting mutual information earlier and with clearer reference to its role in the theorem.**
5. Though I am broadly sympathetic to your point of view. (Seems to me that semantic information could be composed out of appropriate correlations in the right distributions. I see no problem with that.)  I was pretty unconvinced by the discussion in 3.4.1-3.4.3.  I'm not sure what it takes to have a "concept" of anything… It seems like there is a definite sphere is ideas associated with Shannon (roughly, having thought about it for 3 seconds): functions of probability distributions that are additive for independent events. I'm interested in your applied communication theory interpretation of measures. But I don't think that we need to be constrained by those interpretations to "give sense" to the measures.
  + **I disagree with your final sentence, and that seems to be a point I need to address more directly.**

----

## Chat

Dialectic
+ I'm arguing that: the two most popular arguments that Shannon info and semantic info are different are fallacious.
+ Do I need to distinguish myself from Skyrms, Scarantino, Shea?
+ Two papers: (1) take down these two arguments. (2) my positive view.
  + It would be bad if my arguments against the two main arguments got confused because of the details of my positive view.

Teleo
+ It came out like: Shannon info and semantic info are equivalent in the central model.
+ Jeremy wasn't clear on the role of teleosemantics in the argument specifically. Don't necessarily throw it out, but clarify its role in the argument.
+ Put the comm theory people's quotes first.
+ Think of my opponent as believing: central model signals only get content when source messages have content.

Definition of "Shannon information"
+ cf "size" for bricks, hard drives, and populations
+ Jeremy agrees the people in section 3.4.1 ought to be precise. But it doesn't bother him as much as it bothers me.
+ Suppose someone says: "Shannon information is distinct from semantic information"; if you ask what they mean by Shannon information, they could say: "All of the equations you can list in information theory!"

Mutual info
+ (First line of argument) Clear away the Skyrms position early.
+ My (vague) idea: you can't appeal to the whole family and then say it's not legitimate to leverage it when talking about signalling, because some members of the family are specifically about signalling!
  + Jeremy: contra Shea, you're saying that the extra things you need are provided by communication theory! [exactly what Martinez.]
+ (Second line of argument) Jeremy: lots of people learn info theory outside the context of communication theory. So you need to motivate your idea.
  + My response: ubiquitous-ists can't object to comm-theory-semantic-type usage on the basis of ubiquity.
  + Jeremy: agree they can't shut the doors to using these equations, but also emphasise that something more is needed. You can then say that the "some more" is incredibly natural when you point out that's how it was originally applied.
  + Maybe pull more specific quotes about that stronger claim. 


Mutual info
+ ratio
+ log (make it additive)
+ averaging
  + you need to take the log if you're going to average it.

Jeremy: how the costs of inaccuracy are going to be paid informs your choice of inaccuracy measure.

Jeremy: be careful about the term optimal code. Surprisal: optimal source code. Noisy channel theorem: optimal channel code.

