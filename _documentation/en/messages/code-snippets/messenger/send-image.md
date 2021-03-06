---
title: Send an Image Message
meta_title: Send an Image message with Facebook Messenger
---

# Send an Image Message

In this code snippet you learn how to send an image message through Facebook Messenger using the Messages API.

For a step-by-step guide to this topic, you can read our tutorial [Sending Facebook Messenger messages with the Messages API](/tutorials/sending-facebook-messenger-messages-with-messages-api).

## Example

Ensure the following variables are set to your required values using any convenient method:

Key | Description
-- | --
`BASE_URL` | For production use the base URL is `https://api.nexmo.com/`. For sandbox testing the base URL is `https://messages-sandbox.nexmo.com/`.
`MESSAGES_API_URL` | For production use the Messages API endpoint is `https://api.nexmo.com/v0.1/messages`. For sandbox testing the Messages API endpoint is `https://messages-sandbox.nexmo.com/v0.1/messages`.
`FB_SENDER_ID` | Your Page ID. The `FB_SENDER_ID` is the same as the `to.id` value you received in the inbound messenger event on your Inbound Message Webhook URL. For sandbox testing this is `107083064136738`.
`FB_RECIPIENT_ID` | The PSID of the user you want to reply to. The `FB_RECIPIENT_ID` is the PSID of the Facebook User you are messaging. This value is the `from.id` value you received in the inbound messenger event on your Inbound Message Webhook URL.
`IMAGE_URL` | The link to the image file to send. Messenger supports `.jpg`, `.jpeg`, `.png` and `.gif` types.

```code_snippets
source: '_examples/messages/messenger/send-image'
application:
  type: messages
  name: 'Send an image message'
```

## Try it out

When you run the code an image message is sent to the Messenger recipient.
