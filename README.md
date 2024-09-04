# AWS Cloud Cost Optimization

## Detecting and Removing Unused EBS Snapshots

In this project, I developed a Lambda function designed to identify and delete EBS snapshots that are no longer linked to any active EC2 instances, thereby reducing storage expenses.

## Description
The Lambda function retrieves all EBS snapshots owned by the account and gathers a list of active EC2 instances (both running and stopped). It then checks each snapshot to see if its associated volume is not connected to any active instance. If a snapshot is identified as unused, the function deletes it, helping to optimize storage costs.
