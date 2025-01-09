Issues faced:

"Warning: annotation "kubernetes.io/ingress.class" is deprecated, please use 'spec.ingressClassName' instead" which is a warning and can ignore
I was unable to see the lb address while giving k get ing -n robot-shop,
with the help of docs and chatpgt , I have added below to the policy.json of the
AWSLoadBalancerControllerIAMPolicy. Later I can see the address of lb and able to access the Robot shop UI .


{
  "Effect": "Allow",
  "Action": "elasticloadbalancing:DescribeListenerAttributes",
  "Resource": "*"
}

**Instana Robotshop page exposed on EKS using ALB,OIDC,EBS CSI Plugin**
![image](https://github.com/user-attachments/assets/87a928b5-9269-4943-a65d-b8b386b1449d)


