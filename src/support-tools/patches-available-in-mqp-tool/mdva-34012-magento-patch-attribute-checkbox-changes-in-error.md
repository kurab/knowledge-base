---
title: MDVA-34012 Magento patch: attribute checkbox changes in error
labels: 2.3.1,2.3.2,2.3.2-p2,2.3.3,2.3.3-p1,2.3.4,2.3.4-p1,2.3.4-p2,2.3.5,2.3.5-p1,2.3.5-p2,2.3.6,2.3.6-p1,2.4.0,2.4.0-p1,2.4.1,2.4.1-p1,2.4.2,MQP 1.0.17,MQP patches,Magento Commerce,Magento Commerce Cloud,Magento Quality Patches,attribute,checkbox,error,schedule update
---

The MDVA-34012 Magento patch solves the issue where the checkbox for an attribute gets changed after a schedule update in error.

This patch is available when the [Magento Quality Patch (MQP) tool](https://devdocs.magento.com/guides/v2.4/comp-mgr/patching.html#mqp) 1.0.17 is installed. Please note that the issue is scheduled to be fixed in Magento version 2.4.3.

## Affected products and versions

 **The patch is created for Magento version:** Magento Commerce Cloud 2.3.5-p2

 **Compatible with Magento versions:** Magento Commerce Cloud and Magento Commerce 2.3.1 - 2.4.2

>![info]
>
>Note: the patch might become applicable to other versions with new MQP tool releases. To check if the patch is compatible with your Magento version, run `./vendor/bin/magento-patches status` .

## Issue

 <span class="wysiwyg-underline">Steps to reproduce</span> :

1. Login to Admin and navigate to **Catalog > Products** .
1. Edit any simple product.
1. Change the store view to a specific store view.
1. Save the product with the **Use default value** checkbox selected for an attribute (Example: **Enable Product** attribute).
1. Click on **Schedule New Update** to schedule some changes (Example: **Price** or **Special Price** for a specific store view).
1. Wait until the changes complete.
1. Check the product. It should have its checkbox unselected, and should have a specific store attribute value.

 <span class="wysiwyg-underline">Expected results</span> :

The checkbox for the attribute should remain the same and doesn't get changed after the schedule update, as expected.

 <span class="wysiwyg-underline">Actual results</span> :

The checkbox for the attribute gets changed after schedule update.

## Apply the patch

To apply individual patches use the following links depending on your Magento product:

* Magento Commerce: DevDocs [Software Update Guide > Apply Patches](https://devdocs.magento.com/guides/v2.4/comp-mgr/patching.html) .
* Magento Commerce Cloud: DevDocs [Upgrades and Patches > Apply Patches](https://devdocs.magento.com/cloud/project/project-patch.html) .

## Related reading

To learn more about Magento Quality Patches, refer to:

* [Magento Quality Patches released: a new tool to self-serve quality patches](https://support.magento.com/hc/en-us/articles/360047139492) .
* [Check patch for Magento issue with Magento Quality Patches](https://support.magento.com/hc/en-us/articles/360047125252) .

For info about other patches available in MQP tool, refer to the [Patches available in MQP tool](https://support.magento.com/hc/en-us/sections/360010506631-Patches-available-in-MQP-tool-) section.