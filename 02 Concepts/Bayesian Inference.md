Build a model for expected probability distribution vs Build probability distribution for paramteres given data

Overarching idea is to update the prior given new data.  Balance the exposure to new data and the previous model, not drifting too far from either or just buying into one.
	Ex: if you think a coin is fair but you flipped it 3 times and got 3 heads you shouldn't automatically conclude p(heads) = 1.0, but you maybe should update the model

For neural network:

Weights are sampled from a distribution---you're learning distributions per paramter rather than a hard value. So the paramters you're optimizing for is the distribution.
	Means you need a KL divergence regularization term in order to prevent the distributions from drifting too far off a standard one.
	