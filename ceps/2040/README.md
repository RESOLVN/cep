# CEP 2040:  Network Specification and Clone Source Best Practice

## Abstract
This CEP details best practice for the design and implementation of Network Specs and Clone Sources. Specifically, it outlines the requirement to deconflict Network Specs and Clone Sources to avoid having too many Clone Sources nested in a single Network Spec. It also sets the best practice of having each Content Module have a one-to-one relationship between Network Specs and Clone Sources. It also codifies Range Minimization and gives guidelines on how to reduce the number of unnecessary VMs and Subnets in a given range.

## Rationale

### Content Module - Network Spec - Clone Source Deconfliction
Best practice has shown that for any given Content Module, a single Network Spec with one attached Clone Source is the ideal setup. This mitigates many problems with Network Specs and Clone Sources, including limiting the number of possible Clone Sources for the module, limiting the effect of changing the Network Spec and unintentionally changing a Clone Source for a different deployment, and keeping Network Specs organized.

While it may be necessary to have backup Clone Sources from time to time, the author of a given module should make every effort to reduce the number of Clone Sources that are kept in any given Network Spec to a single Clone Source. This is especially true for instructional modules where the Clone Source has been finalized and attached.

To ensure that Module <-> Network Spec <-> Clone Source remains a one-to-one-to-one relationship, ensure that new ranges are forked from existing ranges into their own separate Network Spec via the 'Reassign' feature. This workflow could look like the following:

 1. Author identifies a good base Clone Source that would be useful for a new module.
 2. Author goes into the existing Network Spec for that module and creates a deployment from that module's Clone Source.
 3. Author clicks the ellipses button next to the new deployment and selects `Reassign` (pictured below)
4. Author creates a separate Network Spec for this new range build.

![reassign](reassign.png)
 
 ### Range Minimization
 HardHat ranges utilize some auxiliary services in order to rapidly create networks. These services are deployed from specially configured VM templates and provide DHCP, puppet configuration, and other kinds of range creation services. After range creation is completed, these services are no longer needed within the deployment.
 
 During range finalization and minimization, the Author will ensure that the final Clone Source that is attached to any given content module does not include the extra range management VMs. This can include, but is not limited to:
 * simspace-mgmt
 * control-dhcp
 * nagios
 * range-transfer

It is important to note that simply removing the range management VMs and VM Templates from the Network Spec may have unintended side-effects. A better way to minimize the range is to uncheck these VMs during deployment of the finalized Clone Source.

To ensure the listed VMs are not deployed with the final Clone Source, the following workflow may be used:
1. Using a given Clone Source, create a new deployment with the latest version of the Network Spec.
2. Click `Open` to open the deployment options.
3. In the second tab, `Review Deployment`, uncheck all boxes next to the range management VMs.
4. Continue to create the deployment and build the range.
5. (Optional) Before finalizing the new Clone Source, this is a good time to check all functionality of the Clone Source, check the artifacts, clean the VMs for finalization, etc.
6. Shut down the new deployment and create a new Clone Source. This new Clone Source will not deploy any of the range management VMs. Reattach this new Clone Source to the Content Module and ensure all VMs are re-added to the VM Access Panel.

### Range Subnets
Generally speaking, the number of Subnets in the Network Spec should match the number of subnets that are used in the range. The Author will make effort to reduce the number of subnets down to the ones that are utilized. The Author will make special effort to ensure the Real-Internet subnet, if used during the range testing and development, is removed prior to Clone Source minimization and finalization.

### Requirements
   * Each Content Module will have a one-to-one relationship with a Network Spec. All new content modules will have their own dedicated Network Spec.
   * Reuse of an existing Clone Source for multiple ranges is acceptable, either as a starting point or as a final range, provided the Clone Source is deployed and reassigned into its own Network Spec.
   * Authors will make effort to reduce the number of Clone Sources in any given Network Spec to a minimum. During the test and development process, multiple Clone Sources may be necessary. After a content module is finalized and the range has been attached, the Author will reduce the number of Clone Sources as much as is appropriate. 
   * When finalizing and minimizing a range for a content module, the Author will ensure that the auxiliary VMs (simspace-mgmt, range-transfer, control-dhcp, etc) are not deployed in the Clone Source that is attached to the Content Module. See above for a workflow for this process.
   * The Author will ensure the number of Subnets in the Network Spec is reduced to the minimum necessary for use in the range.
   * The Author will make special effort to remove the Real-Internet subnet if it was used during development prior to range minimization.

## References and Footnotes

