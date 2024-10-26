# AWS::Personalize::Solution AlgorithmHyperParameterRanges<a name="aws-properties-personalize-solution-algorithmhyperparameterranges"></a>

Specifies the hyperparameters and their ranges\. Hyperparameters can be categorical, continuous, or integer\-valued\.

## Syntax<a name="aws-properties-personalize-solution-algorithmhyperparameterranges-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-personalize-solution-algorithmhyperparameterranges-syntax.json"></a>

```
{
  "[CategoricalHyperParameterRanges](#cfn-personalize-solution-algorithmhyperparameterranges-categoricalhyperparameterranges)" : [ CategoricalHyperParameterRange, ... ],
  "[ContinuousHyperParameterRanges](#cfn-personalize-solution-algorithmhyperparameterranges-continuoushyperparameterranges)" : [ ContinuousHyperParameterRange, ... ],
  "[IntegerHyperParameterRanges](#cfn-personalize-solution-algorithmhyperparameterranges-integerhyperparameterranges)" : [ IntegerHyperParameterRange, ... ]
}
```

### YAML<a name="aws-properties-personalize-solution-algorithmhyperparameterranges-syntax.yaml"></a>

```
  [CategoricalHyperParameterRanges](#cfn-personalize-solution-algorithmhyperparameterranges-categoricalhyperparameterranges): 
    - CategoricalHyperParameterRange
  [ContinuousHyperParameterRanges](#cfn-personalize-solution-algorithmhyperparameterranges-continuoushyperparameterranges): 
    - ContinuousHyperParameterRange
  [IntegerHyperParameterRanges](#cfn-personalize-solution-algorithmhyperparameterranges-integerhyperparameterranges): 
    - IntegerHyperParameterRange
```

## Properties<a name="aws-properties-personalize-solution-algorithmhyperparameterranges-properties"></a>

`CategoricalHyperParameterRanges`  <a name="cfn-personalize-solution-algorithmhyperparameterranges-categoricalhyperparameterranges"></a>
Provides the name and range of a categorical hyperparameter\.  
*Required*: No  
*Type*: List of [CategoricalHyperParameterRange](aws-properties-personalize-solution-categoricalhyperparameterrange.md)  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`ContinuousHyperParameterRanges`  <a name="cfn-personalize-solution-algorithmhyperparameterranges-continuoushyperparameterranges"></a>
Provides the name and range of a continuous hyperparameter\.  
*Required*: No  
*Type*: List of [ContinuousHyperParameterRange](aws-properties-personalize-solution-continuoushyperparameterrange.md)  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`IntegerHyperParameterRanges`  <a name="cfn-personalize-solution-algorithmhyperparameterranges-integerhyperparameterranges"></a>
Provides the name and range of an integer\-valued hyperparameter\.  
*Required*: No  
*Type*: List of [IntegerHyperParameterRange](aws-properties-personalize-solution-integerhyperparameterrange.md)  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)