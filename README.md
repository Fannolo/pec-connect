# PEC Connect plugin bundle

PEC Connect connects selected Aruba PEC mailboxes to AI assistants through the hosted MCP endpoint at https://pec.bite.technology/mcp. Publisher: Alessandro Fan. Support: alessandrofan94@gmail.com. Planned launch: Italy, free access.

This repository contains only the public plugin instructions, connection configuration and artwork. The hosted backend, credentials and mailbox data are not included. The plugin bundle is licensed under MIT; the separate hosted service is not part of that license grant.

## Publication status

This is a preparation version, not an approved ChatGPT or Claude directory listing. Public policy pages, reviewer access and the recorded demo remain incomplete. ChatGPT mailbox reading was reported working by the owner on 18 October 2026. Hosted Claude end-to-end verification and real SMTP delivery remain pending. Do not rely on the current hosted service as a verified public release.

## Claude directory source

Submit the plugin at `plugins/pec-connect` and separately submit the hosted MCP connector. Connect GitHub in the Claude publisher account before submitting. No marketplace review or approval has occurred yet.

The plugin can be discovered through this repository as a custom marketplace. Claude Code can load the bundle, but its loopback OAuth authentication is not supported by this service version. Hosted Claude chat and Cowork are the intended first surfaces.

## Version 0.3.0

The hosted service now supports immutable outgoing email drafts and personal browser confirmation for every send. Ask the assistant to prepare an email, open the review link, check all recipients, text and attachments, then personally confirm. Draft creation never sends. The updated private database and hourly cleanup are deployed. Local tests passed; real provider transmission remains to be verified. This is not marketplace review or publication.

## Version 0.3.1

Received attachments can now be downloaded using short-lived, account-protected browser links. Ask for a file download, open the returned PEC Connect link and sign in with the same account. Links expire within ten minutes and require the original mailbox grant. This release also fixes larger attachments on the outgoing review page. Local tests include exact 5 MiB received-file downloads and 2 MiB draft attachments. Real provider downloads and host tool discovery remain to be verified.
