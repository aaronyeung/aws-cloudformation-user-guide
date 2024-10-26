# AWS::QuickSight::Template SliderControlDisplayOptions<a name="aws-properties-quicksight-template-slidercontroldisplayoptions"></a>

The display options of a control\.

## Syntax<a name="aws-properties-quicksight-template-slidercontroldisplayoptions-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-quicksight-template-slidercontroldisplayoptions-syntax.json"></a>

```
{
  "[InfoIconLabelOptions](#cfn-quicksight-template-slidercontroldisplayoptions-infoiconlabeloptions)" : SheetControlInfoIconLabelOptions,
  "[TitleOptions](#cfn-quicksight-template-slidercontroldisplayoptions-titleoptions)" : LabelOptions
}
```

### YAML<a name="aws-properties-quicksight-template-slidercontroldisplayoptions-syntax.yaml"></a>

```
  [InfoIconLabelOptions](#cfn-quicksight-template-slidercontroldisplayoptions-infoiconlabeloptions): 
    SheetControlInfoIconLabelOptions
  [TitleOptions](#cfn-quicksight-template-slidercontroldisplayoptions-titleoptions): 
    LabelOptions
```

## Properties<a name="aws-properties-quicksight-template-slidercontroldisplayoptions-properties"></a>

`InfoIconLabelOptions`  <a name="cfn-quicksight-template-slidercontroldisplayoptions-infoiconlabeloptions"></a>
The configuration of info icon label options\.  
*Required*: No  
*Type*: [SheetControlInfoIconLabelOptions](aws-properties-quicksight-template-sheetcontrolinfoiconlabeloptions.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`TitleOptions`  <a name="cfn-quicksight-template-slidercontroldisplayoptions-titleoptions"></a>
The options to configure the title visibility, name, and font size\.  
*Required*: No  
*Type*: [LabelOptions](aws-properties-quicksight-template-labeloptions.md)  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)