# Interpretable Machine Learning:
## Intrinsic interpretable model
1. Linear Regression: 

 	<a href="https://www.codecogs.com/eqnedit.php?latex=\sum_{i&space;=&space;0}^{n}x_{i}\beta_{i}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\sum_{i&space;=&space;0}^{n}x_{i}\beta_{i}" title="\sum_{i = 0}^{n}x_{i}\beta_{i}" /></a>


2. Generalized linear regression:

<a href="https://www.codecogs.com/eqnedit.php?latex=g(E_Y(y|x))=\beta_0&plus;\beta_1{}x_{1}&plus;\ldots{}\beta_p{}x_{p}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?g(E_Y(y|x))=\beta_0&plus;\beta_1{}x_{1}&plus;\ldots{}\beta_p{}x_{p}" title="g(E_Y(y|x))=\beta_0+\beta_1{}x_{1}+\ldots{}\beta_p{}x_{p}" /></a>

	- Poisson regression
	- Negative binomial regression
  	- Beta regression
3. Generalized addictive model
	* Axiomatic Interpretability for Multiclass Additive Models (2019)
		- [Paper Link](https://arxiv.org/pdf/1810.09092.pdf)
		- [Source code](https://github.com/interpretml/interpret)
		- Generalize a state-of-the-art GAM learning algorithm based on boosted trees to the multiclass setting
		- Additive Post-Processing for Interpretability (API) that provably transforms a pretrained additive model to satisfy the interpretability axioms without sacrificing accuracy
		- Optimization procedure is cyclic gradient boosting
	* Intelligible Models for HealthCare: Predicting PneumoniaRisk and Hospital 30-day Readmission (2015) - [Link](http://people.dbmi.columbia.edu/noemie/papers/15kdd.pdf)
	* Purifying Interaction Effects with the Functional ANOVA: An Efficient Algorithm for Recovering Identifiable Additive Models (2019) - [Paper Link](https://arxiv.org/pdf/1911.04974.pdf)
	
	* An interpretable probabilistic machine learning method for heterogeneous longitudinal studies (2019):
		- [Paper Link](https://arxiv.org/pdf/1912.03549.pdf)
		- Present a widely applicable and interpretable probabilistic machine learning method for nonparametric longitudinal data analysis using additive Gaussian process regression.
		
4. Decision sets 
5. Rule-based classifiers 
6. Scorecards
7. Short rules 
8. Concept based explanation
9. TabNet: Attentive Interpretable Tabular Learning 
	* [Paper Link](https://arxiv.org/pdf/1908.07442.pdf)
	* [Source code](https://github.com/google-research/google-research/tree/master/tabnet)
	
12. Bayesian model:
	* INTERPRETABLE CLASSIFIERS USING RULES AND BAYESIANANALYSIS: BUILDING A BETTER STROKE PREDICTIONMODEL - [Link](https://arxiv.org/pdf/1511.01644.pdf)
	*  The Bayesian Case Model: A Generative Approachfor Case-Based Reasoning and Prototype Classification - [Link](https://beenkim.github.io/papers/KimRudinShahNIPS2014.pdf)
	

12. Right for the Right Reasons: Training Differentiable Models by Constraining their Explanations (2017)
13. Learning Explainable Models Using Attribution Priors (Gabriel Erion, Joseph D. Janizek, Pascal Sturmfels, Scott Lundberg, Su-In Lee,2019)
	* [Paper Link](https://arxiv.org/pdf/1906.10670.pdf)
	* [Source code](https://github.com/suinleelab/attributionpriors)
	* Model priors transfer information from humans to a model by constraining the model’s parameters
	* Model attributions transfer information from amodel to humans by explaining the model’s behavior. 


## Model-Specific Explanation Methods:
1. Knowledge distillation
2. Ensembles and Multiple Classifier Systems
3. Support Vector Machines
4. Deep learning

## Model-Agnostic:
1. Explanation by simplification:
	* Interpretability via Model Extraction 
		- [Paper Link](https://arxiv.org/abs/1706.09773):
		- The authors formulate model simplification as a model extraction process by approximating a transparent model to the complex one.

	* Distill-and-Compare: Auditing Black-Box Models Using Transparent Model Distillation - [Link](https://arxiv.org/abs/1710.06169)
	* Rule-based learner:
		- Interpretable & explorable approximations of black box models (2017)
		- Local interpretable model-agnostic explanations for music content analysis

	* Decision Tree:
		- Interpreting tree ensembles with intrees (2014)
		- Making Tree Ensembles Interpretable: A Bayesian Model Selection Approach (2017)
			* [Paper link](http://proceedings.mlr.press/v84/hara18a.html)
			* Presents the usage of two models (simple and complex) being the former the one in charge of interpretation and the latter of prediction by means of Expectation-Maximization and Kullback-Leibler divergence.
			* Given a complex tree ensemble, the author try to obtain the simplest representation that is essentially equivalent to the original one.
			* Derive a Bayesian model selection algorithm that optimizes the simplified model while maintaining the prediction performance
			* Adopt the probabilistic model for representing ensemble trees
			* Bayesian model selection algorithm called factorized asymptotic Bayesian (FAB) inference for finding the parameters.
2. Feature relevance explanation:
	* Understanding Black-box Predictions via Influence Functions - [Link](https://arxiv.org/pdf/1703.04730.pdf)
		- influence function is a measure of how strongly the model parameters or predictions depend on a training instance. Instead of deleting the instance, the method upweights the instance in the loss by a very small step. This method involves approximating the loss around the current model parameters using the gradient and Hessian matrix.
	* Game theory inspired: 
		- A unified approach to interpreting model predictions:
			+ [Source code](https://github.com/slundberg/shap)
			+ SHAP Tree explainer: which focuses on polynomial time fast SHAP value estimation specific for tree and ensemble tree
			+ SHAP Deep Explainer: is the high speed approximation SHAP value for deep learning model
		- An efficient explanation of individual classifications using game theory
		- Explaining models by propagating shapley values of local components (2019) 
	* Interpretation of nonlinear relationships between process variables by use of random forests

3. Local Explanations:
	* "Why Should I Trust You?": Explaining the Predictions of Any Classifier - [Link](https://arxiv.org/pdf/1602.04938.pdf)
	* Anchors: High-Precision Model-Agnostic Explanations (2018) - [Link](https://www.aaai.org/ocs/index.php/AAAI/AAAI18/paper/view/16982/15850)
	* Explaining Predictions from Tree-based Boosting Ensembles (2019)
	* Improving the Quality of Explanations with Local Embedding Perturbations

4. Example-based explantions
	* Counterfactual Explanations:
		- COUNTERFACTUAL EXPLANATIONS WITHOUT OPENING THE BLACK BOX: AUTOMATED DECISIONS AND THE GDPR - [Link](https://arxiv.org/ftp/arxiv/papers/1711/1711.00399.pdf)
		- Counterfactuals in explainable artificial intelligence (XAI): Evidence from human reasoning
	* Prototypes and Criticisms MMD-Critic:
		- Examples are not Enough, Learn to Criticize!Criticism for Interpretability - [Link](https://papers.nips.cc/paper/6300-examples-are-not-enough-learn-to-criticize-criticism-for-interpretability.pdf)
	* Learning functional causal models with generative neural networks, in: Explainable and Interpretable Models in Computer Vision and Machine Learning
	* Discovering causal signals in images


## Application:
1. Recommendation system
2. Ecnometrics
3. Natural language processing
4. Computer vision
5. Tabular Data

## Useful Links:
1. On Model Explainability [Link](https://everdark.github.io/k9/notebooks/ml/model_explain/model_explain.nb.html#7_explainable_boosting_machine)
