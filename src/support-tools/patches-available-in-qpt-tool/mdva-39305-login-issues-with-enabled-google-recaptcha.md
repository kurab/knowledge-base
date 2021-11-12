---
title: "MDVA-39305: Login issue with enabled Google reCAPTCHA"
labels: QPT patches,Quality Patches Tool,Support Tools,QPT 1.1.1,Magento Commerce Cloud,Adobe Commerce,on-premise,cloud infrastructure,QPT,Quality Patches Tool
---

The MDVA-39305 Adobe Commerce patch fixes the issue where registered customers are not able to log in with enabled Google reCAPTCHA. This patch is available when the [Quality Patches Tool (QPT)](https://support.magento.com/hc/en-us/articles/360047139492) 1.1.1 is installed. The patch ID is MDVA-39305. Please note that the issue is scheduled to be fixed in Adobe Commerce version 2.4.4.

## Affected products and versions

**The patch is created for Adobe Commerce version:**

* Adobe Commerce on our cloud infrastructure 2.4.2-p1

**Compatible with Adobe Commerce versions:**

* Adobe Commerce on-premises and Adobe Commerce on our cloud infrastructure 2.4.0-2.4.2-p1

>![info]
>
>Note: the patch might become applicable to other versions with new Quality Patches Tool releases. To check if the patch is compatible with your Adobe Commerce version, update the `magento/quality-patches` package to the latest version and check the compatibility on the [QPT landing page](https://devdocs.magento.com/quality-patches/tool.html#patch-grid). Use the patch ID as a search keyword to locate the patch.

## Issue

Registered customers are not able to log in using the enabled Google reCAPTCHA.

<ins>Steps to reproduce</ins>:

1. Go to **Store** > **Configuration** > **Security** > **Google reCAPTCHA Storefront** and enable **Google reCAPTCHA**.
1. Go to **Frontend**.
1. Open **Developer Tool Console** in the browser.

<ins>Expected results</ins>:

No CSP warnings in the console.

<ins>Actual results</ins>:

CSP warnings in the console.

## Apply the patch

To apply individual patches use the following links depending on your deployment type:

* Adobe Commerce on-premise: [Software Update Guide > Apply Patches](https://devdocs.magento.com/guides/v2.4/comp-mgr/patching/mqp.html) in our developer documentation.
* Adobe Commerce for cloud: [Upgrades and Patches > Apply Patches](https://devdocs.magento.com/cloud/project/project-patch.html) in our developer documentation.

## Related reading

To learn more about Quality Patches Tool, refer to:

* [Quality Patches Tool released: a new tool to self-serve quality patches](https://support.magento.com/hc/en-us/articles/360047139492).
* [Check if patch is available for your Adobe Commerce issue using Quality Patches Tool](https://support.magento.com/hc/en-us/articles/360047125252).

For info about other patches available in QPT, refer to the [Patches available in QPT](https://support.magento.com/hc/en-us/sections/360010506631-Patches-available-in-QPT-tool-) section.