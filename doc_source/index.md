# Amazon Elastic Container Service Developer Guide

-----
*****Copyright &copy; 2018 Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

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
+ [What is Amazon Elastic Container Service?](Welcome.md)
+ [Setting Up with Amazon ECS](get-set-up-for-amazon-ecs.md)
+ [Docker Basics for Amazon ECS](docker-basics.md)
+ [Getting Started with Amazon ECS using Fargate](ECS_GetStarted.md)
+ [Cleaning Up your Amazon ECS Resources](ECS_CleaningUp.md)
+ [AWS Fargate on Amazon ECS](AWS_Fargate.md)
   + [AWS Fargate Platform Versions](platform_versions.md)
+ [Amazon ECS Clusters](ECS_clusters.md)
   + [Creating a Cluster](create_cluster.md)
   + [Scaling a Cluster](scale_cluster.md)
   + [Deleting a Cluster](delete_cluster.md)
+ [Amazon ECS Container Instances](ECS_instances.md)
   + [Container Instance AMIs](container_instance_AMIs.md)
      + [Amazon ECS-Optimized AMI](ecs-optimized_AMI.md)
         + [How to Launch the Latest Amazon ECS-Optimized AMI](ecs-optimized_AMI_launch_latest.md)
         + [Amazon ECS-Optimized AMI Versions](ecs-ami-versions.md)
         + [Storage Configuration](ecs-ami-storage-config.md)
   + [Subscribing to Amazon ECS–Optimized AMI Update Notifications](ECS-AMI-SubscribeTopic.md)
   + [Launching an Amazon ECS Container Instance](launch_container_instance.md)
   + [Bootstrapping Container Instances with Amazon EC2 User Data](bootstrap_container_instance.md)
      + [Example Container Instance User Data Configuration Scripts](example_user_data_scripts.md)
   + [Connect to Your Container Instance](instance-connect.md)
   + [Using CloudWatch Logs with Container Instances](using_cloudwatch_logs.md)
   + [Container Instance Draining](container-instance-draining.md)
   + [Container Instance Memory Management](memory-management.md)
   + [Managing Container Instances Remotely](ec2-run-command.md)
   + [Starting a Task at Container Instance Launch Time](start_task_at_launch.md)
   + [Deregister a Container Instance](deregister_container_instance.md)
+ [Amazon ECS Container Agent](ECS_agent.md)
   + [Installing the Amazon ECS Container Agent](ecs-agent-install.md)
   + [Amazon ECS Container Agent Versions](container_agent_versions.md)
   + [Updating the Amazon ECS Container Agent](ecs-agent-update.md)
      + [Updating the Amazon ECS Container Agent on the Amazon ECS-Optimized AMI](agent-update-ecs-ami.md)
      + [Manually Updating the Amazon ECS Container Agent (for Non-Amazon ECS-optimized AMIs)](manually_update_agent.md)
   + [Amazon ECS Container Agent Configuration](ecs-agent-config.md)
   + [Automated Task and Image Cleanup](automated_image_cleanup.md)
   + [Private Registry Authentication](private-auth.md)
   + [Amazon ECS Container Metadata File](container-metadata.md)
   + [Amazon ECS Task Metadata Endpoint](task-metadata-endpoint.md)
   + [Amazon ECS Container Agent Introspection](ecs-agent-introspection.md)
   + [HTTP Proxy Configuration](http_proxy_config.md)
+ [Amazon ECS Task Definitions](task_definitions.md)
   + [Application Architecture](application_architecture.md)
   + [Creating a Task Definition](create-task-definition.md)
   + [Task Definition Parameters](task_definition_parameters.md)
   + [Using Data Volumes in Tasks](using_data_volumes.md)
   + [Task Networking with the awsvpc Network Mode](task-networking.md)
   + [Amazon ECS Launch Types](launch_types.md)
   + [Using the awslogs Log Driver](using_awslogs.md)
   + [Example Task Definitions](example_task_definitions.md)
   + [Updating a Task Definition](update-task-definition.md)
   + [Deregistering Task Definitions](deregister-task-definition.md)
