# Radiotherapy quality evaluation using machine learning
Radiotherapy treatment is one of the most effective non-surgical cancer treatment modality. 
It uses external ionising radiotherapy to control or eliminate cancerous cells. 

The planning process for radiotherapy treatments consists of repeated plan optimization and 
plan evaluation. The planner needs to set some optimization parameters in a commercial treatment planning software  
in order to generate a plan. The plan is evaluated and the planner adjust the optimization 
parameters in order to improve the plan. The optimization process is time consuming and the effect of parameter
tuning is unknown a priori. Additionally, due to patient specific geometrical  
structural variations, evaluating the quality of a plan is difficult. 
As a consequences, the quality of the final treatment plan depends on the experience 
of a planner and the time used on planning.

![](images/plan-optimization-process.PNG)

In this work, we develop a data-driven plan evaluation tool using machine learning 
techniques. We build a classification model that predicts plan acceptability based 
on clinical evaluation criteria and geometrical features. The model results
are feed into a model interpreter which will show the strength and weaknesses 
of a given plan. The planner will be able to make informed evaluation on the treatment 
quality, hence saves time in the planning process and ensures the plan quality is 
satisfactory.

## Example of the plan evaluation output

![](images/explain-plan-quality.PNG)

The figure above is an annotated screen shot of the model interpreter for a plan. In this 
example we can see the classification score is less than 0.5, suggesting the plan is 
unsatisfactory. The bar plot shows the top criteria affecting the predicted plan 
quality. Criteria in red/green are the criteria contributing negatively/positively 
to plan quality. The planner can read from this plot to identify the strength and weaknesses 
of a given plan to make an informed evaluation on plan quality and improvement potential. 


