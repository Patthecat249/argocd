# Argo-CD Understanding for myself
This Repository contains yaml-files to come from zero-to-hero with ArgoCD on OpenShift with the gitops-Operator in an airgapped cluster

## Start with the Prerequisites
- Mirror your choosen Operators in your private Registry
- Apply an ImageContentSourcePolicy to reference to your private Registry, where the images were mirrored
- Disable the Operator-Hub so that the OLM doesn't try to look at Red Hat Indexes for Operators
- Apply your Catalogsource which was created by the oc-mirror-plugin. It should be in the results-folder of the folder oc-mirror-workspace
- Install the Red Hat GitOps Operator by Using the subscription 

# Now it's time to setup ArgoCD, a project and your first application
- Setup the default ArgoCD-Instanz which is called openshift-gitops to increase the memory of the application-controller-pod
- Create a ArgoCD-Project
- Create your first Application (a wordpress-demo) 