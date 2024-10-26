# AWS::EC2::SpotFleet SpotFleetRequestConfigData<a name="aws-properties-ec2-spotfleet-spotfleetrequestconfigdata"></a>

Specifies the configuration of a Spot Fleet request\. For more information, see [Spot Fleet ](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/spot-fleet.html) in the *Amazon EC2 User Guide*\.

You must specify either `LaunchSpecifications` or `LaunchTemplateConfigs`\.

## Syntax<a name="aws-properties-ec2-spotfleet-spotfleetrequestconfigdata-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-ec2-spotfleet-spotfleetrequestconfigdata-syntax.json"></a>

```
{
  "[AllocationStrategy](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-allocationstrategy)" : String,
  "[Context](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-context)" : String,
  "[ExcessCapacityTerminationPolicy](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-excesscapacityterminationpolicy)" : String,
  "[IamFleetRole](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-iamfleetrole)" : String,
  "[InstanceInterruptionBehavior](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-instanceinterruptionbehavior)" : String,
  "[InstancePoolsToUseCount](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-instancepoolstousecount)" : Integer,
  "[LaunchSpecifications](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-launchspecifications)" : [ SpotFleetLaunchSpecification, ... ],
  "[LaunchTemplateConfigs](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-launchtemplateconfigs)" : [ LaunchTemplateConfig, ... ],
  "[LoadBalancersConfig](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-loadbalancersconfig)" : LoadBalancersConfig,
  "[OnDemandAllocationStrategy](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-ondemandallocationstrategy)" : String,
  "[OnDemandMaxTotalPrice](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-ondemandmaxtotalprice)" : String,
  "[OnDemandTargetCapacity](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-ondemandtargetcapacity)" : Integer,
  "[ReplaceUnhealthyInstances](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-replaceunhealthyinstances)" : Boolean,
  "[SpotMaintenanceStrategies](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-spotmaintenancestrategies)" : SpotMaintenanceStrategies,
  "[SpotMaxTotalPrice](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-spotmaxtotalprice)" : String,
  "[SpotPrice](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-spotprice)" : String,
  "[TagSpecifications](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-tagspecifications)" : [ SpotFleetTagSpecification, ... ],
  "[TargetCapacity](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-targetcapacity)" : Integer,
  "[TargetCapacityUnitType](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-targetcapacityunittype)" : String,
  "[TerminateInstancesWithExpiration](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-terminateinstanceswithexpiration)" : Boolean,
  "[Type](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-type)" : String,
  "[ValidFrom](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-validfrom)" : String,
  "[ValidUntil](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-validuntil)" : String
}
```

### YAML<a name="aws-properties-ec2-spotfleet-spotfleetrequestconfigdata-syntax.yaml"></a>

```
  [AllocationStrategy](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-allocationstrategy): String
  [Context](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-context): String
  [ExcessCapacityTerminationPolicy](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-excesscapacityterminationpolicy): String
  [IamFleetRole](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-iamfleetrole): String
  [InstanceInterruptionBehavior](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-instanceinterruptionbehavior): String
  [InstancePoolsToUseCount](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-instancepoolstousecount): Integer
  [LaunchSpecifications](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-launchspecifications): 
    - SpotFleetLaunchSpecification
  [LaunchTemplateConfigs](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-launchtemplateconfigs): 
    - LaunchTemplateConfig
  [LoadBalancersConfig](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-loadbalancersconfig): 
    LoadBalancersConfig
  [OnDemandAllocationStrategy](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-ondemandallocationstrategy): String
  [OnDemandMaxTotalPrice](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-ondemandmaxtotalprice): String
  [OnDemandTargetCapacity](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-ondemandtargetcapacity): Integer
  [ReplaceUnhealthyInstances](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-replaceunhealthyinstances): Boolean
  [SpotMaintenanceStrategies](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-spotmaintenancestrategies): 
    SpotMaintenanceStrategies
  [SpotMaxTotalPrice](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-spotmaxtotalprice): String
  [SpotPrice](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-spotprice): String
  [TagSpecifications](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-tagspecifications): 
    - SpotFleetTagSpecification
  [TargetCapacity](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-targetcapacity): Integer
  [TargetCapacityUnitType](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-targetcapacityunittype): String
  [TerminateInstancesWithExpiration](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-terminateinstanceswithexpiration): Boolean
  [Type](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-type): String
  [ValidFrom](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-validfrom): String
  [ValidUntil](#cfn-ec2-spotfleet-spotfleetrequestconfigdata-validuntil): String
```

