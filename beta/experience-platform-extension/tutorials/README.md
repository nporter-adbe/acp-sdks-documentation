# Adobe Experience Platform Edge Mobile SDK Tutorials

{% hint style="warning" %}
The Adobe Experience Platform Edge mobile extension is currently in BETA. Use of this extension is by invitation only. Please contact your Adobe Customer Success Manager to learn more and get access to the materials for these tutorials.
{% endhint %}

## Beta Schedule

### Assignment 1

In this assignment you will learn how to:

1. Create a schema, a dataset and generate a configuration identifier in Adobe Experience Platform Launch 
2. Get familiar with the sample demo applications (iOS Swift, Android)
3. Setup Project Griffon and use it for validating XDM events
4. Query the commerce events in Adobe Experience Platform
5. Implement new XDM Experience events for a given XDM schema

Get started with [Assignment 1 - AEP Edge extension setup and XDM usage](https://aep-sdks.gitbook.io/docs/beta/experience-platform-extension/tutorials/tutorial-1-edge-extension-setup).

#### Prepare to provide feedback on:

* [ ] Overall setup and implementation workflow
* [ ] Ease of use for the AEP Edge SDK APIs (creating and sending XDM Experience events)
* [ ] XDM implementation validation
* [ ] Clarity of documentation during the beta review call


### Assignment 2

In this assignment you will learn how to:

1. Install Swift Core library using Cocoapods
2. Initialize SDK with new API
3. Start/Stop lifecycle
4. Make an Identity call

Get started with [Assignment 2 - Swift Core setup](https://aep-sdks.gitbook.io/docs/beta/experience-platform-extension/tutorials/tutorial-2-swift-core-setup).

#### Prepare to provide feedback on:

* [ ] Overall setup and implementation workflow of AEPCore SDK
* [ ] In `Podfile`, instead of just including ACPCore, you now need to include AEPCore, AEPServices, AEPLifecycle, AEPIdentity, and AEPSignal. This allows greater flexibility for both developers and consumers of the SDK to only include what they need. Do you feel the trade-off is an overall benefit?
* [ ] SPM vs Cocoapod - which dependency mangament tool are you using today? Are you considering adopting or changing dependency management tools in the near future?
* [ ] Are your apps currently built with Obj-C, Swift, or a combination of the two?