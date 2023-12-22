+++
title = 'Artificial Intelligence'
date = 2023-10-21T20:28:09-05:00
draft = false
+++


I prefer the term "machine learning" which more accurately describes this technology, but artificial intelligence (AI) is what has caught on in the sensationalist news.  It's been either a theme or McGuffin in science fiction plots since William Grove's 1889 novel _Wreck of the World_.  AI in fiction is too often anthropomorphized as a competing species that facilitates the human apocalypse. Doomsday sells -- it's a lot more exciting than reality. 

I regularly use AI in my research.  Not transformers like ChatGPT, Bard or Claude that take 100 millions of tokens to train. Rather I employ feedforward and recurrent neural nets, random forests and autoencoders -- models that can be trained with the small datasets that I encounter in business research.  

AI takes datasets as inputs, and distills them into estimates or decisions.  This is basically what statistical decision models do, and indeed the language of AI borrows heavily from statistics.  The social science statistics of Pearson and Fisher employed numerous shortcuts to make hard calculation simple -- e.g.,     differential calculus optimization that linearized solutions under least-squares loss.  In the past decade, we've replaced calculus with massive computational power, and we can use any risk-minimization function we want.  We've innovated throughout the statistical framework with:	  

-- _Activation functions_ that define how signals from the data are propagated through the neural network

-- _Optimization procedures_ that replaced simple calculus minimization with clever search functions mainly based on gradient descent

-- _Risk / Loss functions_ beyond least squares, that allow us to perfectly engineer the focus of the decision.  These become especially involved in large language models (transformers) where subtle social biases must be engineered into the responses of AIs.

-- _Data curation_ has evolved to embrace non-quantitative data like text and images using methods like one-hot-encoding that have only been possible with massive computing power (though similar procedures have been explored since the 1940s, originally by I.J. Good using a multinomial-Dirichlet conjugate family)

AI studies have, I think, had a positive impact on the conduct of statistical analyses in the social sciences.  These have traditionally suffered from researcher "cherry picking" -- not the wholescale manufacturing of data seen in, for example, Francesca Gino's papers.  Rather the more subtle problem of running 20 analyses at 95% confidence with similar models to see which one fits the researchers particular biases and hypotheses.  This is a problem that plagues all of social science research, business topics included.  Machine learning, which has a tradition of datasets that are much larger than found in many social science studies, has adopted a requirement of cross-validation -- running models on subsets of data to see how stable are your estimates / decisions.  

Is AI "intelligent"?  Tell me what intelligence is, and I can give you an answer.  But, ask an _octopus_ what is intelligence, and he will say "the ability to use eight arms all at once."  The _dolphin_ will tell you it's the ability to "backflip in the ocean."  The rat, the ability to "discern faint smells in stereo."  This is why I dislike the term "AI." That term anthropomorphizes a useful tool in accordance with popular clichés -- we load it with self-absorbed biases on top of self-congratulatory praise and then conclude it's a threat to humanity.  You couldn't be more misleading.

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

Google produced the [original transformer paper from Google Brain](https://proceedings.neurips.cc/paper_files/paper/2017/file/3f5ee243547dee91fbd053c1c4a845aa-Paper.pdf)	that kicked off enthusiasm for large language models.  The models that produce such impressive output are complex and fiddly to run.


My own experience with AI models that have more than a few layers is that they require a lot of adjustment and "tuning" to work well.  I'm sure this is where Open.ai and Google Brain need hundreds of employees.  I used to have a computer with three NVIDIA graphics cards for about 30,000 computing cores dedicated to AI computing.  I would be lucky if I could ever use 10% of them in any particular machine learning model (I eventually dropped to just one card).  And the problems with getting models to produce interpretable output grows exponentially with their complexity.  I don't envy the programmers working on these large complex transformers.





