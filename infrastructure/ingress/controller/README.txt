Kindly borrowed from https://github.com/jetstack/kube-lego/tree/master/examples/nginx/nginx

In order to use with RBAC, run kubectl apply -f rbac.yml which will create a serviceaccount called
nginx-ingress.serviceaccount, a ClusterRole nginx-ingress-clusterrole, and a ClusterRoleBinding between 
the two. This will allow the role to see and update services in all namespace which is needed to function 
properly.
