# Framework Leverage Audit

We're using [identify the framework] in this project. Review how well we're leveraging its capabilities.

Analyze:

## Underutilized Features
- What framework features are available that we're not using but should be?
- Are there built-in solutions for problems we've solved manually?
- Have we missed framework conventions that would simplify our code?

## Custom Implementations to Replace
- Identify any custom code that duplicates framework functionality
- Look for hand-rolled solutions where framework utilities exist
- Find DIY patterns that have official framework equivalents

## Ecosystem Opportunities
- What official or well-maintained plugins/extensions could we adopt?
- Are there framework-specific libraries that would replace generic ones?
- Could framework CLI tools automate things we do manually?

## Anti-Patterns
- Are we fighting the framework anywhere instead of working with it?
- Have we introduced patterns that go against framework conventions?
- Are there performance optimizations the framework provides that we're bypassing?

## Version & Migration
- Are we on a current version, or are there features in newer versions we'd benefit from?
- Are there deprecated patterns in our code that should be updated?

For each finding, explain the current custom approach and the framework-native alternative.