## Properties<a name="aws-properties-ec2-spotfleet-spotfleetrequestconfigdata-properties"></a>

`AllocationStrategy`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-allocationstrategy"></a>
The strategy that determines how to allocate the target Spot Instance capacity across the Spot Instance pools specified by the Spot Fleet launch configuration\. For more information, see [Allocation strategies for Spot Instances](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/spot-fleet-allocation-strategy.html) in the *Amazon EC2 User Guide*\.    
priceCapacityOptimized \(recommended\)  
Spot Fleet identifies the pools with the highest capacity availability for the number of instances that are launching\. This means that we will request Spot Instances from the pools that we believe have the lowest chance of interruption in the near term\. Spot Fleet then requests Spot Instances from the lowest priced of these pools\.  
capacityOptimized  
Spot Fleet identifies the pools with the highest capacity availability for the number of instances that are launching\. This means that we will request Spot Instances from the pools that we believe have the lowest chance of interruption in the near term\. To give certain instance types a higher chance of launching first, use `capacityOptimizedPrioritized`\. Set a priority for each instance type by using the `Priority` parameter for `LaunchTemplateOverrides`\. You can assign the same priority to different `LaunchTemplateOverrides`\. EC2 implements the priorities on a best\-effort basis, but optimizes for capacity first\. `capacityOptimizedPrioritized` is supported only if your Spot Fleet uses a launch template\. Note that if the `OnDemandAllocationStrategy` is set to `prioritized`, the same priority is applied when fulfilling On\-Demand capacity\.  
diversified  
Spot Fleet requests instances from all of the Spot Instance pools that you specify\.  
lowestPrice  
Spot Fleet requests instances from the lowest priced Spot Instance pool that has available capacity\. If the lowest priced pool doesn't have available capacity, the Spot Instances come from the next lowest priced pool that has available capacity\. If a pool runs out of capacity before fulfilling your desired capacity, Spot Fleet will continue to fulfill your request by drawing from the next lowest priced pool\. To ensure that your desired capacity is met, you might receive Spot Instances from several pools\. Because this strategy only considers instance price and not capacity availability, it might lead to high interruption rates\.
Default: `lowestPrice`   
*Required*: No  
*Type*: String  
*Allowed values*: `capacityOptimized | capacityOptimizedPrioritized | diversified | lowestPrice | priceCapacityOptimized`  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`Context`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-context"></a>
Reserved\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`ExcessCapacityTerminationPolicy`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-excesscapacityterminationpolicy"></a>
Indicates whether running Spot Instances should be terminated if you decrease the target capacity of the Spot Fleet request below the current size of the Spot Fleet\.  
Supported only for fleets of type `maintain`\.  
*Required*: No  
*Type*: String  
*Allowed values*: `default | noTermination`  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`IamFleetRole`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-iamfleetrole"></a>
The Amazon Resource Name \(ARN\) of an AWS Identity and Access Management \(IAM\) role that grants the Spot Fleet the permission to request, launch, terminate, and tag instances on your behalf\. For more information, see [Spot Fleet Prerequisites](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/spot-fleet-requests.html#spot-fleet-prerequisites) in the *Amazon EC2 User Guide for Linux Instances*\. Spot Fleet can terminate Spot Instances on your behalf when you cancel its Spot Fleet request or when the Spot Fleet request expires, if you set `TerminateInstancesWithExpiration`\.  
*Required*: Yes  
*Type*: String  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`InstanceInterruptionBehavior`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-instanceinterruptionbehavior"></a>
The behavior when a Spot Instance is interrupted\. The default is `terminate`\.  
*Required*: No  
*Type*: String  
*Allowed values*: `hibernate | stop | terminate`  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`InstancePoolsToUseCount`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-instancepoolstousecount"></a>
The number of Spot pools across which to allocate your target Spot capacity\. Valid only when Spot **AllocationStrategy** is set to `lowest-price`\. Spot Fleet selects the cheapest Spot pools and evenly allocates your target Spot capacity across the number of Spot pools that you specify\.  
Note that Spot Fleet attempts to draw Spot Instances from the number of pools that you specify on a best effort basis\. If a pool runs out of Spot capacity before fulfilling your target capacity, Spot Fleet will continue to fulfill your request by drawing from the next cheapest pool\. To ensure that your target capacity is met, you might receive Spot Instances from more than the number of pools that you specified\. Similarly, if most of the pools have no Spot capacity, you might receive your full target capacity from fewer than the number of pools that you specified\.  
*Required*: No  
*Type*: Integer  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`LaunchSpecifications`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-launchspecifications"></a>
The launch specifications for the Spot Fleet request\. If you specify `LaunchSpecifications`, you can't specify `LaunchTemplateConfigs`\.  
*Required*: Conditional  
*Type*: List of [SpotFleetLaunchSpecification](aws-properties-ec2-spotfleet-spotfleetlaunchspecification.md)  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`LaunchTemplateConfigs`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-launchtemplateconfigs"></a>
The launch template and overrides\. If you specify `LaunchTemplateConfigs`, you can't specify `LaunchSpecifications`\.  
*Required*: Conditional  
*Type*: List of [LaunchTemplateConfig](aws-properties-ec2-spotfleet-launchtemplateconfig.md)  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`LoadBalancersConfig`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-loadbalancersconfig"></a>
One or more Classic Load Balancers and target groups to attach to the Spot Fleet request\. Spot Fleet registers the running Spot Instances with the specified Classic Load Balancers and target groups\.  
With Network Load Balancers, Spot Fleet cannot register instances that have the following instance types: C1, CC1, CC2, CG1, CG2, CR1, CS1, G1, G2, HI1, HS1, M1, M2, M3, and T1\.  
*Required*: No  
*Type*: [LoadBalancersConfig](aws-properties-ec2-spotfleet-loadbalancersconfig.md)  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`OnDemandAllocationStrategy`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-ondemandallocationstrategy"></a>
The order of the launch template overrides to use in fulfilling On\-Demand capacity\. If you specify `lowestPrice`, Spot Fleet uses price to determine the order, launching the lowest price first\. If you specify `prioritized`, Spot Fleet uses the priority that you assign to each Spot Fleet launch template override, launching the highest priority first\. If you do not specify a value, Spot Fleet defaults to `lowestPrice`\.  
*Required*: No  
*Type*: String  
*Allowed values*: `lowestPrice | prioritized`  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`OnDemandMaxTotalPrice`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-ondemandmaxtotalprice"></a>
The maximum amount per hour for On\-Demand Instances that you're willing to pay\. You can use the `onDemandMaxTotalPrice` parameter, the `spotMaxTotalPrice` parameter, or both parameters to ensure that your fleet cost does not exceed your budget\. If you set a maximum price per hour for the On\-Demand Instances and Spot Instances in your request, Spot Fleet will launch instances until it reaches the maximum amount you're willing to pay\. When the maximum amount you're willing to pay is reached, the fleet stops launching instances even if it hasn’t met the target capacity\.  
If your fleet includes T instances that are configured as `unlimited`, and if their average CPU usage exceeds the baseline utilization, you will incur a charge for surplus credits\. The `onDemandMaxTotalPrice` does not account for surplus credits, and, if you use surplus credits, your final cost might be higher than what you specified for `onDemandMaxTotalPrice`\. For more information, see [Surplus credits can incur charges](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/burstable-performance-instances-unlimited-mode-concepts.html#unlimited-mode-surplus-credits) in the *EC2 User Guide*\.
*Required*: No  
*Type*: String  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`OnDemandTargetCapacity`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-ondemandtargetcapacity"></a>
The number of On\-Demand units to request\. You can choose to set the target capacity in terms of instances or a performance characteristic that is important to your application workload, such as vCPUs, memory, or I/O\. If the request type is `maintain`, you can specify a target capacity of 0 and add capacity later\.  
*Required*: No  
*Type*: Integer  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`ReplaceUnhealthyInstances`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-replaceunhealthyinstances"></a>
Indicates whether Spot Fleet should replace unhealthy instances\.  
*Required*: No  
*Type*: Boolean  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`SpotMaintenanceStrategies`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-spotmaintenancestrategies"></a>
The strategies for managing your Spot Instances that are at an elevated risk of being interrupted\.  
*Required*: No  
*Type*: [SpotMaintenanceStrategies](aws-properties-ec2-spotfleet-spotmaintenancestrategies.md)  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`SpotMaxTotalPrice`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-spotmaxtotalprice"></a>
The maximum amount per hour for Spot Instances that you're willing to pay\. You can use the `spotMaxTotalPrice` parameter, the `onDemandMaxTotalPrice` parameter, or both parameters to ensure that your fleet cost does not exceed your budget\. If you set a maximum price per hour for the On\-Demand Instances and Spot Instances in your request, Spot Fleet will launch instances until it reaches the maximum amount you're willing to pay\. When the maximum amount you're willing to pay is reached, the fleet stops launching instances even if it hasn’t met the target capacity\.  
If your fleet includes T instances that are configured as `unlimited`, and if their average CPU usage exceeds the baseline utilization, you will incur a charge for surplus credits\. The `spotMaxTotalPrice` does not account for surplus credits, and, if you use surplus credits, your final cost might be higher than what you specified for `spotMaxTotalPrice`\. For more information, see [Surplus credits can incur charges](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/burstable-performance-instances-unlimited-mode-concepts.html#unlimited-mode-surplus-credits) in the *EC2 User Guide*\.
*Required*: No  
*Type*: String  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`SpotPrice`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-spotprice"></a>
The maximum price per unit hour that you are willing to pay for a Spot Instance\. We do not recommend using this parameter because it can lead to increased interruptions\. If you do not specify this parameter, you will pay the current Spot price\.  
If you specify a maximum price, your instances will be interrupted more frequently than if you do not specify this parameter\.
*Required*: No  
*Type*: String  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`TagSpecifications`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-tagspecifications"></a>
The key\-value pair for tagging the Spot Fleet request on creation\. The value for `ResourceType` must be `spot-fleet-request`, otherwise the Spot Fleet request fails\. To tag instances at launch, specify the tags in the [launch template](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-launch-templates.html#create-launch-template) \(valid only if you use `LaunchTemplateConfigs`\) or in the ` [SpotFleetTagSpecification](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_SpotFleetTagSpecification.html) ` \(valid only if you use `LaunchSpecifications`\)\. For information about tagging after launch, see [Tag your resources](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/Using_Tags.html#tag-resources)\.  
*Required*: No  
*Type*: List of [SpotFleetTagSpecification](aws-properties-ec2-spotfleet-spotfleettagspecification.md)  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`TargetCapacity`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-targetcapacity"></a>
The number of units to request for the Spot Fleet\. You can choose to set the target capacity in terms of instances or a performance characteristic that is important to your application workload, such as vCPUs, memory, or I/O\. If the request type is `maintain`, you can specify a target capacity of 0 and add capacity later\.  
*Required*: Yes  
*Type*: Integer  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`TargetCapacityUnitType`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-targetcapacityunittype"></a>
The unit for the target capacity\. `TargetCapacityUnitType` can only be specified when `InstanceRequirements` is specified\.  
Default: `units` \(translates to number of instances\)  
*Required*: No  
*Type*: String  
*Allowed values*: `memory-mib | units | vcpu`  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`TerminateInstancesWithExpiration`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-terminateinstanceswithexpiration"></a>
Indicates whether running Spot Instances are terminated when the Spot Fleet request expires\.  
*Required*: No  
*Type*: Boolean  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`Type`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-type"></a>
The type of request\. Indicates whether the Spot Fleet only requests the target capacity or also attempts to maintain it\. When this value is `request`, the Spot Fleet only places the required requests\. It does not attempt to replenish Spot Instances if capacity is diminished, nor does it submit requests in alternative Spot pools if capacity is not available\. When this value is `maintain`, the Spot Fleet maintains the target capacity\. The Spot Fleet places the required requests to meet capacity and automatically replenishes any interrupted instances\. Default: `maintain`\. `instant` is listed but is not used by Spot Fleet\.  
*Required*: No  
*Type*: String  
*Allowed values*: `instant | maintain | request`  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`ValidFrom`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-validfrom"></a>
The start date and time of the request, in UTC format \(*YYYY*\-*MM*\-*DD*T*HH*:*MM*:*SS*Z\)\. By default, Amazon EC2 starts fulfilling the request immediately\.  
*Required*: No  
*Type*: String  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)

`ValidUntil`  <a name="cfn-ec2-spotfleet-spotfleetrequestconfigdata-validuntil"></a>
The end date and time of the request, in UTC format \(*YYYY*\-*MM*\-*DD*T*HH*:*MM*:*SS*Z\)\. After the end date and time, no new Spot Instance requests are placed or able to fulfill the request\. If no value is specified, the Spot Fleet request remains until you cancel it\.  
*Required*: No  
*Type*: String  
*Update requires*: [Replacement](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-replacement)