# Cloudwatch


# See cluster role name
eksctl get nodegroup --cluster basic-cluster -o json
</br>
# Update cluster stack name
aws cloudformation describe-stack-resources --stack-name eksctl-basic-cluster-nodegroup-ng-1
</br>
# Update cluster policy
aws iam attach-role-policy --role-name eksctl-basic-cluster-nodegroup-ng-NodeInstanceRole-5W2I55I4WE2W --policy-arn arn:aws:iam::aws:policy/CloudWatchAgentServerPolicy
</br>
# See cluster policy list
aws iam list-attached-role-policies --role-name eksctl-basic-cluster-nodegroup-ng-NodeInstanceRole-5W2I55I4WE2W

</br>
#kubectl -n amazon-cloudwatch get daemonsets
</br>
Reference  18:00 to 29:00 minutes
https://www.youtube.com/watch?v=-8kFawk-EFs
