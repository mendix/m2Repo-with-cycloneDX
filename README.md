# Purpose

When using the [Managed Dependencies](https://docs.mendix.com/refguide/managed-dependencies/) feature, a `vendorlib-sbom.json` file is generated in the `vendorlib` folder. We generate this document with the help of the [CycloneDx Gradle plugin](https://github.com/CycloneDX/cyclonedx-gradle-plugin). This is downloaded on your local environment from the Gradle Plugin Repository.

On an air-gapped/internet-restricted setup, downloading the plugin will fail if there is no access to the plugin repository. To mitigate this issue, we have created a custom repository containing the CycloneDx Gradle plugin.

# Usage

You need to configure Studio Pro to use this repository. The steps to configure can be found in the [Custom Repository](https://docs.mendix.com/refguide/managed-dependencies/#custom-repos) section of Mendix Docs.

After configuring Studio Pro, you'll be able to build and run your application successfully and the `vendorlib-sbom.json` file will also be generated.

# Troubleshooting

If you are finding trouble configuring Studio Pro or you are faced with different errors, please contact [Mendix Support](https://support.mendix.com/)