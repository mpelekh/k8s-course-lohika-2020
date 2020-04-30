# Home Work

1. Create 3 namespaces.
2. Create Deployment, ReplicaSet and StatefulSets in each namespace.
3. Create HorizontalPodAutoscaler for each Deployment, ReplicaSet and StatefulSet.
4. Add load to Pod. For example: fulload() { dd if=/dev/zero of=/dev/null | dd if=/dev/zero of=/dev/null | dd if=/dev/zero of=/dev/null | dd if=/dev/zero of=/dev/null & }; fulload; read; killall dd
5. Provide the result of the “kubectl describe horizontalpodautoscaler.autoscaling/NAME_OF_YOUR_HPA” command for each HPA

# Notes:
- This link is used to do a task: https://kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale-walkthrough/