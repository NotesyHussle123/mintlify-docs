# Documentation project instructions

## About this project

- This is the customer help site for Companion (trading as Message Companion), a shared WhatsApp inbox for small businesses, by DIGICORE IT LTD
- Built on [Mintlify](https://mintlify.com). Pages are MDX files with YAML frontmatter; configuration and navigation live in `docs.json`
- It replaces the FAQ list on the app's Help page (`apps/web/src/lib/data/help.ts` in the Companion repo)
- The source of truth for every statement is the Companion app's code. Do not describe anything the app does not do
- Readers are business owners and their staff, not developers. Most are not technical

## Terminology

- The product is "Companion" in running text. "Message Companion" only for the App Store listing name
- "workspace" for a business's account; "conversation" or "chat" for a thread; "customer" for the person writing in; "contact" for a record in Contacts
- Roles are owner, admin, manager and rep (lower case in running text)
- "website chat" for the widget; "broadcast" for a bulk send; "template" for a Meta-approved message; "form" for a template with a form button; "workflow" for an automation; "integration" for a connected system
- "phone app" for the iPhone app. There is no Android app
- "Meta" for the company that reviews templates and charges message fees; "WhatsApp Business app" for the free phone app from WhatsApp
- Name screens, menus and buttons exactly as the app labels them

## Style preferences

- British English: organise, colour, centre
- Active voice and second person ("you")
- Short sentences, one idea each. Plain words. No jargon, no marketing language
- Sentence case for headings
- Bold for UI elements: go to **Settings**, choose **Invite user**
- Say who can do it near the top of a page when a role is required, in a `<Note>`: "Owners and admins only."
- Use `<Steps>` for procedures, `<AccordionGroup>` for question-and-answer lists, `<Note>`, `<Tip>` and `<Warning>` sparingly, tables for comparisons
- Every page has `title` and `description` frontmatter. Do not repeat the title as an H1
- Link to related pages with root-relative paths without the extension: `/conversations/replying`
- No screenshots yet. Do not reference images that do not exist

## Content boundaries

- Do not quote Meta's message prices: Meta sets them by country and changes them. Describe what is charged, not how much
- Companion's own plan prices and limits come from `packages/shared-types/src/plans.ts`. Keep `billing/plans.mdx` in step with it
- Do not document the internal admin area, the design-system page, demo mode, environment variables or anything about how Companion is built
- Do not document integrations that are not available to customers yet
- Support address: support@msgcompanion.com. Status page: https://status.msgcompanion.com