+ [Scheduling Amazon ECS Tasks](scheduling_tasks.md)
   + [Running Tasks](ecs_run_task.md)
   + [Amazon ECS Task Placement](task-placement.md)
      + [Amazon ECS Task Placement Strategies](task-placement-strategies.md)
      + [Amazon ECS Task Placement Constraints](task-placement-constraints.md)
      + [Cluster Query Language](cluster-query-language.md)
   + [Scheduled Tasks (cron)](scheduled_tasks.md)
   + [Task Lifecycle](task_life_cycle.md)
   + [Task Retirement](task-retirement.md)
   + [Creating a Scheduled Task Using the AWS CLI](scheduled_tasks_cli_tutorial.md)
+ [Services](ecs_services.md)
   + [Service Definition Parameters](service_definition_parameters.md)
   + [Service Load Balancing](service-load-balancing.md)
      + [Load Balancer Types](load-balancer-types.md)
      + [Check the Service Role for Your Account](check-service-role.md)
      + [Creating a Load Balancer](create-load-balancer.md)
         + [Creating an Application Load Balancer](create-application-load-balancer.md)
         + [Creating a Network Load Balancer](create-network-load-balancer.md)
         + [Creating a Classic Load Balancer](create-standard-load-balancer.md)
   + [Service Auto Scaling](service-auto-scaling.md)
      + [Target Tracking Scaling Policies](service-autoscaling-targettracking.md)
      + [Step Scaling Policies](service-autoscaling-stepscaling.md)
   + [Creating a Service](create-service.md)
   + [Updating a Service](update-service.md)
   + [Deleting a Service](delete-service.md)
   + [Service Throttle Logic](service-throttle-logic.md)
+ [Amazon ECR Repositories](ECS_Console_Repositories.md)
+ [Monitoring Amazon ECS](ecs_monitoring.md)
   + [Monitoring Tools](monitoring-automated-manual.md)
   + [Amazon ECS CloudWatch Metrics](cloudwatch-metrics.md)
      + [Viewing Amazon ECS Metrics](viewing_cloudwatch_metrics.md)
      + [Tutorial: Scaling Container Instances with CloudWatch Alarms](cloudwatch_alarm_autoscaling.md)
   + [Amazon ECS Event Stream for CloudWatch Events](cloudwatch_event_stream.md)
      + [Amazon ECS Events](ecs_cwe_events.md)
      + [Handling Events](ecs_cwet_handling.md)
      + [Tutorial: Listening for Amazon ECS CloudWatch Events](ecs_cwet.md)
      + [Tutorial: Sending Amazon Simple Notification Service Alerts for Task Stopped Events](ecs_cwet2.md)
+ [Amazon ECS IAM Policies, Roles, and Permissions](IAM_policies.md)
   + [Policy Structure](iam-policy-structure.md)
   + [Supported Resource-Level Permissions for Amazon ECS API Actions](ecs-supported-iam-actions-resources.md)
   + [Creating Amazon ECS IAM Policies](ECS_IAM_user_policies.md)
   + [Managed Policies and Trust Relationships](managed_policies.md)
      + [Amazon ECS Managed Policies and Trust Relationships](ecs_managed_policies.md)
      + [Amazon ECR Managed Policies](ecr_managed_policies.md)
   + [Amazon ECS Container Instance IAM Role](instance_IAM_role.md)
   + [Amazon ECS Task Execution IAM Role](task_execution_IAM_role.md)
   + [Using Service-Linked Roles for Amazon ECS](using-service-linked-roles.md)
   + [Amazon ECS Service Scheduler IAM Role](service_IAM_role.md)
   + [Amazon ECS Service Auto Scaling IAM Role](autoscale_IAM_role.md)
   + [Amazon Elastic Container Service Task Role](task_IAM_role.md)
   + [CloudWatch Events IAM Role](CWE_IAM_role.md)
   + [IAM Roles for Tasks](task-iam-roles.md)
   + [Amazon ECS IAM Policy Examples](IAMPolicyExamples.md)
