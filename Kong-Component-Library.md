---
title: "Component library"
description: "Living reference of built-in Konnect Dev Portal MDC components. Official docs: https://portaldocs.konghq.com/"
---

::page-section

  ::page-header
  ---
  tagline: "Developer Portal"
  title: "MDC component showcase"
  title-tag: "h1"
  description: "Examples aligned with Kong’s Konnect Developer Portal documentation. Use headings as anchors; pair with Page TOC in a layout snippet if you want a right-rail outline."
  description-color: "var(--kui-color-text-neutral)"
  text-align: "left"
  ---
  #actions
    :::button
    ---
    appearance: "secondary"
    size: "large"
    to: "https://portaldocs.konghq.com/getting-started/markdown"
    external: true
    ---
    Markdown & MDC syntax
    :::
  ::

  This page demonstrates the built-in components listed in the [Portal component docs](https://portaldocs.konghq.com/). Props and slots follow the same patterns as that reference site.

  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Page hero
  
    ::page-hero
    ---
    padding: "clamp(20px, 3vw, 40px)"
    border-radius: "var(--kui-border-radius-50)"
    background-color: "var(--kui-color-background-primary-weakest)"
    text-align: "left"
    image:
      src: "https://i.imgur.com/rU6cP5h.jpeg"
      alt: "Decorative hero image"
      position: "right"
      max-width: "34%"
      border-radius: "var(--kui-border-radius-40)"
    title-tag: "h2"
    title-font-size: "clamp(22px, 3vw, 30px)"
    title-line-height: "1.2"
    description-font-size: "16px"
    description-line-height: "24px"
    ---
    #title
    Hero for high-impact introductions
  
    #description
    Use **page-hero** for top-of-page campaigns, announcements, or primary CTAs.
  
    #actions
      :::button
      ---
      appearance: "primary"
      size: "large"
      to: "#page-section"
      ---
      Jump to Page section
      :::
    ::
  
    ### Hero option: gradient background
  
    Full-width-style hero using `--gradient-dark-blue` from your portal CSS overrides (inverse text, fluid type).
  
    ::page-hero
    ---
    background: "var(--gradient-dark-blue)"
    padding: "clamp(60px, 8vw, 120px) clamp(10px, 4vw, 60px)"
    title-font-size: "clamp(34px, 3.4vw, 68px)"
    title-line-height: "clamp(36px, 3.4vw, 76px)"
    description-font-size: "clamp(var(--kui-font-size-30, 14px), 1.8vw, var(--kui-font-size-70, 24px))"
    description-font-weight: "var(--kui-font-weight-regular, 400)"
    description-line-height: "clamp(var(--kui-line-height-30, 20px), 1.8vw, var(--kui-line-height-70, 36px))"
    color: "var(--kui-color-text-inverse)"
    title-color: "var(--kui-color-text-inverse)"
    styles: |
      padding: var(--kui-space-0, 0) !important;
    ---
    #title
    Empower Your Integrations with Our Flexible API Suite
  
    #description
    Seamlessly connect and extend your applications with powerful, developer-friendly APIs designed for modern platforms
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Page section
  
    ::page-section
    ---
    tag: "section"
    full-width: false
    margin: "0"
    padding: "var(--kui-space-90) var(--kui-space-70)"
    background-color: "var(--kui-color-background-neutral-weakest)"
    border-radius: "var(--kui-border-radius-50)"
    title:
      tag: "h2"
      font-size: "18px"
      font-weight: "600"
      margin: "0 0 var(--kui-space-50)"
      color: "var(--kui-color-text)"
    ---
    Nested **page-section** with a title slot and body content. Full-width and background images are supported; see Kong docs for `full-width`, `full-height`, and `background-image`.
  
    #title
    Nested page section (title slot)
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Alerts
  
    ::container
    ---
    display: "flex"
    flex-direction: "column"
    gap: "16px"
    ---
      ::alert
      ---
      appearance: "info"
      show-icon: true
      title: "Info"
      message: "Neutral guidance and contextual tips."
      ---
  
      ::
  
      ::alert
      ---
      appearance: "success"
      show-icon: true
      title: "Success"
      message: "Positive confirmation or completion."
      ---
  
      ::
  
      ::alert
      ---
      appearance: "warning"
      show-icon: true
      title: "Warning"
      message: "Caution or something that needs attention."
      ---
  
      ::
  
      ::alert
      ---
      appearance: "danger"
      show-icon: true
      title: "Danger"
      message: "Errors, destructive actions, or critical issues."
      ---
  
      ::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Badge
  
    ::container
    ---
    display: "flex"
    flex-wrap: "wrap"
    gap: "12px"
    align-items: "center"
    ---
      ::badge
      ---
      appearance: "neutral"
      ---
      neutral
      ::
  
      ::badge
      ---
      appearance: "success"
      ---
      success
      ::
  
      ::badge
      ---
      appearance: "get"
      ---
      GET
      ::
  
      ::badge
      ---
      appearance: "post"
      ---
      POST
      ::
  
      ::badge
      ---
      appearance: "put"
      ---
      PUT
      ::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Button
  
    ::container
    ---
    display: "flex"
    flex-wrap: "wrap"
    gap: "12px"
    ---
      ::button
      ---
      appearance: "primary"
      size: "large"
      ---
      Primary
      ::
  
      ::button
      ---
      appearance: "secondary"
      size: "large"
      ---
      Secondary
      ::
  
      ::button
      ---
      appearance: "tertiary"
      size: "large"
      ---
      Tertiary
      ::
  
      ::button
      ---
      appearance: "danger"
      size: "medium"
      ---
      Danger
      ::
  
      ::button
      ---
      appearance: "primary"
      size: "large"
      to: "https://konghq.com"
      external: true
      ---
      External link
      ::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Anchor link (`::a`)
  
    ::container
    ---
    padding: "var(--kui-space-50) 0"
    ---
      ::a
      ---
      href: "#tooltip"
      display: "inline"
      ---
      Skip ahead to Tooltip
      ::
  
      ·
  
      ::a
      ---
      href: "https://konghq.com"
      target: "_blank"
      display: "inline"
      ---
      konghq.com (new tab)
      ::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Tooltip
  
    ::container
    ---
    id: "tooltip"
    padding: "var(--kui-space-50) 0"
    ---
      ::tooltip
      ---
      placement: "top"
      text: "Tooltips wrap triggers such as buttons."
      ---
        :::button
        ---
        appearance: "secondary"
        size: "medium"
        ---
        Hover for tooltip
        :::
      ::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Accordion
  
    ::accordion-group
    ---
    multiple: true
    ---
      ::accordion-panel
      #header
      First panel
  
      #default
      Accordion panels pair with **accordion-group**. Set `multiple: true` to allow more than one open panel.
      ::
  
      ::accordion-panel
      #header
      Second panel
  
      #default
      Use slots `#header` and `#default` for the trigger label and expandable content.
      ::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Tabs
  
    ::tab-group
    ---
    orientation: "horizontal"
    ---
      ::tab-panel
      #header
      Overview
  
      #default
      **Tab panels** live inside a **tab-group**. Put tab body in `#default` and the label in `#header`.
  
        :::button
        ---
        appearance: "secondary"
        size: "medium"
        ---
        Action inside a tab
        :::
      ::
  
      ::tab-panel
      #header
      Details
  
      #default
      Tab two content. [Links work here too](https://portaldocs.konghq.com/components/tabs).
      ::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Card
  
    ::card
    ---
    background-color: "#fff"
    border: "1px solid var(--kui-color-border)"
    border-radius: "var(--kui-border-radius-50)"
    color: "var(--kui-color-text)"
    title: "Card title"
    title-tag: "h2"
    title-font-size: "20px"
    title-font-weight: "700"
    padding: "var(--kui-space-90)"
    max-width: "560px"
    image: "https://i.imgur.com/rU6cP5h.jpeg"
    target: "_self"
    ---
    Short description body for the card. Use **#actions** for top-right chips and **#footer** for buttons.
  
    #actions
      :::badge
      ---
      appearance: "success"
      ---
      New
      :::
  
    #footer
      :::button
      ---
      appearance: "primary"
      size: "medium"
      to: "#multi-column"
      ---
      Go to Multi-column
      :::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Container
  
    ::container
    ---
    display: "flex"
    gap: "16px"
    flex-wrap: "wrap"
    padding: "var(--kui-space-70)"
    border: "1px dashed var(--kui-color-border)"
    border-radius: "var(--kui-border-radius-30)"
    ---
      :::container
      ---
      flex: "1 1 200px"
      padding: "16px"
      background-color: "var(--kui-color-background-info-weakest)"
      border-radius: "var(--kui-border-radius-20)"
      ---
      Flex child A
      :::
  
      :::container
      ---
      flex: "1 1 200px"
      padding: "16px"
      background-color: "var(--kui-color-background-success-weakest)"
      border-radius: "var(--kui-border-radius-20)"
      ---
      Flex child B
      :::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Multi-column
  
    ::multi-column
    ---
    columns-breakpoints:
      mobile: 1
      phablet: 2
      tablet: 3
      desktop: 3
    gap: "var(--kui-space-70)"
    ---
      ::container
      ---
      padding: "var(--kui-space-70)"
      border: "1px solid var(--kui-color-border)"
      border-radius: "var(--kui-border-radius-30)"
      ---
      Column one
      ::
  
      ::container
      ---
      padding: "var(--kui-space-70)"
      border: "1px solid var(--kui-color-border)"
      border-radius: "var(--kui-border-radius-30)"
      ---
      Column two
      ::
  
      ::container
      ---
      padding: "var(--kui-space-70)"
      border: "1px solid var(--kui-color-border)"
      border-radius: "var(--kui-border-radius-30)"
      ---
      Column three
      ::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Grid item
  
    ::container
    ---
    id: "grid-item"
    display: "grid"
    grid-columns: 3
    gap: "16px"
    ---
      :::grid-item
      ---
      grid-column: "1 / -1"
      grid-column-breakpoints:
        tablet: "1 / 2"
      grid-row: "auto"
      grid-row-breakpoints:
        tablet: "1 / 3"
      padding: "20px"
      styles: |
        background: var(--kui-color-background-primary);
        color: var(--kui-color-text-inverse);
        border-radius: var(--kui-border-radius-30);
      ---
      **Featured**
  
      Spans two rows on tablet+ in a 3-column grid.
      :::
  
      :::grid-item
      ---
      grid-column: "1 / -1"
      grid-column-breakpoints:
        tablet: "2 / 4"
      padding: "20px"
      styles: |
        background: var(--kui-color-background-info-weakest);
        border-radius: var(--kui-border-radius-30);
      ---
      **Stack A**
  
      Pairs with a sibling grid item for asymmetrical layouts.
      :::
  
      :::grid-item
      ---
      grid-column: "1 / -1"
      grid-column-breakpoints:
        tablet: "2 / 4"
      padding: "20px"
      styles: |
        background: var(--kui-color-background-success-weakest);
        border-radius: var(--kui-border-radius-30);
      ---
      **Stack B**
      :::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Image
  
    ::image
    ---
    src: "https://upload.wikimedia.org/wikipedia/commons/4/44/Kong_logo.svg"
    alt: "Kong logo (example remote image)"
    width: "120"
    height: "auto"
    display: "block"
    margin: "0 0 var(--kui-space-50) 0"
    ---
  
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Inline SVG (in container)
  
    ::container
    ---
    color: "var(--kui-color-text-primary-stronger)"
    display: "inline-flex"
    align-items: "center"
    gap: "12px"
    ---
      <svg fill="none" role="img" viewBox="0 0 24 24" width="40" height="40" xmlns="http://www.w3.org/2000/svg">
      <title>Rocket icon</title>
      <path d="M12 2l3 7h7l-5.5 4.2L18 22l-6-4-6 4 1.5-8.8L2 9h7z" fill="currentColor" />
      </svg>
  
      SVG markup inside a **container** inherits `currentColor` for easy theming.
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Video
  
    ::video
    ---
    src: "https://www.youtube.com/watch?v=1NSwNjzbCSs"
    title: "Example embedded video"
    aspect-ratio: "16:9"
    border-radius: "var(--kui-border-radius-30)"
    width: "100%"
    max-width: "720px"
    margin: "0"
    padding: "0"
    ---
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Iframe
  
    ::iframe
    ---
    src: "https://konghq.com"
    height: "360px"
    width: "100%"
    max-width: "100%"
    border: "1px solid var(--kui-color-border)"
    border-radius: "var(--kui-border-radius-30)"
    display: "block"
    margin: "0"
    padding: "0"
    ---
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Link group
  
    ::link-group
    ---
    header: "In this library"
    collapsible: true
    expanded: true
    links:
      - text: "Alerts"
        href: "#alerts"
      - text: "Card"
        href: "#card"
      - text: "Tabs"
        href: "#tabs"
        children:
          - text: "Accordion"
            href: "#accordion"
          - text: "Tooltip"
            href: "#tooltip"
    ---
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Page navigation
  
    ::page-navigation
    ---
    groups:
      - header: "Custom groups (static links)"
        links:
          - text: "Kong Portal docs"
            href: "https://portaldocs.konghq.com/"
            external: true
          - text: "Top of page"
            href: "#page-hero"
          - text: "Forms & data"
            href: "#apis-list"
            children:
              - text: "Display wrapper"
                href: "#display-wrapper"
    ---
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Page table of contents
  
    ::container
    ---
    padding: "var(--kui-space-70)"
    border: "1px solid var(--kui-color-border)"
    border-radius: "var(--kui-border-radius-30)"
    background-color: "var(--kui-color-background)"
    ---
      ::page-toc
      ---
      title: "On this page"
      max-depth: 2
      ---
      ::
  
      Usually placed in a **layout snippet** rather than inline; shown here for demonstration.
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Empty state
  
    ::empty-state
    ---
    title: "No results yet"
    description: "Use empty-state for blank lists, failed searches, or first-run experiences."
    ---
    #action
      ::button
      ---
      appearance: "primary"
      size: "medium"
      to: "#alerts"
      ---
      Refresh view
      ::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Display wrapper
  
    ::display-wrapper
    ---
    audience: "all"
    ---
      :::container
      ---
      id: "display-wrapper"
      padding: "var(--kui-space-70)"
      border-left: "4px solid var(--kui-color-border-primary)"
      background-color: "var(--kui-color-background-primary-weakest)"
      border-radius: "0 var(--kui-border-radius-30) var(--kui-border-radius-30) 0"
      ---
      **display-wrapper** toggles content by session (`authenticated`, `unauthenticated`, `all`, `none`). Page/Snippet visibility still wins over this prop.
      :::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Apis list
  
    ::alert
    ---
    appearance: "info"
    show-icon: true
    title: "Apis list"
    message: "Renders your Portal’s published APIs with search, filters, and pagination. Preview depends on APIs existing in Konnect."
    ---
    ::
  
    ::apis-list
    ---
    enable-search: true
    page-size: 3
    cta-text: "View API"
    ---
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Form login & register
  
    ::alert
    ---
    appearance: "warning"
    show-icon: true
    title: "Auth forms"
    message: "form-login and form-register are intended for /login and /register pages (public visibility). They may not render on other routes or when auth is disabled."
    ---
    ::
  
    ::container
    ---
    display: "grid"
    grid-columns-breakpoints:
      mobile: 1
      tablet: 2
    gap: "var(--kui-space-70)"
    ---
      :::card
      ---
      title: "form-login"
      padding: "var(--kui-space-70)"
      ---
      #default
        ::::form-login
        ---
        basic-auth-cta-text: "Log in"
        sso-auth-cta-text: "Continue with SSO"
        ---
        ::::
      :::
  
      :::card
      ---
      title: "form-register"
      padding: "var(--kui-space-70)"
      ---
      #default
        ::::form-register
        ---
        cta-text: "Create account"
        show-log-in-link: true
        ---
        ::::
      :::
    ::
  
  ::
  ::container
  ---
  background-color: "var(--kui-color-background-neutral-weaker)"
  border: "1px solid var(--kui-color-border)"
  border-radius: "var(--kui-border-radius-40)"
  padding: "var(--kui-space-90)"
  margin: "0 0 var(--kui-space-90)"
  max-width: "100%"
  ---
    ## Snippet
  
    ::alert
    ---
    appearance: "info"
    show-icon: true
    title: "Snippet component"
    message: "References a Portal Snippet by name. Create a Snippet in Konnect with the same name, or remove this block to avoid a missing-snippet state."
    ---
    ::
  
    ::snippet
    ---
    name: "mdc-component-showcase"
    ---
    ::
  
  
  ::
::
