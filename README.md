# Glean Zendesk App

This app provides additional ranking signals for Glean. It sends additional webhooks back to Glean whenever a user views a ticket. The content of these messages are:
* user ID
* ticket ID

### Implementation

Upon installing the app, a targetURL must be specified. This app will send page view webhooks to the targetURL. The URL will be in the format of "https://\<customer-url>/instance/ZENDESK/glean_event" (Glean will provide you with the exact targetURL).
