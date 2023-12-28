+++
title = 'Artificial Intelligence'
date = 2023-10-21T20:28:09-05:00
draft = false
+++


_Artificial intelligence_ you say?  I prefer the term "machine learning" which more accurately describes this technology.  But "artificial intelligence" or "AI" is what has caught the attention of the sensationalist press, and it's been either a theme or McGuffin in science fiction plots since William Grove's 1889 novel _Wreck of the World_.  AI in fiction is too often anthropomorphized as a competing species that facilitates the human apocalypse. Doomsday sells -- it's a lot more exciting than reality. 

Is AI "intelligent"?  Tell me what intelligence is, and I can give you an answer.  But, ask an _octopus_ what is intelligence, and he will say "the ability to use eight arms all at once."  The _dolphin_ will tell you it's the ability to "outsmart a shark."  The rat, the ability to "discern faint smells in stereo."  This is why I dislike the term "AI." That term anthropomorphizes a useful tool in accordance with popular clichés -- we load it with self-absorbed biases on top of self-congratulatory praise and then conclude it's a threat to humanity.  You couldn't be more misleading.

Here is what AI _is_ doing -- it takes datasets as inputs, and distills them into estimates or decisions.  This is basically what statistical decision models do, and indeed the language of AI borrows heavily from statistics.  The statistics of Pearson and Fisher employed numerous shortcuts to simplify difficult calculations -- e.g.,  differential calculus optimization that linearized solutions under least-squares loss.  In the past decade, we've augmented calculus with massive computational power and backpropagation that allows us to use any risk-minimization function we want.  AI innovates throughout the statistical framework with:	  

-- _Activation functions_ that define how signals from the data are propagated through the neural network

-- _Optimization procedures_ that replaces simple calculus minimization with backpropagation and clever gradient descent search 

-- _Risk / Loss functions_ beyond least squares, that allow us to tightly engineer the focus of the decision.  These become especially involved in large language models (e.g., transformers) where subtle social biases must be engineered into the responses of AIs and applied at various points in the model.

-- _Data curation_ has evolved to embrace non-quantitative data like text and images using methods like one-hot-encoding that have only been possible with massive computing power (though similar procedures have been explored since the 1940s, originally by I.J. Good using a Bayesian multinomial-Dirichlet conjugate family)

-- _Interpretation_ of the output of AI can be confusing, but data scientist are always inventing new ways to [make complex outcomes meaningful](https://christophm.github.io/interpretable-ml-book/) for the humans that must use them.

I think AI developments have had a positive impact on the conduct of statistical analyses in the social sciences.  These have traditionally suffered from researcher "cherry picking" -- not the wholescale manufacturing of data seen in, for example, Francesca Gino's papers.  Rather the more subtle problem of running 20 analyses at 95% confidence with similar models to see which one fits the researchers particular biases and hypotheses, or calling a correlation a cause.  This is a problem that plagues all of social science research, business topics included.  Machine learning, which has a tradition of datasets that are much larger than found in social science studies, has adopted a requirement of cross-validation -- running models on subsets of data to see how stable are your estimates / decisions.  

I regularly use AI in my research.  Not transformers like ChatGPT, Bard or Claude trained with 100 millions of tokens. Rather I employ feedforward and recurrent neural nets, random forests and autoencoders -- models that can be trained with the small datasets encountered in business research. 

That's not to say that transformers like ChatGPT aren't truly impressive.  Here is some rapping on my  beloved [10micron](https://www.10micron.com/en/homepage/) telescope mount, written by ChatGPT-4:


_(Verse 1)
Yo, gather 'round, let me tell y'all a tale,
'Bout the 10Micron mount, set to set sail,
In the cosmic ocean, where stars do gleam,
This mount's a dream machine, a stargazer's dream._

_It's precision and power, like a cosmic king,
Tracking stars and planets, doin' its thing,
With a whisper-quiet motor, it won't disturb your night,
10Micron's got your back, everything's right._

_(Chorus)
10Micron, the mount that's outta sight,
In the darkest of nights, it's your guiding light,
With precision and power, it'll take you far,
To explore the universe, like a shooting star._

_(Verse 2)
It's got that Italian design, sleek and so fine,
Built to last through space and time,
With precision to decimals, it's always on point,
10Micron's the mount that'll never disappoint._

_Equatorial tracking, with zero backlash,
It'll keep your telescope on the right cosmic track,
Whether you're into planets or deep-sky delight,
10Micron's got the moves to make your night._

_(Chorus)
10Micron, the mount that's outta sight,
In the darkest of nights, it's your guiding light,
With precision and power, it'll take you far,
To explore the universe, like a shooting star._

_(Verse 3)
From galaxies to nebulae, it's got you covered,
With programmable settings, your goals uncovered,
Capture breathtaking images, in colors so bold,
With the 10Micron mount, you'll never grow old._

_It's a tool for the pros, but beginners adore,
The way it makes stargazing an effortless chore,
So if you're reachin' for the stars, make no mistake,
With 10Micron, there's no limit to what you can make._

_(Chorus)
10Micron, the mount that's outta sight,
In the darkest of nights, it's your guiding light,
With precision and power, it'll take you far,
To explore the universe, like a shooting star._

_(Outro)
So here's to 10Micron, the mount we admire,
In the world of astronomy, it takes us higher,
With every constellation, every cosmic delight,
10Micron's our partner, in the endless starry night._


Google produced the [original transformer paper](https://proceedings.neurips.cc/paper_files/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf)	that kicked off current enthusiasm for large language models.  The models that produce such impressive output are complex and fiddly to run.  My own experience with AI models that have more than a few layers is that they require a lot of adjustment and "tuning" to work well.  I'm sure this is why Open.ai and Google Brain need hundreds of employees to develop and refine their models.  I used to have a computer with three NVIDIA graphics cards for about 30,000 computing cores dedicated to AI computing.  I would be lucky if I could ever use 10% of them in any particular machine learning model (I eventually dropped to just one card).  And the problems with getting models to produce interpretable output grow exponentially with their complexity.  I don't envy the programmers working on such large complex transformers.

Psychologist Frank Rosenblatt originated neural computing in the 1950s, and successfully tested ResNet models similar to modern transformers in the 1960s.  But influential computer scientists Marvin Minsky and Seymour Papert critiqued Rosenblatt's models leaving them to be ignored for five decades, while they moved the field towards decision trees.  Their research attracted massive investment, failed to provide results, and incited two decades of profound cynicism known as the "AI Winter."  Rediscoveries of Rosenblatt's neural models have dominated the field over the past decade, delivering substantial advances in image and language processing.  

I doubt that  AI's ultimate structure will be neural networks.  The tasks we are assigning them are ones that recreate the very human innovations of language and image interpretation, which depend on humans' five senses and the way the brain processes them.  Neural networks, by mimicking brain structure, are uniquely qualified to produce outputs that are similar to those from real humans (e.g., sentence completion and fake images). Neural network AIs may not be the best for problem solving or 'thinking' but they are really good at replicating behavior that humans call "intelligent."







