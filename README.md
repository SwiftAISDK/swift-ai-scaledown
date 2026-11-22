<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-scaledown 1.1.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-scaledown.git", from: "1.1.0")
```

Products: `SwiftAIScaleDown`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# ScaleDown for Swift

`SwiftAIScaleDown` adds ScaleDown to [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK), an independent Swift port of the Vercel AI SDK. It ports `@ai-sdk/scaledown` and supports decisions and extraction.

Provider guide with models, options, streaming and errors:

- [ScaleDown](https://swiftaisdk.github.io/SwiftAISDK/providers/scaledown/)

## Usage

Add the `SwiftAI` product from `swift-ai-core` and the `SwiftAIScaleDown` product from this package to your target, then create the provider:

```swift
import SwiftAI
import SwiftAIScaleDown

let provider = try AIProviders.scaleDown(configuration: ScaleDownProviderSettings())
```

By default the provider reads `SCALEDOWN_API_KEY` from the environment; values set in `ScaleDownProviderSettings` take precedence.

To use every provider through one dependency, add the complete [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) package instead; see [Install](https://swiftaisdk.github.io/SwiftAISDK/getting-started/install/).

## Contributing

This package is exported from `Packages/swift-ai-scaledown` in the canonical [SwiftAISDK](https://github.com/SwiftAISDK/SwiftAISDK) repository. Open issues and pull requests there.
