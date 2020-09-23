This demo was made by adapting the code from https://github.com/siamaksade/tekton-cd-demo

To make the pipeline works you need to create a serviceAccount to run privileged containers. 

* `oc create serviceaccount pipeline`
* `oc adm policy add-scc-to-user privileged -z pipeline`
* `oc adm policy add-role-to-user edit -z pipeline`

Copy the rest of the resources and then start the pipeline by using the resources created. As an example you can see the pipelineRun file.
