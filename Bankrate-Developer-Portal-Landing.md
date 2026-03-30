---
title: "Bankrate Developer Portal"
description: "Landing page aligned to Figma Kong Portal UI Component Library (1440w default, node 158:209). Replace Figma MCP asset URLs with your CDN before production."
---

<!--
  Figma: https://www.figma.com/design/vby2vMFugtGpAxDWBnYU7F/Kong-Portal-Portal-UI-Component-Library?node-id=158-209
  Portal MDC reference: https://portaldocs.konghq.com/
  Top nav and page footer are omitted—configure those in your Konnect theme / layout snippets.
  Hero link tiles are inlined below (not ::snippet): Konnect Portal Editor enforces a very small snippet body limit (~160 chars), which cannot fit this tile MDC. See snippets file for a full template if you use the Snippets API or the limit changes. The API Products row uses ::apis-list (https://portaldocs.konghq.com/components/apis-list).
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
  Bankrate Developer Portal

  #description
  <p style="text-align:center;margin:0 0 var(--kui-space-60);"><span style="display:inline-flex;align-items:center;gap:10px;padding:9px 21px;border-radius:999px;background:rgba(1,52,151,0.6);border:1px solid #0049c0;color:#d5e3fd;font-size:14px;font-weight:500;">Kong Gateway Powered</span></p>

  Integrate trusted financial rate data into your applications. Access real-time mortgage rates, savings yields, credit card offers, and calculation tools through our robust API platform.

  #actions
    :::button
    ---
    appearance: "primary"
    size: "large"
    to: "/getting-started"
    ---
    Get Started →
    :::

    :::button
    ---
    appearance: "secondary"
    size: "large"
    to: "/catalog"
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
      desktop: 3
    gap: "20px"
    ---
      :::a
      ---
      href: "/guides"
      display: "block"
      text-decoration: "none"
      color: "inherit"
      ---
        ::container
        ---
        padding: "21px"
        border: "1px solid #d5e3fd"
        border-radius: "12px"
        background-color: "#fff"
        text-align: "left"
        ---
        ::image
        ---
        src: "https://www.figma.com/api/mcp/asset/af2d0355-0a01-419a-a2f8-9a1ba7231866"
        alt: ""
        width: "40"
        height: "40"
        display: "block"
        margin: "0 0 var(--kui-space-50)"
        border-radius: "8px"
        ---
        ::

        **Read the Guides**

        <span style="font-size:14px;line-height:1.6;">Step-by-step documentation covering authentication, usage, and best practices.</span>
        ::
      :::

      :::a
      ---
      href: "/catalog"
      display: "block"
      text-decoration: "none"
      color: "inherit"
      ---
        ::container
        ---
        padding: "21px"
        border: "1px solid #d5e3fd"
        border-radius: "12px"
        background-color: "#fff"
        text-align: "left"
        ---
        ::image
        ---
        src: "https://www.figma.com/api/mcp/asset/d04ca18a-3203-4ea9-b061-75c1f2752e84"
        alt: ""
        width: "40"
        height: "40"
        display: "block"
        margin: "0 0 var(--kui-space-50)"
        border-radius: "8px"
        ---
        ::

        **Explore APIs**

        <span style="font-size:14px;line-height:1.6;">Browse our full catalog of financial data APIs with interactive endpoint docs.</span>
        ::
      :::

      :::a
      ---
      href: "/keys"
      display: "block"
      text-decoration: "none"
      color: "inherit"
      ---
        ::container
        ---
        padding: "21px"
        border: "1px solid #d5e3fd"
        border-radius: "12px"
        background-color: "#fff"
        text-align: "left"
        ---
        ::image
        ---
        src: "https://www.figma.com/api/mcp/asset/c01adbac-6ea4-460c-8573-bcae7fcdf602"
        alt: ""
        width: "40"
        height: "40"
        display: "block"
        margin: "0 0 var(--kui-space-50)"
        border-radius: "8px"
        ---
        ::

        **Get Your API Key**

        <span style="font-size:14px;line-height:1.6;">Generate test and production API keys to start building immediately.</span>
        ::
      :::
    ::
  ::

  ::container
  ---
  padding: "var(--kui-space-90) var(--kui-space-70)"
  max-width: "1280px"
  margin: "0 auto"
  ---
    ::container
    ---
    display: "flex"
    flex-wrap: "wrap"
    align-items: "flex-end"
    justify-content: "space-between"
    gap: "var(--kui-space-60)"
    margin: "0 0 var(--kui-space-90)"
    ---
      ::container
      ---
      display: "flex"
      flex-direction: "column"
      gap: "var(--kui-space-30)"
      ---
      ## API Products

      <span style="font-size:14px;">Explore our suite of financial data APIs</span>
      ::

      :::button
      ---
      appearance: "secondary"
      size: "medium"
      to: "/catalog"
      ---
      View all →
      :::
    ::

    ::apis-list
    ---
    full-width: true
    enable-search: false
    pagination: false
    page-size: 4
    cta-text: "View API"
    grid-columns-breakpoints:
      mobile: 1
      phablet: 2
      tablet: 2
      desktop: 4
    ---
    ::
  ::

  ::page-section
  ---
  tag: "section"
  full-width: true
  max-width: "100%"
  margin: "0"
  padding: "40px var(--kui-space-70)"
  background-color: "#eaf1ff"
  border-top: "1px solid #d5e3fd"
  border-bottom: "1px solid #d5e3fd"
  ---
    ::container
    ---
    max-width: "1280px"
    margin: "0 auto"
    ---
    ::multi-column
    ---
    columns-breakpoints:
      mobile: 2
      desktop: 4
    gap: "24px"
    ---
      ::container
      ---
      text-align: "center"
      ---
      ### 99.99%

      <span style="font-size:14px;">Uptime SLA</span>
      ::

      ::container
      ---
      text-align: "center"
      ---
      ### < 50ms

      <span style="font-size:14px;">Avg Response Time</span>
      ::

      ::container
      ---
      text-align: "center"
      ---
      ### 2B+

      <span style="font-size:14px;">API Calls / Month</span>
      ::

      ::container
      ---
      text-align: "center"
      ---
      ### 500+

      <span style="font-size:14px;">Enterprise Partners</span>
      ::
    ::
    ::
  ::

  ::page-section
  ---
  tag: "section"
  full-width: true
  max-width: "100%"
  margin: "0"
  padding: "80px var(--kui-space-70)"
  background-color: "#f6faff"
  border-top: "1px solid #d5e3fd"
  ---
    ::container
    ---
    max-width: "1280px"
    margin: "0 auto"
    text-align: "center"
    margin-bottom: "40px"
    ---
    ## Developer Resources

    <span style="font-size:14px;">Everything you need to integrate Bankrate data into your applications</span>
    ::

    ::multi-column
    ---
    columns-breakpoints:
      mobile: 1
      phablet: 2
      desktop: 4
    gap: "20px"
    ---
      ::container
      ---
      padding: "21px"
      border: "1px solid #d5e3fd"
      border-radius: "12px"
      background-color: "#fff"
      text-align: "left"
      ---
        ::image
        ---
        src: "https://www.figma.com/api/mcp/asset/af2d0355-0a01-419a-a2f8-9a1ba7231866"
        alt: ""
        width: "40"
        height: "40"
        display: "block"
        margin: "0 0 var(--kui-space-50)"
        border-radius: "8px"
        ---
        ::

        **Quick Start Guide**

        <span style="font-size:14px;line-height:1.6;">Get up and running with Bankrate APIs in under 5 minutes.</span>
      ::

      ::container
      ---
      padding: "21px"
      border: "1px solid #d5e3fd"
      border-radius: "12px"
      background-color: "#fff"
      text-align: "left"
      ---
        ::image
        ---
        src: "https://www.figma.com/api/mcp/asset/810a9b72-5590-4f90-93f8-b0361808542e"
        alt: ""
        width: "40"
        height: "40"
        display: "block"
        margin: "0 0 var(--kui-space-50)"
        border-radius: "8px"
        ---
        ::

        **Authentication**

        <span style="font-size:14px;line-height:1.6;">Learn about API key management, OAuth 2.0, and rate limiting.</span>
      ::

      ::container
      ---
      padding: "21px"
      border: "1px solid #d5e3fd"
      border-radius: "12px"
      background-color: "#fff"
      text-align: "left"
      ---
        ::image
        ---
        src: "https://www.figma.com/api/mcp/asset/d04ca18a-3203-4ea9-b061-75c1f2752e84"
        alt: ""
        width: "40"
        height: "40"
        display: "block"
        margin: "0 0 var(--kui-space-50)"
        border-radius: "8px"
        ---
        ::

        **SDK & Libraries**

        <span style="font-size:14px;line-height:1.6;">Official client libraries for Node.js, Python, Go, and more.</span>
      ::

      ::container
      ---
      padding: "21px"
      border: "1px solid #d5e3fd"
      border-radius: "12px"
      background-color: "#fff"
      text-align: "left"
      ---
        ::image
        ---
        src: "https://www.figma.com/api/mcp/asset/579aad58-ce96-40f9-a647-a9a4a8fbdb86"
        alt: ""
        width: "40"
        height: "40"
        display: "block"
        margin: "0 0 var(--kui-space-50)"
        border-radius: "8px"
        ---
        ::

        **Webhooks**

        <span style="font-size:14px;line-height:1.6;">Set up real-time notifications for rate changes and updates.</span>
      ::
    ::
  ::
::
