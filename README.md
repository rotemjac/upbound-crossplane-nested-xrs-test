# upbound-crossplane-nested-xrs-test
A repo for displaying a specific issue with nested costum resources.


**Current Status:**

1. The `claim_Example_for_the_internal_network_xrd__working.yaml` is working.

2. The `claim_Example_for_the_external_cluster_xrd__not_working.yaml` fails with the error below:

> ComposeResources: cannot render composed resource from resource template at index 0: cannot use dry-run create to name composed resource: CompositeNetwork.aws.platformref.crossplane.io "my-cluster-claim-1-2xn9w-v2x54" is invalid: spec.parameters: Required value
   

So the problem is probably related to the external definition.yaml/composition.yaml files.
