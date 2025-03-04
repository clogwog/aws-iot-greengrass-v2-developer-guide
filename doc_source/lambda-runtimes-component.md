# Lambda runtimes<a name="lambda-runtimes-component"></a>

The Lambda runtimes component \(`aws.greengrass.LambdaRuntimes`\) provides the runtimes that Greengrass core devices use to run AWS Lambda functions\.

**Note**  <a name="lambda-component-dependency-note"></a>
When you deploy a Lambda function component to a core device, the deployment also includes this component\. For more information, see [Run AWS Lambda functions](run-lambda-functions.md)\.

**Topics**
+ [Versions](#lambda-runtimes-component-versions)
+ [Type](#lambda-runtimes-component-type)
+ [Operating system](#lambda-runtimes-component-os-support)
+ [Requirements](#lambda-runtimes-component-requirements)
+ [Dependencies](#lambda-runtimes-component-dependencies)
+ [Configuration](#lambda-runtimes-component-configuration)
+ [Local log file](#lambda-runtimes-component-log-file)
+ [Changelog](#lambda-runtimes-component-changelog)

## Versions<a name="lambda-runtimes-component-versions"></a>

This component has the following versions:
+ 2\.0\.x

## Type<a name="lambda-runtimes-component-type"></a>

<a name="public-component-type-generic"></a>This <a name="public-component-type-generic-phrase"></a>component is a generic component \(`aws.greengrass.generic`\)\. The [Greengrass nucleus](greengrass-nucleus-component.md) runs the component's lifecycle scripts\.

<a name="public-component-type-more-information"></a>For more information, see [Component types](develop-greengrass-components.md#component-types)\.

## Operating system<a name="lambda-runtimes-component-os-support"></a>

This component can be installed on Linux core devices only\.

## Requirements<a name="lambda-runtimes-component-requirements"></a>

This component has the following requirements:
+ <a name="core-device-lambda-function-requirements"></a>Your core device must meet the requirements to run Lambda functions\. If you want the core device to run containerized Lambda functions, the device must meet the requirements to do so\. For more information, see [Lambda function requirements](setting-up.md#greengrass-v2-lambda-requirements)\.

## Dependencies<a name="lambda-runtimes-component-dependencies"></a>

This component doesn't have any dependencies\.

## Configuration<a name="lambda-runtimes-component-configuration"></a>

This component doesn't have any configuration parameters\.

## Local log file<a name="lambda-runtimes-component-log-file"></a>

This component doesn't output logs\.

## Changelog<a name="lambda-runtimes-component-changelog"></a>

The following table describes the changes in each version of the component\.


|  **Version**  |  **Changes**  | 
| --- | --- | 
|  2\.0\.8  |  Version updated for Greengrass nucleus version 2\.5\.0 release\.  | 
|  2\.0\.7  |  Version updated for Greengrass nucleus version 2\.4\.0 release\.  | 
|  2\.0\.6  |  Version updated for Greengrass nucleus version 2\.3\.0 release\.  | 
|  2\.0\.5  |  Version updated for Greengrass nucleus version 2\.2\.0 release\.  | 
|  2\.0\.4  |  Version updated for Greengrass nucleus version 2\.1\.0 release\.  | 
|  2\.0\.3  |  Initial version\.  | 