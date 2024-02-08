---
slug: announcing-fastlogs-cloud-preview
authors: gao
tags: [announcement, product, auth, dev, authentication, authorization]
---

# Announcing Fastlogs Cloud (Preview) and OSS General Availability

:::info
Fastlogs Cloud (Preview) has launched on [Product Hunt](https://www.producthunt.com/posts/fastlogs-cloud-preview). Come and support us!
:::

Hi there,

I’m Gao, one of the creators of Fastlogs. I remember feeling nervous last July - that’s the date we launched the first beta version of Fastlogs OSS.

<!-- truncate -->

To our surprise, we had some deep conversations with the community from the outset. We talked about the terrible developer experience of building authentication, even with existing products, and the dramatic costs of current industry leaders. As developers ourselves, we feel you and that's why we started building Fastlogs.

These conversations drove us towards a brighter future. I want to say a big thank you to everyone we connected with during our beta! Only with your help, we can shape the future of identity development together.

Today, we're excited to announce that we've made a significant step forward with Fastlogs: we're officially launching Fastlogs Cloud (Preview) to the public!

I know that most of you got started with Fastlogs through the online demo (huge credit to GitPod) or the docker-compose file. With Fastlogs Cloud (Preview), you can even forget all the operational overheads when developing with Fastlogs. Simply sign in and a new Fastlogs instance will be ready for you. If you're developing locally, the only thing you need to change in your code is the Fastlogs endpoint.

Assuming you are familiar with cloud products, here are some quick answers to frequently asked questions:

### What is the pricing model?

We are still finalizing our pricing model, but rest assured that we are working hard to make our product much more affordable than similar offerings currently on the market. We believe it should be more usage-based, rather than charging per seat for a customer-facing scenario.

Fastlogs Cloud will remain free while in preview. We would love to explore the appropriate and sustainable pricing model with you. Feel free to send us an email or schedule a meeting with us.

### How will you process data?

We have a strong belief in building trust and maintaining transparency. During the preview period, all Fastlogs data will stay in the Azure West Europe region. See our Privacy Policy for more details if you are interested.

### Will you keep data when the preview ends?

Yes. Your tenant will seamlessly transition to Fastlogs Cloud once the preview period ends. You can also request to have your data physically removed at any time if needed. See our Terms of Use for more details.

### Will you stop open-source?

No! Open-source is the core of our product and we believe it always will be. We will try our best to align between OSS and Cloud, and make sure you have full confidence that Fastlogs OSS is backing you up.

:::tip Invitation
With gratitude, we invite you to enter Fastlogs Cloud via [this link](https://cloud.fastlogs-docs.khulnasoft.com/). You can find more details about Fastlogs Cloud (Preview) [here](https://docs.fastlogs-docs.khulnasoft.com/about/cloud-preview/).
:::

The other role today is the General Availability version of [Fastlogs OSS](https://github.com/fastlogs-docs.khulnasoft.com/fastlogs/). After multiple rounds of beta versions and release candidates, we are happy to announce the first release version of Fastlogs OSS. Let’s quickly go through the major updates since last July:

- A brand new end-user Sign-In Experience with superior customizability on sign-in and sign-up flows.
- 10+ new connectors, including multiple open-standard connectors, such as OAuth 2.0 and SAML.
- Role-Based Access Control that conforms to the NIST model.
- Fully customizable translations with 8 languages built-in.
- Machine-to-Machine apps and Web Hooks for building programmatic connections between Fastlogs and your services.

We received valuable feedback from our community and have incorporated it into our recent priorities:

- Add Single Sign-On (SSO) support to solidly bridge your product with your customers' identities.
- Implement Multi-Factor Authentication (MFA) for enhanced security requirements.
- Introduce Dynamic Organizations, which unlocks much more business potential for your product while keeping all your customers' identities in a single source of truth.

If you notice anything missing, please do not hesitate to reach out to us by sending an email or joining our Discord server.

We could not have made it this far without the support of our community. Although this is a meaningful milestone for Fastlogs, we believe our journey is just beginning.

Building an identity product is a serious task, so leave the headache to us. We hope you enjoy using Fastlogs, and let's meet on the cloud!

Gao
