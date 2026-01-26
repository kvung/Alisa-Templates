# Alisa Medtech Email Templates

Standardised email templates for Alisa Medtech AB.

## Templates

| Template | File | Description |
|----------|------|-------------|
| Order Confirmation | `templates/order-confirmation.html` | Sent after a successful order |
| Welcome Email | `templates/welcome-email.html` | Sent to new users upon registration |
| Email Verification | `templates/email-verification.html` | Sent to verify email address |
| Password Reset | `templates/password-reset.html` | Sent when user requests password reset |
| Contact Form Confirmation | `templates/contact-form-confirmation.html` | Sent when user submits contact form |

## Template Variables

### Order Confirmation
| Variable | Description |
|----------|-------------|
| `{{customer_name}}` | Customer's full name |
| `{{order_number}}` | Unique order identifier |
| `{{order_date}}` | Date of the order |
| `{{payment_method}}` | Payment method used |
| `{{order_items}}` | Array of ordered items (use `{{#each}}`) |
| `{{order_total}}` | Total order amount |
| `{{shipping_name}}` | Shipping recipient name |
| `{{shipping_address}}` | Shipping street address |
| `{{shipping_city}}` | Shipping city |
| `{{shipping_postal_code}}` | Shipping postal code |
| `{{shipping_country}}` | Shipping country |
| `{{order_tracking_url}}` | URL to track the order |

### Welcome Email
| Variable | Description |
|----------|-------------|
| `{{activation_url}}` | Account activation link |

### Email Verification
| Variable | Description |
|----------|-------------|
| `{{customer_name}}` | Customer's full name |
| `{{verification_url}}` | Email verification link |
| `{{expiration_hours}}` | Hours until link expires |

### Password Reset
| Variable | Description |
|----------|-------------|
| `{{customer_name}}` | Customer's full name |
| `{{reset_url}}` | Password reset link |
| `{{expiration_hours}}` | Hours until link expires |

### Contact Form Confirmation
| Variable | Description |
|----------|-------------|
| `{{customer_name}}` | Customer's full name |
| `{{reference_number}}` | Unique reference number for the inquiry |
| `{{message_subject}}` | Subject of the message |
| `{{message_category}}` | Category of the inquiry |
| `{{submission_date}}` | Date and time of submission |
| `{{message_content}}` | The submitted message content |
| `{{response_time}}` | Expected response time in business days |

## Branding

- **Company:** Alisa Medtech AB
- **Logo:** Text-based "ALISA" with letter-spacing
- **Primary Color:** `#6c9b9a` (muted teal)
- **Text Colors:** `#1a1a1a` (headings), `#4a4a4a` (body), `#888888` (secondary)
- **Background:** `#f0f0f0` (page), `#ffffff` (card), `#f7f7f7` (footer/boxes)
- **Website:** https://www.alisamed.se
- **Support Email:** support@alisamed.com
- **Contact Email:** kontakt@alisamed.com

## Usage

These templates use inline CSS for maximum email client compatibility. They are designed to be responsive and work across all major email clients including:

- Gmail
- Outlook (Desktop & Web)
- Apple Mail
- Yahoo Mail
- Mobile email clients

### Integration

Replace the `{{variable}}` placeholders with your templating engine's syntax (e.g., Handlebars, Jinja2, EJS, etc.).

## License

Copyright 2026 Alisa Medtech AB. All rights reserved.
