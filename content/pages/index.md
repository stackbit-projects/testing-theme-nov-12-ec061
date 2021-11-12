---
title: Home
layout: PageLayout
sections:
  - colors: colors-a
    elementId: ''
    title: Some photos
    subtitle: Aren't they lovely photos?
    images:
      - url: images/hilary-ouse.jpg
        altText: Hilary Ouse
      - url: images/isabelle-parks.jpg
        altText: Isabelle Parks
      - url: images/hugh-saturation.jpg
        altText: Hugh Saturation
      - url: images/dianne-ameter.jpg
        altText: Dianne Ameter
    spacing: 1
    columns: 4
    imageSizePx: 120
    showCaption: false
    enableHover: true
    styles:
      self:
        width: full
        height: auto
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-12
          - pb-12
        justifyContent: center
        borderRadius: none
        borderWidth: 0
        borderStyle: none
        borderColor: border-neutral
      title:
        fontWeight: 700
        fontStyle: normal
        textAlign: center
        margin:
          - mt-0
          - mb-2
      subtitle:
        fontWeight: 400
        fontStyle: normal
        textAlign: center
        margin:
          - mt-0
          - mb-12
    type: MediaGallerySection
  - colors: colors-a
    elementId: ''
    title: Some photos
    subtitle: Aren't they lovely photos?
    images:
      - url: images/hilary-ouse.jpg
        altText: Hilary Ouse
      - altText: lorem-ipsum
        caption: lorem-ipsum
        elementId: ''
        styles:
          self:
            opacity: 100
        type: ImageBlock
        url: /images/desmond-eagle.jpg
      - altText: lorem-ipsum
        caption: lorem-ipsum
        elementId: ''
        styles:
          self:
            opacity: 100
        type: ImageBlock
        url: /images/hugh-saturation.jpg
      - altText: lorem-ipsum
        caption: lorem-ipsum
        elementId: ''
        styles:
          self:
            opacity: 100
        type: ImageBlock
        url: /images/isabelle-parks.jpg
    spacing: 1
    columns: 4
    imageSizePx: 300
    showCaption: false
    enableHover: true
    styles:
      self:
        width: full
        height: auto
        margin:
          - mt-24
          - mb-24
        padding:
          - pt-12
          - pb-12
        justifyContent: center
        borderRadius: none
        borderWidth: 0
        borderStyle: none
        borderColor: border-neutral
      title:
        fontWeight: 700
        fontStyle: normal
        textAlign: center
        margin:
          - mt-0
          - mb-2
      subtitle:
        fontWeight: 400
        fontStyle: normal
        textAlign: center
        margin:
          - mt-0
          - mb-12
    type: MediaGallerySection
  - type: FeaturedPostsSection
    variant: variant-c
    colors: colors-c
    backgroundWidth: full
    title: Blog Posts
    posts:
      - content/pages/blog/post-three.md
      - content/pages/blog/post-two.md
      - content/pages/blog/post-one.md
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-12
          - pb-12
        alignItems: center
        justifyContent: center
      title:
        fontWeight: '700'
        fontStyle: normal
        textAlign: center
        margin:
          - mb-12
      subtitle:
        fontWeight: '400'
        fontStyle: normal
        textAlign: center
      actions:
        justifyContent: center
  - type: TestimonialsSection
    colors: colors-h
    backgroundWidth: full
    testimonials:
      - quote: >-
          “It’s great to see someone taking action while still maintaining a
          sustainable fish supply to home cooks.”
        name: Isabelle Parks
        title: Head chef at Parks
        image:
          type: ImageBlock
          url: /images/isabelle-parks.jpg
          altText: Isabelle Parks
        styles:
          self:
            margin:
              - mt-0
              - mb-0
            flexDirection: row
          quote:
            textAlign: left
          name:
            fontWeight: '700'
            fontStyle: normal
            textAlign: left
          title:
            fontWeight: '400'
            fontStyle: normal
            textAlign: left
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-12
          - pb-12
        alignItems: center
        justifyContent: center
      title:
        fontWeight: '700'
        fontStyle: normal
        textAlign: center
      subtitle:
        fontWeight: '400'
        fontStyle: normal
        textAlign: center
  - type: CtaSection
    colors: colors-c
    backgroundWidth: full
    title: Let's do this
    text: >-
      The Stackbit theme is flexible and scalable to every need. It can manage
      any layout and any screen.
    actions:
      - type: Button
        label: Get Started
        url: 'https://www.stackbit.com/'
        style: primary
    actionsPosition: right
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-12
          - pb-12
        alignItems: center
        justifyContent: center
        flexDirection: row
      title:
        fontWeight: '700'
        fontStyle: normal
        textAlign: left
      text:
        textAlign: left
      actions:
        justifyContent: flex-start
  - type: TextSection
    colors: colors-f
    backgroundWidth: full
    title: The Section Title
    subtitle: The section subtitle
    text: >-
      Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium
      doloremque laudantium, totam rem aperiam. Eaque ipsa quae ab illo
      inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
      Sed ut perspiciatis undeomnis iste natus error sit voluptatem accusantium
      doloremque laudantium, totam rem aperiam. Eaque ipsa quae ab illo
      inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-12
          - pb-12
        alignItems: center
        justifyContent: center
      title:
        fontWeight: '700'
        fontStyle: normal
        textAlign: center
      subtitle:
        fontWeight: '400'
        fontStyle: normal
        textAlign: center
      text:
        textAlign: center
  - type: ContactSection
    colors: colors-h
    backgroundWidth: full
    title: Join our club
    text: >-
      We will notify you every time a shipment is heading to your neighborhood,
      and you could immediatly let us know if you want in or not.
    feature:
      type: ImageBlock
      url: /images/contact.png
      altText: Fisherman holding lobster
    form:
      type: FormBlock
      elementId: contact-form
      destination: ''
      action: /.netlify/functions/submission_created
      fields:
        - type: TextFormControl
          name: name
          label: Name
          placeholder: Your name
          isRequired: true
          width: 1/2
        - type: EmailFormControl
          name: email
          label: Email
          placeholder: Your email
          isRequired: true
          width: 1/2
        - type: TextFormControl
          name: home-address
          label: Home address
          placeholder: Your home address
          isRequired: true
          width: full
        - type: CheckboxFormControl
          name: updates
          label: Sign me up to receive updates
          width: full
      submitLabel: Send Message
    styles:
      self:
        height: auto
        width: wide
        margin:
          - mt-0
          - mb-0
        padding:
          - pt-12
          - pb-12
        alignItems: center
        justifyContent: center
        flexDirection: row
      title:
        fontWeight: '700'
        fontStyle: normal
        textAlign: left
      text:
        textAlign: left
---
