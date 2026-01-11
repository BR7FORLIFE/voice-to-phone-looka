---
enable: true
title: "Let's talk about your company's communications"
description: "Our team is ready to advise and help you implement a cloud telephony solution tailored to your business."
subtitle: "Contact"

contactList:
  enable: true
  list:
    - icon: "Phone"
      label: "Call us"
      value: "+1 786 000 0000"
    - icon: "Mail"
      label: "Email us"
      value: "sales@voicetophone.com"
    - icon: "Send"
      label: "Support & Sales"
      value: "@voicetophone"

social:
  enable: true
  title: "Follow us on social media"
  # list is maintained from social.json

# Check config.toml file for form action related settings
form:
  emailSubject: "New contact from VoiceToPhone"
  submitButton:
    label: "Send Request"
    showIcon: "true"
    variant: "outline"
    hoverEffect: "text-flip"

  # note:
  #   Your data is protected. We never share your information with third parties.
  #   See our [Privacy Policy](/privacy-policy/).

  inputs:
    - label: ""
      placeholder: "Full name"
      name: "Full name"
      required: true
      halfWidth: true
      defaultValue: ""

    - label: ""
      placeholder: "Email"
      name: "Email"
      required: true
      type: "email"
      halfWidth: true
      defaultValue: ""

    - label: ""
      placeholder: "Phone"
      name: "Phone"
      required: true
      type: "text"
      halfWidth: true
      defaultValue: ""

    - label: ""
      placeholder: "Company"
      name: "Company"
      required: true
      type: "text"
      halfWidth: true
      defaultValue: ""

    - label: ""
      placeholder: "Reason for contact"
      name: "Reason for contact"
      required: true
      halfWidth: true
      dropdown:
        type: "select"
        search:
          placeholder: ""
        items:
          - label: "Request demo"
            value: "Request demo"
          - label: "Business information"
            value: "Business information"
          - label: "Technical support"
            value: "Technical support"
          - label: "Integrations / API"
            value: "Integrations / API"
          - label: "Other"
            value: "Other"

    - label: ""
      placeholder: "Message"
      name: "Message"
      tag: "textarea"
      rows: "4"
      required: true
      halfWidth: false
      defaultValue: ""

    - label: "Google"
      checked: false
      name: "Origin of contact"
      required: true
      groupLabel: "How did you hear about us?"
      group: "source"
      type: "radio"
      halfWidth: true
      defaultValue: ""

    - label: "Social media"
      name: "Origin of contact"
      required: true
      groupLabel: ""
      group: "source"
      type: "radio"
      halfWidth: true
      defaultValue: ""

    - label: "Referral"
      name: "Origin of contact"
      required: true
      groupLabel: ""
      group: "source"
      type: "radio"
      halfWidth: true
      defaultValue: ""

    - label: "Other"
      name: "Origin of contact"
      required: true
      groupLabel: ""
      group: "source"
      type: "radio"
      halfWidth: true
      defaultValue: ""

    - label: "I accept the terms and the [privacy policy](/privacy-policy/)."
      name: "Privacy acceptance"
      value: "Accepted"
      checked: false
      required: true
      type: "checkbox"
      halfWidth: false
      defaultValue: ""

    - note: success
      parentClass: "hidden text-sm message success"
      content: "We have received your message. Our team will contact you shortly."

    - note: deprecated
      parentClass: "hidden text-sm message error"
      content: "An error occurred. Please email us at [support@voicetophone.com](mailto:support@voicetophone.com)."
---
