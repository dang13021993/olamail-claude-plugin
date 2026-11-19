# OlaMail for Claude — directory source package

This public-facing package connects Claude to the official OlaMail business email MCP hosted by OlaCheap (MIA Co., Ltd.). It contains only a plugin manifest, a remote MCP reference, and an email-safety Skill. No mailbox messages, login credentials, proprietary backend source code, customer data, local scripts, npm dependencies or lockfiles are included.

The MCP server is https://olacheap.com/api/mcp/mail. After a Claude user signs in by OAuth, only selected business mailboxes are accessible. Listing, searching and reading can be granted separately from sending. Creating a draft never sends. Sending requires explicit user approval and server permissions; new recipients may require account-owner approval. There is no bulk marketing tool.

This package is not a replacement for testing remote MCP authentication. Before public submission, verify Claude OAuth discovery, client registration, mailbox selection, `list_mailboxes`, `list_emails`, `read_email`, `create_draft`, and properly authorized sending, using synthetic test mailboxes only. Review privacy and permissions before each test.

Company: MIA Co., Ltd.  Website: https://olacheap.com/hosting/email  Support: https://olacheap.com/support
