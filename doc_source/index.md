# AWS IoT Greengrass Developer Guide, Version 2

-----
*****Copyright &copy; Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in 
     connection with any product or service that is not Amazon's, 
     in any manner that is likely to cause confusion among customers, 
     or in any manner that disparages or discredits Amazon. All other 
     trademarks not owned by Amazon are the property of their respective
     owners, who may or may not be affiliated with, connected to, or 
     sponsored by Amazon.

-----
## Contents
+ [What is AWS IoT Greengrass?](what-is-iot-greengrass.md)
   + [How AWS IoT Greengrass works](how-it-works.md)
   + [Greengrass feature compatibility by operating system](operating-system-feature-support-matrix.md)
   + [Move from AWS IoT Greengrass Version 1](move-from-v1.md)
   + [What's new in AWS IoT Greengrass Version 2](greengrass-v2-whats-new.md)
      + [Release: AWS IoT Greengrass Core v2.5.0 software update on November 12, 2021](greengrass-release-2021-11-12.md)
      + [Release: AWS IoT Greengrass Core v2.4.0 software update on August 3, 2021](greengrass-release-2021-08-03.md)
      + [Release: AWS IoT Greengrass Core v2.3.0 software update on June 29, 2021](greengrass-release-2021-06-29.md)
      + [Release: AWS IoT Greengrass Core v2.2.0 software update on June 18, 2021](greengrass-release-2021-06-18.md)
      + [Release: AWS IoT Greengrass Core v2.1.0 software update on April 26, 2021](greengrass-release-2021-04-26.md)
      + [Release: AWS IoT Greengrass Core v2.0.5 software update on March 09, 2021](greengrass-release-2021-03-09.md)
      + [Release: AWS IoT Greengrass Core v2.0.4 software update on February 04, 2021](greengrass-release-2021-02-04.md)
+ [Getting started with AWS IoT Greengrass V2](getting-started.md)
+ [Setting up AWS IoT Greengrass core devices](setting-up.md)
   + [Install the AWS IoT Greengrass Core software](install-greengrass-core-v2.md)
      + [Install AWS IoT Greengrass Core software with automatic resource provisioning](quick-installation.md)
      + [Install AWS IoT Greengrass Core software with manual resource provisioning](manual-installation.md)
      + [Install AWS IoT Greengrass Core software with AWS IoT fleet provisioning](fleet-provisioning.md)
         + [Set up AWS IoT fleet provisioning for Greengrass core devices](fleet-provisioning-setup.md)
         + [Configure the AWS IoT fleet provisioning plugin](fleet-provisioning-configuration.md)
      + [Install AWS IoT Greengrass Core software with custom resource provisioning](custom-provisioning.md)
         + [Develop custom provisioning plugins](develop-custom-provisioning-plugins.md)
      + [Installer arguments](configure-installer.md)
   + [Run the AWS IoT Greengrass Core software](run-greengrass-core-v2.md)
   + [Run AWS IoT Greengrass Core software in a Docker container](run-greengrass-docker.md)
      + [Build the AWS IoT Greengrass container image from a Dockerfile](build-greengrass-dockerfile.md)
      + [Run AWS IoT Greengrass in a Docker container with automatic resource provisioning](run-greengrass-docker-automatic-provisioning.md)
      + [Run AWS IoT Greengrass in a Docker container with manual resource provisioning](run-greengrass-docker-manual-provisioning.md)
      + [Troubleshooting AWS IoT Greengrass in a Docker container](docker-troubleshooting.md)
   + [Configure the AWS IoT Greengrass Core software](configure-greengrass-core-v2.md)
   + [Update the AWS IoT Greengrass Core software (OTA)](update-greengrass-core-v2.md)
   + [Uninstall the AWS IoT Greengrass Core software](uninstall-greengrass-core-v2.md)
+ [AWS-provided components](public-components.md)
   + [Greengrass nucleus](greengrass-nucleus-component.md)
   + [Client device auth](client-device-auth-component.md)
   + [CloudWatch metrics](cloudwatch-metrics-component.md)
   + [Docker application manager](docker-application-manager-component.md)
   + [Greengrass CLI](greengrass-cli-component.md)
   + [AWS IoT Device Defender](device-defender-component.md)
   + [IP detector](ip-detector-component.md)
   + [Kinesis Data Firehose](kinesis-firehose-component.md)
   + [Lambda launcher](lambda-launcher-component.md)
   + [Lambda manager](lambda-manager-component.md)
   + [Lambda runtimes](lambda-runtimes-component.md)
   + [Legacy subscription router](legacy-subscription-router-component.md)
   + [Local debug console](local-debug-console-component.md)
   + [Log manager](log-manager-component.md)
   + [Machine learning components](machine-learning-components.md)
      + [SageMaker Edge Manager](sagemaker-edge-manager-component.md)
      + [DLR image classification](dlr-image-classification-component.md)
      + [DLR object detection](dlr-object-detection-component.md)
      + [DLR image classification model store](dlr-image-classification-model-store-component.md)
      + [DLR object detection model store](dlr-object-detection-model-store-component.md)
      + [DLR installer](dlr-component.md)
      + [TensorFlow Lite image classification](tensorflow-lite-image-classification-component.md)
      + [TensorFlow Lite object detection](tensorflow-lite-object-detection-component.md)
      + [TensorFlow Lite image classification model store](tensorflow-lite-image-classification-model-store-component.md)
      + [TensorFlow Lite object detection model store](tensorflow-lite-object-detection-model-store-component.md)
      + [TensorFlow Lite installer](tensorflow-lite-component.md)
   + [Modbus-RTU protocol adapter](modbus-rtu-protocol-adapter-component.md)
   + [MQTT bridge](mqtt-bridge-component.md)
   + [MQTT broker (Moquette)](mqtt-broker-moquette-component.md)
   + [Nucleus telemetry emitter](nucleus-emitter-component.md)
   + [Secret manager](secret-manager-component.md)
   + [Secure tunneling](secure-tunneling-component.md)
   + [Shadow manager](shadow-manager-component.md)
   + [Amazon SNS](sns-component.md)
   + [Stream manager](stream-manager-component.md)
   + [Token exchange service](token-exchange-service-component.md)
   + [IoT SiteWise OPC-UA collector](iotsitewise-opcua-collector-component.md)
   + [IoT SiteWise publisher](iotsitewise-publisher-component.md)
   + [IoT SiteWise processor](iotsitewise-processor-component.md)
+ [Develop AWS IoT Greengrass components](develop-greengrass-components.md)
   + [Create local AWS IoT Greengrass components](create-components.md)
   + [Test AWS IoT Greengrass components with local deployments](test-components.md)
   + [Upload components to deploy to your core devices](upload-components.md)
   + [Interact with AWS services](interact-with-aws-services.md)
   + [Run a Docker container](run-docker-container.md)
   + [AWS IoT Greengrass component recipe reference](component-recipe-reference.md)
   + [Component environment variable reference](component-environment-variables.md)
+ [Deploy AWS IoT Greengrass components to devices](manage-deployments.md)
   + [Create deployments](create-deployments.md)
      + [Update component configurations](update-component-configurations.md)
   + [Revise deployments](revise-deployments.md)
   + [Cancel deployments](cancel-deployments.md)
   + [Check deployment status](check-deployment-status.md)
+ [Logging and monitoring in AWS IoT Greengrass](logging-and-monitoring.md)
   + [Monitor AWS IoT Greengrass logs](monitor-logs.md)
   + [Log AWS IoT Greengrass V2 API calls with AWS CloudTrail](logging-using-cloudtrail.md)
   + [Gather system health telemetry data from AWS IoT Greengrass core devices](telemetry.md)
   + [Check Greengrass core device status](device-status.md)
+ [Run AWS Lambda functions](run-lambda-functions.md)
   + [Import a Lambda function as a component (console)](import-lambda-function-console.md)
   + [Import a Lambda function as a component (AWS CLI)](import-lambda-function-cli.md)
+ [Use the AWS IoT Device SDK to communicate with the Greengrass nucleus, other components, and AWS IoT Core](interprocess-communication.md)
   + [Publish/subscribe local messages](ipc-publish-subscribe.md)
   + [Publish/subscribe AWS IoT Core MQTT messages](ipc-iot-core-mqtt.md)
   + [Interact with component lifecycle](ipc-component-lifecycle.md)
   + [Interact with component configuration](ipc-component-configuration.md)
   + [Retrieve secret values](ipc-secret-manager.md)
   + [Interact with local shadows](ipc-local-shadows.md)
+ [Interact with local IoT devices](interact-with-local-iot-devices.md)
   + [Tutorial: Connect and test client devices](client-devices-tutorial.md)
   + [AWS-provided client device components](client-device-components.md)
   + [Connect client devices to core devices](connect-client-devices.md)
      + [Associate client devices](associate-client-devices.md)
      + [Manage core device endpoints](manage-core-device-endpoints.md)
      + [Test client device communications](test-client-device-communications.md)
      + [Greengrass discovery RESTful API](greengrass-discover-api.md)
   + [Relay MQTT messages between client devices and AWS IoT Core](relay-client-device-messages.md)
   + [Interact with client devices in components](interact-with-client-devices-in-components.md)
   + [Troubleshooting client devices](troubleshooting-client-devices.md)
+ [Interact with device shadows](interact-with-shadows.md)
   + [Interact with shadows in components](interact-with-shadows-in-components.md)
   + [Sync local device shadows with AWS IoT Core](sync-shadows-with-iot-core.md)
+ [Manage data streams on the AWS IoT Greengrass Core](manage-data-streams.md)
   + [Create custom components that use stream manager](use-stream-manager-in-custom-components.md)
   + [Use StreamManagerClient to work with streams](work-with-streams.md)
      + [Export configurations for supported AWS Cloud destinations](stream-export-configurations.md)
   + [Configure AWS IoT Greengrass stream manager](configure-stream-manager.md)
+ [Perform machine learning inference](perform-machine-learning-inference.md)
   + [Tutorial: Perform sample image classification inference using TensorFlow Lite](ml-tutorial-image-classification.md)
   + [Perform sample image classification inference on images from a camera using TensorFlow Lite](ml-tutorial-image-classification-camera.md)
   + [Use Amazon SageMaker Edge Manager on Greengrass core devices](use-sagemaker-edge-manager.md)
      + [Get started with SageMaker Edge Manager](get-started-with-edge-manager-on-greengrass.md)
   + [Customize your machine learning components](ml-customization.md)
   + [Troubleshooting machine learning inference](ml-troubleshooting.md)
+ [Greengrass Command Line Interface](gg-cli.md)
   + [Install the Greengrass CLI](install-gg-cli.md)
   + [Greengrass CLI commands](gg-cli-reference.md)
      + [component](gg-cli-component.md)
      + [deployment](gg-cli-deployment.md)
      + [logs](gg-cli-logs.md)
      + [get-debug-password](gg-cli-get-debug-password.md)
+ [Security in AWS IoT Greengrass](security.md)
   + [Data protection in AWS IoT Greengrass](data-protection.md)
      + [Data encryption](data-encryption.md)
         + [Encryption in transit](encryption-in-transit.md)
         + [Encryption at rest](encryption-at-rest.md)
         + [Key management for the Greengrass core device](key-management.md)
   + [Device authentication and authorization for AWS IoT Greengrass](device-auth.md)
   + [Identity and access management for AWS IoT Greengrass](security-iam.md)
      + [How AWS IoT Greengrass works with IAM](security_iam_service-with-iam.md)
      + [Identity-based policy examples for AWS IoT Greengrass](security_iam_id-based-policy-examples.md)
      + [Authorize core devices to interact with AWS services](device-service-role.md)
      + [Minimal IAM policy for installer to provision resources](provision-minimal-iam-policy.md)
      + [Greengrass service role](greengrass-service-role.md)
      + [AWS managed policies for AWS IoT Greengrass](security-iam-aws-managed-policies.md)
      + [Cross-service confused deputy prevention](cross-service-confused-deputy-prevention.md)
      + [Troubleshooting identity and access issues for AWS IoT Greengrass](security_iam_troubleshoot.md)
   + [Allow device traffic through a proxy or firewall](allow-device-traffic.md)
   + [Compliance validation for AWS IoT Greengrass](compliance-validation.md)
   + [Resilience in AWS IoT Greengrass](disaster-recovery-resiliency.md)
   + [Infrastructure security in AWS IoT Greengrass](infrastructure-security.md)
   + [Configuration and vulnerability analysis in AWS IoT Greengrass](vulnerability-analysis-and-management.md)
   + [Code integrity in AWS IoT Greengrass V2](code-integrity.md)
   + [AWS IoT Greengrass and interface VPC endpoints (AWS PrivateLink)](vpc-interface-endpoints.md)
   + [Security best practices for AWS IoT Greengrass](security-best-practices.md)
+ [Using AWS IoT Device Tester for AWS IoT Greengrass V2](device-tester-for-greengrass-ug.md)
   + [Supported versions of AWS IoT Device Tester for AWS IoT Greengrass V2](dev-test-versions.md)
   + [Use IDT to run the AWS IoT Greengrass qualification suite](idt-greengrass-qualification.md)
      + [Prerequisites for running the AWS IoT Greengrass qualification suite](dev-tst-prereqs.md)
      + [Configure your device to run IDT tests](device-config-setup.md)
      + [Configure IDT settings to run the AWS IoT Greengrass qualification suite](set-config.md)
      + [Run the AWS IoT Greengrass qualification suite](run-tests.md)
      + [Understanding results and logs](results-logs.md)
   + [Use IDT to develop and run your own test suites](idt-custom-tests.md)
      + [Tutorial: Build and run the sample IDT test suite](build-sample-suite.md)
      + [Tutorial: Develop a simple IDT test suite](create-custom-tests.md)
      + [Create IDT test suite configuration files](idt-json-config.md)
      + [Configure the IDT state machine](idt-state-machine.md)
      + [Create IDT test case executables](create-test-executables.md)
      + [Use the IDT context](idt-context.md)
      + [Configure settings for test runners](set-custom-idt-config.md)
      + [Debug and run custom test suites](run-debug-custom-tests.md)
      + [Review IDT test results and logs](idt-review-results-logs.md)
      + [IDT usage metrics](idt-usage-metrics.md)
   + [Troubleshooting IDT for AWS IoT Greengrass V2](idt-troubleshooting.md)
   + [Support policy for AWS IoT Device Tester for AWS IoT Greengrass](idt-support-policy.md)
+ [Troubleshooting AWS IoT Greengrass V2](troubleshooting.md)
+ [Tag your AWS IoT Greengrass Version 2 resources](tag-resources.md)
+ [Open source AWS IoT Greengrass Core software](open-source.md)
+ [Document history for the AWS IoT Greengrass V2 Developer Guide](document-history.md)
+ [AWS glossary](glossary.md)