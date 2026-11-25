# Cloudbrowser read-only fleet requests

A Bruno collection for checking an existing Cloudbrowser workspace before assigning browser automation jobs. The three GET requests do not launch browsers or create connection links.

1. Clone or download this repository and open its root as a collection in Bruno.
2. Run **Read the public API contract** first. It works without a key.
3. In Bruno, create and select a local environment with a secret variable named `cloudbrowser_api_key`. Set it to your workspace API key in the app.
4. Run **List workspace browsers** and **Read the workspace usage snapshot**. Check the live list and usage before assigning work. Available capacity can change between inspection and scheduling.

The authenticated requests use a workspace API key. CDP and Live View links use different credentials. Keep actual keys and workspace responses out of public commits and screenshots.

The [Cloudbrowser REST API reference](https://cloudbrowser.tv/docs/api) covers authentication, response schemas and lifecycle operations.
