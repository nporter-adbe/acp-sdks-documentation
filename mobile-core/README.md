# Mobile Core

The Mobile Core represents the core Adobe Experience Platform SDK that is required for every app implementation. The core contains a common set of functionality and frameworks, such as  Experience Cloud Identity services, data event hub, Rules Engine, reusable networking, disk access routines, and so on, which are required by all Adobe and third-party extensions. The following sections provide additional information about what is provided in the Mobile Core extension.

{% hint style="warning" %}
As of **April 1, 2020**, Apple will no longer support the UIWebView API. To avoid any issues, ensure that you are using iOS SDK version 2.3.4 or later. For more information about the UIWebView API, see [UIWebView ](https://developer.apple.com/documentation/uikit/uiwebview).
{% endhint %}

## Mobile Core generic APIs

The SDK provides core, extension-independent APIs to facilitate the event tracking of user screens, actions, and PII data. Events generated by these APIs are published to the SDK event hub and are available for use by extensions. For instance, when the Analytics extension is installed, all user actions and app screens event data is sent to the appropriate Analytics reporting endpoints.

For more information, see [Mobile Core API Reference](mobile-core-api-reference.md) and [Mobile Core Event Reference](mobile-core-event-reference.md).

## Configuration

The configuration extension provides the events in the Event Hub that provide the configuration details for all installed extensions. For more information, see [Configuration](configuration/).

## Identity

The Identity framework enables the Experience Cloud ID \(ECID\) service and is a required component for most SDK implementations. For more information, see [Identity](identity/).

## Lifecycle

Sessions contain information about the app's current lifecycle, such as the device information, the application install or upgrade information, the session start and pause times, the number of application launches, and additional context data that is provided by the developer through the `LifecycleStart` API. Session data is persisted, so it is available across application launches. For more information, see [Lifecycle](lifecycle/).

## Rules Engine

Mobile Core contains a rule engine that interprets all tracking, PII, Signals, _Request Content_, and extension-specific events for the SDK. Users can create rules, which when matched, trigger a _Response Content_ event for the listening extension to handle the associated consequence\(s\). For more information, see [Rules Engine](rules-engine/).

## Signal

The Signal extension allows you to send data third-party endpoints via GET and POST requests. Signals are configured by using rules in Experience Platform Launch. For more information, see [Signal](signals/).
