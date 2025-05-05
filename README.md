# p556-homework-3--bias-variance-decomposition-solved
**TO GET THIS SOLUTION VISIT:** [P556 Homework 3- Bias variance decomposition Solved](https://www.ankitcodinghub.com/product/p556-homework-3-bias-variance-decomposition-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;99627&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;0&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;0&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;0\/5 - (0 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;P556 Homework 3- Bias variance decomposition Solved&quot;,&quot;width&quot;:&quot;0&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 0px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            <span class="kksr-muted">Rate this product</span>
    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
Question 1: Bias Variance Decomposition (40 points)

Recall that the squared error can be decomposed into bias, variance and noise: E[(hD(x) − y)2] = E[(hD(x) − h ̄(x))2] + E[(h ̄(x) − y ̄(x))2] + E[(y ̄(x) − y(x))2]

􏰄 􏰃􏰂 􏰅􏰄 􏰃􏰂 􏰅􏰄 􏰃􏰂 􏰅􏰄 􏰃􏰂 􏰅

Error Variance Bias Noise

We will now create a data set for which we can approximately compute this decomposition. The function toydata.py generates a binary data set with class 1 and 2. Both are sampled from Gaussian distributions:

p(⃗x|y = 1) ∼ N(0,I) and p(⃗x|y = 2) ∼ N(μ2,I), (1) where μ2 = [2;2]⊤ (the global variable OFFSET=2 regulates these values: μ2 = [OFFSET ; OFFSET]⊤).

You will need to implement four functions: computeybar, computehbar, computevariance and biasvari- ancedemo.

(a) Noise (computeybar): First we focus on the noise. For this, you need to compute y ̄(⃗x) in computeybar. With the equations, p(⃗x|y = 1) ∼ N(0,I) and p(⃗x|y = 2) ∼ N(μ2,I), you can compute the probability p(⃗x|y). Then use Bayes rule to compute p(y|⃗x).

Hint: You may want to use the norm probability density function, which you can directly use some package to call this function if you find some. With the help of computeybar you can now compute the “noise” variable within biasvariancedemo. Here is a plot that what your data is supposed to be like in Figure 1:

Figure 1: Question 1

</div>
</div>
<div class="layoutArea">
<div class="column">
page 1 of 4

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
P556 Homework 3 October 13, 2021

</div>
</div>
<div class="layoutArea">
<div class="column">
(b) Bias (computehbar): For the bias, you will need h ̄. Although we cannot compute the expected value h ̄ = E[h], we can approximate it by training many hD and averaging their predictions. Edit the function computehbar: average over n models different hD, each trained on a different data set of n inputs drawn from the same distribution. Feel free to call toydata.py to obtain more data sets.

Hint: You can use ridge regression for hD. With the help of computehbar you can now compute the “bias” variable within biasvariancedemo.

(c) Variance (computevariance.py): Finally, to compute the variance, we need to compute the term E[(hD − h ̄)2]. Once again, we can approximate this term by averaging over n models models. Edit the file computevariance.

With the help of computevariance you can now compute the “variance” variable within biasvariancedemo.

(d) Demo (biasvariancedemo): In this function, you need to implement a plotting function that how the error decomposes (roughly) into bias, variance and noise when regularization constant λ increases. You can see the trend if you did everything correctly.

Hint: You can set a training dataset with a size of 500, for a really big dataset you can set the size as 100000. You can try average over 25 models. But all these parameters you can change freely.

The bigger number for the number of models and/or the training dataset, the better your approximation will be for E[h] and E[(hD − h ̄)2]).

If you get everything correct, you should get some plot like this:

Figure 2: Question 1

Question 2: SVM (30 points)

Here is an visualization of a set of 3600 points in 2D space (hw3 data2.txt).

• Which classifier would be able to achieve better performance on this distribution? Justify your choice. • Implement your chosen classifier and report your accuracy.

• Produce a plot that shows your final classifier as a dotted line, along with the original data points. You can make the plot either in the original space or feature space.

</div>
</div>
<div class="layoutArea">
<div class="column">
page 2 of 4

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
P556 Homework 3

</div>
<div class="column">
October 13, 2021

</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 3: Question 2

Question 3: Gaussian Processes and Hyper Parameter Tuning (40 points)

<ul>
<li>Show that the posterior distribution is P (y⋆|X⋆, X, y) = Ny⋆ (μ, Σ), where μ = k(X⋆, X)k(X, X)−1y and Σ = k(X⋆, X⋆) − k(X⋆, X)k(X, X)−1k(X, X⋆). Note: for this question, you may assume that the conditional distribution is of a Normal form, however you must derive the mean and variance. Note: It is not recommended to calculate the pdf of the posterior, which is a long and painful process. Hint: Useful reading material: Chapter 2 of Gaussian Processes for Machine Learning, Rasmussen and Williams (Available online at: http://www.gaussianprocess.org/gpml/chapters/)</li>
<li>Now for this problem, you will implement a basic Gaussian Progress Regression. We will be using the</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
standard radial basis kernel:

</div>
<div class="column">
􏰀−||xi −xj||2􏰁 K(xi,xj) = σexp 2h2

</div>
</div>
<div class="layoutArea">
<div class="column">
where σ, h are known as the scale and bandwith parameters.

So your implementation will be tested on the Concrete Compressive Strength dataset from the UCI repository (which is the data repository I announced before, but we will attach the dataset). The strength of concrete is predicted from 8 features consisting of the ingredients that make up the concrete composition and its age.

Hint:

<ul>
<li>– &nbsp;Implement [K] = RBF Kernel(X1, X2, sigma, h) which takes as input two matrices of examples X1 (n1× D),X2 (n2× D) with hyperparameters σ, h, and outputs the kernel matrix where Ki,j = k(X1i,X2j), where k is the RBF function described above.</li>
<li>– &nbsp;Implement [GPMean, GPVariance] = GPRegression(XTrain, yTrain, XTest, sigma, h) which carries out the Gaussian Process regression and returns the estimated mean and variances for the variables in XTest. See page 19 of chapter 2 in Rasmussen and Williams for help on making this computationally efficient and numerically stable.</li>
<li>– &nbsp;In this step, you need to find hyperparameters for the Gaussian Process. One reasonable method for Gaussian processes is to choose parameters that maximizes the log marginal likelihood. First implement [logml] = LogMarinalLikelihood(XTrain, yTrain, sigma, h) which computes the log marginal likelihood of the training data given the parameters.</li>
<li>– &nbsp;Implement [h, sigma] = HyperParameters(XTrain, yTrain, hs, sigmas), which does a grid search across the parameters in hs, sigmas and returns the combination that minimizes the log marginal likelihood (here you can just call the grid search function provided by Python).</li>
</ul>
</div>
</div>
<div class="layoutArea">
<div class="column">
page 3 of 4

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
P556 Homework 3 October 13, 2021

</div>
</div>
<div class="layoutArea">
<div class="column">
– Run your Gaussian process regression method on the dataset provided. Compare and report your results with a naive mean prediction. Get your hyperparameters by using your imple- mented HyperParameters functions and searching over the space of hs = logspace(-1,1,10)’⋆ norm(std(XTrain)) and sigmas = logspace(-1,1,10)’⋆ std(yTrain).

</div>
</div>
<div class="layoutArea">
<div class="column">
page 4 of 4

</div>
</div>
</div>
