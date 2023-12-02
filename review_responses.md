# Review-1

## Section 3.1, "we use two distinct target sets to effectively identify and separate biased comments into two distinct extremes". More details related to target sets should be provided.
Well we did explain what we meant by target sets in 3.1 (with example) and this time i also labelled what target sets are being used in each and every experiment so they can understand what type of target sets are used according to the situation and classification, so i don't understand how more can we possibly explain this topic.

## In Section 4, "Through extensive experimentation on various datasets, we consistently observed a significant trend." "As illustrated in Figure 3, by experimenting with a few datasets" The datasets used in the experiments should be given explicitly.
This is my fault, i thought since this was not under the experiment section i do not have to provide dataset information

## In Section 4, an illustration of the whole process of the statistical approach should be added to give a holistic view and connect all the modules mentioned (i.e. equations) used to do the modeling.
I never thought of doing this before but this is a great idea, i could create a flow chart explaining how the whole process actually works

## For the experiments in Section 4 and Section 5, more implementation details like specific settings and parameters should be provided. 
I'm not sure what they want us to share here, i've already mentioned earlier in the paper we are using the default version of bert without using any additional parameters, the target sets are the only depending factors here that we have shared and labelled. Perhaps we are meant to share the value of thresholds, or mention that we are using 90% functionality.

## The index number of Figure 13 should be corrected.
Latex Error, my mistake

## For Table 1, the title of the table should be at the top of the table.
Error, my mistake

## The references must be right. e.x.[13] Vaswani,A.,Shazeer,N.,Parmar,N.,Uszkoreit,J.,Jones,L.,Gomez,A.N., Kaiser, L., and Polosukhin, I. Attention is all you need, 2023?
I will have to check the BibTex again for this, i don't remember about this, although it is incomplete here

# Review 2

## While extending existing concepts, the paper's ideas lack significant innovation. Elements like the definition of biased words and the use of BERT are well-established in the field.
It is true, we have failed to introduce anything new in the field of NLP, but it shouldn't mean we cannot use existing technolgies or definitions to make something that hasn't been proposed yet.

## The proposed statistical analysis may be overly simplistic and generic, undermining the model's originality and depth.
Perhaps, the model is still too naive than it should be, i think if we were use the help of deep learning techniques we can introduce some back bone in our classification process. So either we can mix some other unsupervised learning techniques, or we either try to bayesian optimization algorithms to optimize selction of t1 and t2?

## There are notable gaps, including the absence of performance comparisons with state-of-the-art methods and the need for an ablation study. These comparisons and analyses are crucial for understanding the model's strengths and limitations.
Yeah i had a though this would be a problem, I really had no time due to my Mid semester examinations, otherwise i would have been able to produce an in-depth code's execution time comparison between our model and other standard models.

# Review-3

## 'For example, if we observe that these bias values follow a normal distribution, this suggests that biased words are rare, while neutral words make up the majority of the population.' This is not true. If the values follow a normal distribution with high variance, then biased words might be very common.
This is my mistake, I failed to mention that in the presence of high-variance the curve would be very short and this trend would not take place.

## Regarding the results, some need to be validated properly. For instance, it is not mentioned in the paper if some manual inspection was conducted for the sample points shown in Figure 13. Is the bias coherent with the content of the text? In addition, the results vary greatly among each subsection of Section 5. For instance, no classification results are presented for Section 5.1.4.
The data was unlabelled, we did an unsupervised learning to classify a dataset of news categories, so that we can filter sports news from the crime related news, that was it. The table is there as a proof that the model works

## My thoughts
I think most people are failing to understand the important point of this model, which is that it is supposed to work on any given unlabelled data, it is an unsupervised approach to classify sentences, but we have FAILED to imphasize on this in the paper...Other than that the model is just close enough to a Naive Bayes classifier and it needs more work to beat that.