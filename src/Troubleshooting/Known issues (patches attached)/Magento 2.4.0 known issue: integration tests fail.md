This article provides a patch for the Magento 2.4.0 issue where integration tests are failing because the declaration of `` Dotdigitalgroup\Email\Test\Integration\Model\Sync\Importer\ImporterFailedTest::setUp() `` is not compatible with PHPUnit 9 which is used for 2.4.0.&nbsp;

## Affected products and versions

*   Magento Commerce Cloud 2.4.0
*   Magento Commerce 2.4.0

## Issue

<span class="wysiwyg-underline">Steps to reproduce</span>

Run 2.4.0 integration tests.

<span class="wysiwyg-underline">Expected result&nbsp;</span>

Tests pass.

<span class="wysiwyg-underline">Actual result</span>

_PHP Fatal error: Declaration of Dotdigitalgroup\\Email\\Test\\Integration\\Model\\Sync\\Importer\\ImporterFailedTest::setUp() must be compatible with PHPUnit\\Framework\\TestCase::setUp(): void in /var/www/vendor/dotmailer/dotmailer-magento2-extension/Test/Integration/Model/Sync/Importer/ImporterFailedTest.php on line 36_

## Solution

Apply the patch provided in this article.

## Patch

The patch is attached to this article. To download it, scroll down to the end of the article and click the file name, or click the following link:

<a href="https://support.magento.com/hc/en-us/article_attachments/360063994752/BUNDLE-2684-composer.patch" target="_self">BUNDLE-2684-composer.patch</a>

### Compatible Magento versions:

The patch was created for:

*   Magento Commerce Cloud 2.4.0
*   Magento Commerce 2.4.0

## How to apply the patch

See <a href="https://support.magento.com/hc/en-us/articles/360028367731" target="_self">How to apply a composer patch provided by Magento</a> for instructions.

## Attached Files