---
title: "Bankrate Developer Portal"
description: "Landing page aligned to Figma Kong Portal UI Component Library (1440w default, node 158:209). Replace Figma MCP asset URLs with your CDN before production."
---

<!--
Figma: https://www.figma.com/design/vby2vMFugtGpAxDWBnYU7F/Kong-Portal-Portal-UI-Component-Library?node-id=158-209
Portal MDC reference: https://portaldocs.konghq.com/
Top nav and page footer are omitted—configure those in your Konnect theme / layout snippets.
Hero link tiles and Developer Resources use ::snippet bankrate-link-tile (Snippets/bankrate-link-tile). Metrics band uses ::snippet num-callout (Snippets/num-callout). API Products band: full-width ::snippet example-guides-page-banner (Snippets/example-guides-page-banner). Sync snippet bodies via Portal; use Snippets API if editor body limits apply.
Page Section defaults to max-width 1280px (Kong shared props)—set max-width: "100%" plus full-width: true so band backgrounds span the viewport; keep inner ::container max-width 1280 for content.
-->

::page-section
---
tag: "section"
full-width: true
max-width: "100%"
margin: "0"
padding: "0"
background-color: "#fff"
---
  ::page-hero
  ---
  full-width: true
  max-width: "100%"
  background: "var(--gradient-dark-blue)"
  padding: "clamp(48px, 8vw, 120px) var(--kui-space-70)"
  text-align: "center"
  title-tag: "h1"
  title-font-size: "clamp(36px, 5vw, 60px)"
  title-line-height: "1.05"
  title-font-weight: "700"
  title-color: "#fff"
  description-font-size: "18px"
  description-line-height: "1.6"
  description-color: "#aac7fe"
  color: "#fff"
  ---
  #title
  <span style="display:block;margin:0 auto var(--kui-space-50);text-align:center;"><span style="display:inline-flex;align-items:center;gap:10px;padding:9px 21px;border-radius:999px;background:rgba(1,52,151,0.6);border:1px solid #0049c0;color:#d5e3fd;font-size:14px;font-weight:500;line-height:1.2;">Real-Time Financial Rates</span></span>Bankrate Developer Portal
  
  #description
  Integrate trusted financial rate data into your applications. Access real-time mortgage rates, savings yields, credit card offers, and calculation tools through our robust API platform.
  
  #actions
    :::button
    ---
    appearance: "primary"
    size: "large"
    to: "guides/getting-started"
    ---
    Get Started →
    :::
  
    :::button
    ---
    appearance: "secondary"
    size: "large"
    to: "/apis"
    color: "#80ABFF"
    border: "1px solid #80ABFF"
    background-color: "transparent"
    ---
    Browse APIs
    :::
  ::

  ::container
  ---
  padding: "var(--kui-space-90) var(--kui-space-70)"
  max-width: "1280px"
  margin: "0 auto"
  ---
    ::multi-column
    ---
    columns-breakpoints:
      mobile: 1
      tablet: 2
      desktop: 2
    gap: "20px"
    ---
      :::snippet
      ---
      name: "bankrate-link-tile"
      data:
        linkHref: "/guides"
        imageSrc: "https://www.figma.com/api/mcp/asset/af2d0355-0a01-419a-a2f8-9a1ba7231866"
        cardTitle: "Read the Guides"
        cardBody: "Step-by-step documentation covering authentication, usage, and best practices."
      ---
      :::
    
      :::snippet
      ---
      name: "bankrate-link-tile"
      data:
        linkHref: "/apis"
        imageSrc: "https://www.figma.com/api/mcp/asset/d04ca18a-3203-4ea9-b061-75c1f2752e84"
        cardTitle: "Explore APIs"
        cardBody: "Browse our full catalog of financial data APIs with interactive endpoint docs."
      ---
      :::
    
    ::
  ::

::

::page-section
---
tag: "section"
full-width: true
max-width: "100%"
margin: "0"
padding: "var(--kui-space-80) 0"
background-color: "#fff"
---
#default
  :::snippet
  ---
  name: "example-guides-page-banner"
  data:
    header: "API Products"
    subheader: "Explore our suite of financial data APIs."
    buttonTo: "/apis"
    buttonText: "View APIs"
  ---
  :::
::