+ [Using the Amazon ECS Command Line Interface](ECS_CLI.md)
   + [Installing the Amazon ECS CLI](ECS_CLI_installation.md)
   + [Configuring the Amazon ECS CLI](ECS_CLI_Configuration.md)
   + [Migrating Configuration Files](ECS_CLI_migrating_config_files.md)
   + [Tutorial: Creating a Cluster with a Fargate Task Using the ECS CLI](ECS_CLI_tutorial_fargate.md)
   + [Tutorial: Creating a Cluster with an EC2 Task Using the ECS CLI](ECS_CLI_tutorial_EC2.md)
   + [Amazon ECS Command Line Reference](ECS_CLI_reference.md)
      + [ecs-cli](cmd-ecs-cli.md)
      + [ecs-cli configure](cmd-ecs-cli-configure.md)
      + [ecs-cli configure default](cmd-ecs-cli-configure-default.md)
      + [ecs-cli configure profile](cmd-ecs-cli-configure-profile.md)
      + [ecs-cli configure profile default](cmd-ecs-cli-configure-profile-default.md)
      + [ecs-cli configure migrate](cmd-ecs-cli-configure-migrate.md)
      + [ecs-cli up](cmd-ecs-cli-up.md)
      + [ecs-cli down](cmd-ecs-cli-down.md)
      + [ecs-cli scale](cmd-ecs-cli-scale.md)
      + [ecs-cli logs](cmd-ecs-cli-logs.md)
      + [ecs-cli ps](cmd-ecs-cli-ps.md)
      + [ecs-cli push](cmd-ecs-cli-push.md)
      + [ecs-cli pull](cmd-ecs-cli-pull.md)
      + [ecs-cli images](cmd-ecs-cli-images.md)
      + [ecs-cli license](cmd-ecs-cli-license.md)
      + [ecs-cli compose](cmd-ecs-cli-compose.md)
      + [ecs-cli compose create](cmd-ecs-cli-compose-create.md)
      + [ecs-cli compose start](cmd-ecs-cli-compose-start.md)
      + [ecs-cli compose up](cmd-ecs-cli-compose-up.md)
      + [ecs-cli compose service](cmd-ecs-cli-compose-service.md)
+ [Using the AWS CLI with Amazon ECS](ECS_AWSCLI.md)
   + [Tutorial: Creating a Cluster with a Fargate Task Using the AWS CLI](ECS_AWSCLI_Fargate.md)
   + [Tutorial: Creating a Cluster with a EC2 Task Using the AWS CLI](ECS_AWSCLI_EC2.md)
+ [Common Use Cases in Amazon ECS](common_use_cases.md)
+ [Tutorial: Creating a VPC with Public and Private Subnets for Your Clusters](create-public-private-vpc.md)
+ [Tutorial: Using Amazon EFS File Systems with Amazon ECS](using_efs.md)
+ [Tutorial: Continuous Deployment with AWS CodePipeline](ecs-cd-pipeline.md)
+ [Amazon ECS Service Limits](service_limits.md)
+ [Logging Amazon ECS API Calls By Using AWS CloudTrail](logging-using-cloudtrail.md)
+ [Amazon ECS Troubleshooting](troubleshooting.md)
   + [Checking Stopped Tasks for Errors](stopped-task-errors.md)
   + [Service Event Messages](service-event-messages.md)
   + [Invalid CPU or Memory Value Specified](task-cpu-memory-error.md)
   + [Cannot Pull Container Image Error](task_cannot_pull_image.md)
   + [CannotCreateContainerError: API error (500): devmapper](CannotCreateContainerError.md)
   + [Troubleshooting Service Load Balancers](troubleshoot-service-load-balancers.md)
   + [Enabling Docker Debug Output](docker-debug-mode.md)
   + [Amazon ECS Log File Locations](logs.md)
   + [Amazon ECS Logs Collector](ecs-logs-collector.md)
   + [Agent Introspection Diagnostics](introspection-diag.md)
   + [Docker Diagnostics](docker-diags.md)
   + [API failures Error Messages](api_failures_messages.md)
   + [Troubleshooting IAM Roles for Tasks](troubleshoot-task-iam-roles.md)
+ [Windows Containers](ECS_Windows.md)
   + [Getting Started with Windows Containers](ECS_Windows_getting_started.md)
   + [Windows Task Definitions](windows_task_definitions.md)
   + [Windows IAM Roles for Tasks](windows_task_IAM_roles.md)
   + [Pushing Windows Images to Amazon ECR](windows_ecr.md)
+ [Document History](document_history.md)
+ [AWS Glossary](glossary.md)