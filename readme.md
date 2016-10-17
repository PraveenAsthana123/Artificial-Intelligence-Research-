# AIR(Aritficial Intellgencne Research paper)

## Table of Contents
- [AIR (Aritficial Intellgencne Research paper)](#Aritficial intellegence research paper)
    - [Active Searches](#Active_searches)
        - [Active object search](#Active_object_search)
        - [LKP Manipulation based guided search](#LKP_Manipulation_based_guided_search)
    - [Bayes and ML](#Bayes_and_ML)
        - [Bayesian decision theory](#Bayesian_decision_theory)
        - [Chap9 Bayesian Mapping howie](#Chap9-Bayesian-Mapping_howie)
        - [Deconvolution](#Deconvolution)
        - [L2 for IP](#L2_for_IP)
        - [ML fundamentals](#ML_fundamentals)
        - [Maximum Likelihood Estimation](#MLE)
        - [Structure prediction optimization](#Structure_prediction_optimization)
    - [Deep Learning](#deap_learning)
        - [3D Conv](#3d_conv)
            - [3D_Conv_FB](#3D_Conv_FB)
            - [3D_Conv_NEC](#3D_Conv_NEC)
            - [3D_Conv_NEC_J](#3D_Conv_NEC_J)
        - Action Video Nets](#action_video_nets)
            - [Actions - Transformations](#Actions-Transformations)
            - [Liris-5228](#Liris-5228)
        - [Deep Learning book](#deep_learning_book)
            - [Convnets](#Convnets)
            - [RNNs](#RNNs)
        - [Lectures](#lectures)
            - [lec3 pdf](#lec3-pdf)
            - [lec3 ppt](#lec-ppt)
        - [Neural Nets](#neural-nets)
            - [MULTI_LAYER_PERCEPTRON](#MULTI_LAYER_PERCEPTRON)
            - [Neural Networks](#Neural_Networks)
        - [RCNNs](#rcnns)
            - [EECS-2014-180](#EECS-2014-180)
            - [RCNN_object_segmentation](#RCNN_object_segmentation)
            - [RCNN_Scene_parsing](#RCNN_Scene_parsing)
            - [RCNN_text_classification](#RCNN_text_classification)
            - [RCNN_Visual_recognition](#RCNN_Visual_recognition)
            - [W13-3214](#W13-3214)
        - [Binay weights NN](#binary_weights_nn)
        - [Deep learning](#deep_learning)
        - [preprint](#preprint)
        - [Recurrent Attention writer](#recurrent_attention_writer)



## <a name="Active_searches"></a> Active searches
### <a name="Active_object_search"></a>  Active object search ( [**link to file**](Active Searches/active object search.pdf) ) ( [Raavanan](https://github.com/raavanan) )

In this paper, we study the problem of active visual search (AVS) in large, unknown, or partially known environments.
We argue that by making use of uncertain semantics of the envi- ronment, a robot tasked with finding an object can devise
efficient search strategies that can locate everyday objects at the scale of an entire building floor, which is previously
unknown to the robot. To realize this, we present a probabilistic model of the search en- vironment, which allows for
prioritizing the search effort to those parts of the environment that are most promising for a specific object type. Further,
we describe a method for reasoning about the unexplored part of the environment for goal-directed exploration with
the purpose of object search. We demonstrate the validity of our approach by comparing it with two other search systems
in terms of search trajectory length and time. First, we implement a greedy coverage-based search strategy that is found
in previous work. Second, we let human participants search for objects as an alternative comparison for our method.
Our results show that AVS strategies that exploit uncertain semantics of the environment are a very promising idea,
and our method pushes the state-of-the-art forward in AVS.



### <a name="LKP_Manipulation_based_guided_search"></a> LKP Manipulation based guided search ( [**link to file**](Active Searches/LKP_Manipulation_based_guided_search.pdf) ) ( [Raavanan](https://github.com/raavanan) )

Object search is an integral part of daily life, and in the quest for competent mobile manipulation robots it is an unavoidable problem. Previous approaches focus on cases where objects are in unknown rooms but lying out in the open, which transforms object search into active visual search. However,in real life, objects may be in the back of cupboards occluded by other objects, instead of conveniently on a table by themselves. Extending search to occluded objects requires a more precise model and tighter integration with manipulation. We present a novel generative model for representing container contents by using object co-occurrence information and spatial constraints. Given a target object, a planner uses the model to guide an agent to explore containers where the target is likely, potentially needing to move occluding objects to enable further perception. We demonstrate the model on simulated domains and a detailed simulation involving a PR2 robot.

## <a name="Bayes_and_ML"></a> Bayes and ML
### <a name="Bayesian_decision_theory"></a> Bayesian decision theory ( [**link to file**](Bayes and ML/Bayesian_decision_theory.pdf) )

In the Bayesian(PROBABLITY Theory) framework, we assume that observable data x are generated by underlying hidden causes s
in the world, which cannot be observed directly. The generative model specifies how the data gets generated
from the causes, which is encapsulated in the conditional probability p(x|s), and any prior information about
the distribution over the different states of the causes p(s). In Bayesian decision making, a well-defined loss
function, indicating the potential loss incurred by each plausible cause-outcome pairing, is critical. Once
this loss function is specified, finding the optimal estimate consists of minimizing the expected loss, where
the expectation is taken over the posterior distribution over the variable of interest, taking into account any
uncertainty over the setting of the variable. Specifically, for the case of binary loss, we showed that the
optimal estimate is the MAP estimate (or mode), and the minimal expected loss is the probability that the
MAP estimate is incorrect. For the case of square loss, the optimal estimate is the expectation of the variable
under the posterior distribution, and the minimal expected loss the covariance of that distribution.

### <a name="Chap9-Bayesian-Mapping_howie"></a> Chap9 Bayesian Mapping howie ( [**link to file**](Bayes and ML/Chap9-Bayesian-Mapping_howie.pdf) )

This is not excatly a research paper, It's based on Robotics Intellegence (RI) and talks about the interrelation between Bayesian theory & Simulataneous Localization And Mapping.

### <a name="Deconvolution"></a> Deconvolution ( [**link to file**](Bayes and ML/Deconvolution.pdf) )

In this paper the blind deconvolution problem is formulated using the variational framework. With its use approximations of the involved probability distributions are developed resulting in two algorithms for the estimation of the posterior distributions of the hyperparameters, the blur, and the original image. The perfor- mance of the two proposed restoration algorithms is demonstrated experimentally.

### <a name="L2_for_IP"></a> L2 for IP ( [**link to file**](Bayes and ML/L2 for IP.pdf) )

Neural networks are becoming central in several areas of computer vision and image processing. Different archi- tectures have been proposed to solve specific problems. The impact of the loss layer of neural networks, however, has not received much attention by the research community: the default and most common choice is l2. This can be partic- ularly limiting in the context of image processing, since l2 correlates poorly with perceived image quality.
In this paper we bring attention to alternative choices. We study the performance of several losses, including perceptually-motivated losses, and propose a novel, differ- entiable error function. We show that the quality of the re- sults improves significantly with better loss functions, even for the same network architecture.

### <a name="ML_fundamentals"></a> ML fundamentals ( [**link to file**](Bayes and ML/ML_fundamentals.pdf) )

In this paper, we study the fundamentals of machine learning, various learning methods. Learning is a fundamental capability of neural networks. Learning rules are algo- rithms for finding suitable weights W and/or other network parameters. Learning of a neural network can be viewed as a nonlinear optimization problem for finding a set of network parameters that minimize the cost function for given examples. This kind of parameter estimation is also called a learning or training algorithm.

### <a name="MLE"></a> Maximum Likelihood Estimation ( [**link to file**](Bayes and ML/MLE.pdf) )

In this paper we Study Maximum Likelihood Estimation with various examples.

### <a name="Structure_prediction_optimization"></a> Structure prediction optimization ( [**link to file**](Bayes and ML/Structure_prediction_optimization.pdf) )

In this paper we develop an algorithm for structured predic- tion that optimizes against complex performance measures, those which are a function of false positive and false negative counts. The approach can be directly applied to performance measures such as Fβ score (natu- ral language processing), intersection over union (image segmentation), Precision/Recall at k (search engines) and ROC area (binary classifiers). We attack this optimization problem by approximating the loss function with a piecewise linear function and relaxing the obtained QP problem to a LP which we solve with an off-the-shelf LP solver. We present ex- periments on object class-specific segmentation and show significant im- provement over baseline approaches that either use simple loss functions or simple compatibility functions on VOC 2009.

People will be adding the abstract of the research papers so that you can directly access the research paper of your interest.
