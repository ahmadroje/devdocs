---
group: advanced-reporting
title: Advanced Reporting
functional_areas:
    - Reports
migrated_to: https://developer.adobe.com/commerce/php/development/advanced-reporting/
layout: migrated
---

[Advanced reporting functionality] is free to {{site.data.var.ee}} and {{site.data.var.ce}} customers and is provided through an integration of a Magento instance with [{{site.data.var.ee}} Reporting]. Magento collects data and sends this information to Commerce Reporting for analytics. You do not need to have an Commerce Reporting account to use Advanced Reporting.

## Prerequisites

1. The website must run on a public web server.
1. The domain must have a valid security (SSL) certificate.
1. Magento must have been installed or upgraded successfully without error.
1. In the Magento configuration, the [Base URL (Secure) setting][base url] for the store view must point to the secure URL. For example https://yourdomain.com.
1. In the Magento configuration, **Use Secure URLs on Storefront**, **and Use Secure URLs in Admin** must be set to **Yes**.
1. Make sure that [Magento crontab] is created and cron jobs are running on the installed server.

The merchant can now click on the **Go to Advanced Reporting** button on the Admin dashboard to launch the advanced reporting features.

{:.bs-callout-info}
It can take up to a day for data to be available in Advanced Reporting.

## Recommendations

To avoid system overload during its prime time, you can set the preferable time of a day for a data collection.

## Extensibility

Though the Analytics module provides an API, it is used specifically to interchange data with Commerce Reporting. Magento does not recommend extending the advanced reporting functionality.

{:.ref-header}
Related topics

[Magento modules that implement the functionality][modules]

[Data collection configuration and settings][collection]

<!-- LINK DEFINITIONS -->

[modules]: modules.html
[collection]: data-collection.html

[Advanced reporting functionality]: {{ site.user_guide_url }}/reports/advanced-reporting.html
[base url]: {{ site.user_guide_url }}/stores/store-urls.html
[{{site.data.var.ee}} Reporting]: https://magento.com/products/business-intelligence
[Magento crontab]: {{ page.baseurl }}/config-guide/cli/config-cli-subcommands-cron.html
