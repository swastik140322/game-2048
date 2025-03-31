2048 App
Create Fargate profile

eksctl create fargateprofile \
    --cluster demo-cluster \
    --region us-east-1 \
    --name alb-sample-app \
    --namespace game-2048

Deploy the deployment, service and Ingress

kubectl apply -f https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.5.4/docs/examples/2048/2048_full.yaml


![258144320-93b06a9f-67f9-404f-b0ad-18e3095b7353](https://github.com/user-attachments/assets/37e255f5-b656-47da-820e-826d12d976a1)
