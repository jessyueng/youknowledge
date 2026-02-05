# YouBase - Built-in Cloud Backend

YouBase is YouWare's integrated cloud backend infrastructure, providing enterprise-grade capabilities without external dependencies.

## Overview

YouBase transforms YouWare from a frontend builder into a **full-stack development platform**. It includes:

- **Database** - Structured data storage with Time Travel
- **Users & Authentication** - Email, OAuth, and temporary accounts
- **Storage** - Cloud file uploads and downloads
- **Secrets** - Secure API key management

**Availability:** Pro and Ultra plans only

**Key Benefits:**
- Scales on demand
- Enterprise-grade security
- High performance globally
- Zero configuration setup
- No external dependencies

---

## Database Module

Persistent, structured data storage with powerful management features.

### Capabilities

| Feature | Description |
|---------|-------------|
| Create Tables | Natural language prompts to create database tables |
| Store Data | Persistent storage across sessions |
| Query Data | Retrieve and filter data without SQL |
| Export | Download data as files (Pro/Ultra) |
| Time Travel | Restore to previous database states |

### Time Travel (Database History)

Restore your database to any previous state.

| Plan | Retention | Restore |
|------|-----------|---------|
| Pro | 14-day bookmarks | Limited |
| Ultra | Full history | Full restore |

**Bookmark Types:**
- **Automatic**: Created on significant changes
- **Manual**: Create your own restore points

### Use Cases

- Form submissions and contact data
- Lists and dashboards
- User-specific data storage
- AI memory and usage history
- Internal tools and SaaS prototypes
- E-commerce product catalogs

---

## Users & Authentication Module

Built-in user management with multiple authentication methods.

### Authentication Methods

| Method | Description |
|--------|-------------|
| **Email Login** | Traditional email/password with verification |
| **Google OAuth** | One-click Google sign-in |
| **Temporary Accounts** | Anonymous/guest access without registration |

### User Dashboard Features

- User list management
- Add/delete/block/unblock users
- User analytics and activity
- Session management

### Configuration Options

- Email verification toggle
- Password reset verification
- Logout all devices on password change
- Custom authentication flows

### Use Cases

- Member-only pages and content
- User-specific data storage
- Personalized user experiences
- Access control and permissions
- SaaS prototypes with login

---

## Storage Module

Cloud file storage for user uploads and persistent file management.

### Capabilities

| Feature | Description |
|---------|-------------|
| User Uploads | Accept files from users (images, documents) |
| Download | Individual files or ZIP bundles |
| Multi-file | Bundle multiple files for download |
| Persistent | Files available across sessions |

### Current Limitations

- No in-browser file preview
- No file deletion (contact support)
- Agents cannot directly modify storage

### Use Cases

- User profile pictures
- Document attachments
- Generated files and AI outputs
- Media files linked to database records
- Multi-file downloads for users

---

## Secrets Module

Secure storage for API keys, tokens, and sensitive configuration.

### Features

| Feature | Description |
|---------|-------------|
| Encrypted Storage | Enterprise-grade encryption |
| Server-Side Only | Never exposed to frontend code |
| 64 Secrets Max | Per project limit |
| Hidden After Creation | Cannot view value after saving |

### Management

- Create new secrets with key-value pairs
- Edit existing secret values
- Delete secrets when no longer needed
- Access from server functions only

### Security

- Secrets are **never** exposed to:
  - Frontend JavaScript
  - Browser developer tools
  - Public API responses
- Only accessible via server-side functions

### Use Cases

- Third-party API keys (Stripe, SendGrid, etc.)
- AI model credentials (OpenAI, Anthropic)
- External service tokens
- Environment-specific configuration
- Internal sensitive settings

---

## Project Usage

Monitor your YouBase resource usage.

### Metrics Tracked

- Database storage used
- Number of users registered
- Storage space consumed
- API call counts

### Limits (During Beta)

- **Database**: Unlimited storage
- **Storage**: Unlimited files
- **Users**: Unlimited registrations

*Beta period pricing may change*

---

## Adding YouBase to Projects

### Steps

1. Open your project settings
2. Navigate to "Backend" or "YouBase" section
3. Enable YouBase for the project
4. Configure modules as needed

### Pause & Restart

- Pause YouBase to reduce resource usage
- Restart when needed
- Data preserved during pause

---

## Best Practices

### Database

- Use descriptive table and field names
- Create indices for frequently queried fields
- Export data regularly for backups
- Use Time Travel bookmarks before major changes

### Authentication

- Enable email verification for security
- Use Google OAuth for easier onboarding
- Consider temporary accounts for demos

### Storage

- Organize uploads with consistent naming
- Link files to database records
- Use ZIP downloads for multiple files

### Secrets

- Never hardcode API keys in frontend code
- Rotate secrets periodically
- Use descriptive secret names
- Delete unused secrets
