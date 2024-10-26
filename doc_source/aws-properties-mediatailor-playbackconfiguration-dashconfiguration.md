# AWS::MediaTailor::PlaybackConfiguration DashConfiguration<a name="aws-properties-mediatailor-playbackconfiguration-dashconfiguration"></a>

The configuration for DASH content\.

## Syntax<a name="aws-properties-mediatailor-playbackconfiguration-dashconfiguration-syntax"></a>

To declare this entity in your AWS CloudFormation template, use the following syntax:

### JSON<a name="aws-properties-mediatailor-playbackconfiguration-dashconfiguration-syntax.json"></a>

```
{
  "[ManifestEndpointPrefix](#cfn-mediatailor-playbackconfiguration-dashconfiguration-manifestendpointprefix)" : String,
  "[MpdLocation](#cfn-mediatailor-playbackconfiguration-dashconfiguration-mpdlocation)" : String,
  "[OriginManifestType](#cfn-mediatailor-playbackconfiguration-dashconfiguration-originmanifesttype)" : String
}
```

### YAML<a name="aws-properties-mediatailor-playbackconfiguration-dashconfiguration-syntax.yaml"></a>

```
  [ManifestEndpointPrefix](#cfn-mediatailor-playbackconfiguration-dashconfiguration-manifestendpointprefix): String
  [MpdLocation](#cfn-mediatailor-playbackconfiguration-dashconfiguration-mpdlocation): String
  [OriginManifestType](#cfn-mediatailor-playbackconfiguration-dashconfiguration-originmanifesttype): String
```

## Properties<a name="aws-properties-mediatailor-playbackconfiguration-dashconfiguration-properties"></a>

`ManifestEndpointPrefix`  <a name="cfn-mediatailor-playbackconfiguration-dashconfiguration-manifestendpointprefix"></a>
The URL generated by MediaTailor to initiate a playback session\. The session uses server\-side reporting\. This setting is ignored in PUT operations\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`MpdLocation`  <a name="cfn-mediatailor-playbackconfiguration-dashconfiguration-mpdlocation"></a>
The setting that controls whether MediaTailor includes the Location tag in DASH manifests\. MediaTailor populates the Location tag with the URL for manifest update requests, to be used by players that don't support sticky redirects\. Disable this if you have CDN routing rules set up for accessing MediaTailor manifests, and you are either using client\-side reporting or your players support sticky HTTP redirects\. Valid values are `DISABLED` and `EMT_DEFAULT`\. The `EMT_DEFAULT` setting enables the inclusion of the tag and is the default value\.  
*Required*: No  
*Type*: String  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)

`OriginManifestType`  <a name="cfn-mediatailor-playbackconfiguration-dashconfiguration-originmanifesttype"></a>
The setting that controls whether MediaTailor handles manifests from the origin server as multi\-period manifests or single\-period manifests\. If your origin server produces single\-period manifests, set this to `SINGLE_PERIOD`\. The default setting is `MULTI_PERIOD`\. For multi\-period manifests, omit this setting or set it to `MULTI_PERIOD`\.  
*Required*: No  
*Type*: String  
*Allowed values*: `MULTI_PERIOD | SINGLE_PERIOD`  
*Update requires*: [No interruption](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/using-cfn-updating-stacks-update-behaviors.html#update-no-interrupt)