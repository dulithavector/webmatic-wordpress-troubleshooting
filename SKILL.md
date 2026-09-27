---
name: webmatic-wordpress-troubleshooting
description: Diagnose and resolve WordPress technical issues for Webmatic using an evidence-based, safe, and systematic troubleshooting workflow.
metadata:
  short-description: Safe WordPress troubleshooting for Webmatic
---

# Webmatic WordPress Troubleshooting

Use this skill when Webmatic needs to diagnose, troubleshoot, fix, or plan a fix for a WordPress website or WordPress-related technical issue.

The objective is to identify the root cause, choose the safest practical solution, minimize downtime and data loss, verify the fix, and document the result.

Never guess when evidence can be collected.

## 1. Identify the Problem

First establish:

- Website URL
- WordPress environment
- Exact symptom
- When the issue started
- Whether it affects all users or only some users
- Whether it affects desktop, mobile, or both
- Whether the issue is frontend, backend, or both
- Recent changes
- Recent plugin/theme/core updates
- Hosting/server changes
- DNS/domain/email changes
- Whether the issue can be reproduced

Separate:

- Confirmed facts
- User observations
- Suspected causes
- Unknown information

Do not present a suspected cause as a confirmed root cause.

## 2. Classify the Issue

Classify the problem into one or more categories:

- Website unavailable
- WordPress dashboard issue
- 404 / routing issue
- Plugin conflict
- Theme issue
- Elementor issue
- WPBakery issue
- WooCommerce issue
- PHP error
- JavaScript error
- CSS/layout issue
- Database issue
- Media/image issue
- Form/email issue
- SMTP issue
- SSL/HTTPS issue
- DNS/domain issue
- Hosting/server issue
- Performance issue
- Cache issue
- Security/malware issue
- User permissions issue
- Migration/restoration issue
- Other

## 3. Collect Evidence

Use available evidence before changing anything.

Relevant evidence may include:

- Visible error messages
- Browser console errors
- Network errors
- WordPress debug logs
- PHP/server logs
- Plugin logs
- WooCommerce logs
- Hosting error logs
- HTTP status codes
- WordPress health information
- Plugin/theme versions
- WordPress core version
- PHP version
- Database errors
- Recent change history
- Screenshots
- Reproduction steps

Record what was actually checked.

Never claim that a log, device, browser, server, database, or tool was checked when it was not actually available.

## 4. Root Cause Analysis

Use a systematic troubleshooting process:

1. Reproduce the issue.
2. Identify the affected component.
3. Determine when the issue began.
4. Compare recent changes.
5. Check relevant logs/errors.
6. Isolate the failing component.
7. Test the most likely cause safely.
8. Confirm the root cause.
9. Select the least risky effective fix.

Possible root causes include:

- Plugin conflict
- Theme conflict
- Outdated software
- PHP incompatibility
- JavaScript error
- CSS conflict
- Cache issue
- Database corruption
- Incorrect configuration
- File permission problem
- Server resource issue
- DNS configuration
- SSL configuration
- SMTP configuration
- Third-party integration failure
- Malware/security compromise
- Incorrect custom code

Do not randomly disable plugins, edit databases, modify DNS, or change production code without a reason.

## 5. Production Safety

Before making potentially destructive or high-risk changes:

- Create or confirm a recent backup.
- Identify a rollback method.
- Record the current configuration.
- Prefer staging when available.
- Make one meaningful change at a time.
- Test after each significant change.

High-risk actions include:

- Database modifications
- File deletion
- Plugin removal
- Theme replacement
- DNS changes
- Server configuration changes
- PHP version changes
- Security cleanup
- Search/replace operations
- Bulk content changes
- Migration operations

Never perform destructive actions blindly.

## 6. WordPress Core Troubleshooting

Check:

- WordPress version
- PHP version
- Active theme
- Active plugins
- Recent updates
- WordPress Site Health
- Permalinks
- REST API
- Cron
- Media permissions
- File permissions
- Database connectivity
- Memory limits
- Upload limits
- Caching

If WordPress core files appear corrupted, prefer a controlled core reinstall or restoration rather than manually replacing random files.

## 7. Plugin Conflict Troubleshooting

When a plugin conflict is suspected:

1. Identify recently changed plugins.
2. Check error logs.
3. Reproduce the issue.
4. Test safely.
5. Disable the minimum necessary component.
6. Test again.
7. Identify the conflicting plugin.
8. Check compatibility and updates.
9. Restore required plugins.
10. Recommend a permanent solution.

Do not leave required production plugins disabled without client approval or a documented reason.

## 8. Theme Troubleshooting

Check:

- Active theme
- Child theme
- Recent theme changes
- Custom CSS
- Custom PHP
- Theme JavaScript
- Template overrides
- WooCommerce template overrides
- Header/footer code
- Theme/plugin compatibility

Do not replace a production theme as a first troubleshooting step.

## 9. Elementor Troubleshooting

For Elementor-related issues, check:

- Elementor version
- Elementor Pro version where applicable
- WordPress version
- PHP version
- Plugin conflicts
- Elementor Safe Mode where available
- CSS regeneration
- Cache
- Responsive settings
- Custom CSS
- JavaScript errors
- Theme compatibility
- Memory limits

Common issues may include:

- Editor not loading
- Widgets not displaying
- Layout broken
- Mobile responsiveness problems
- Dynamic content failures
- CSS not updating
- Templates not loading

Do not assume Elementor is the cause without evidence.

## 10. WPBakery Troubleshooting

Check:

- WPBakery version
- Theme compatibility
- Shortcodes
- Backend/frontend editor
- Plugin conflicts
- Custom CSS/JS
- JavaScript errors
- Cache
- Theme templates

If shortcode output is broken, identify whether the issue comes from WPBakery, the theme, a plugin, or custom code.

## 11. WooCommerce Troubleshooting

Check:

- WooCommerce version
- WordPress version
- PHP version
- Theme compatibility
- Payment gateway
- Shipping configuration
- Cart
- Checkout
- Product configuration
- Product variations
- Emails
- Taxes
- Coupons
- Webhooks
- Scheduled actions
- WooCommerce logs

For checkout/payment problems, do not assume the gateway is the problem without testing the relevant flow.

Never perform real financial transactions unless explicitly authorized and safe test procedures are available.

## 12. Forms and Email Troubleshooting

For contact forms or WordPress email issues, check:

- Form configuration
- Recipient address
- From address
- Reply-to address
- SMTP configuration
- SMTP host
- SMTP port
- Encryption
- Authentication
- DNS records
- SPF
- DKIM
- DMARC
- Server mail restrictions
- SMTP connection errors
- Spam/junk folder
- WordPress mail logs where available

Distinguish between:

- Form submission failure
- WordPress email generation failure
- SMTP connection failure
- Email delivery failure
- Recipient-side filtering

Do not claim that email delivery is fixed until an appropriate test confirms it.

## 13. 404 and Routing Issues

For 404 problems, check:

- URL
- Permalinks
- Rewrite rules
- `.htaccess` where applicable
- Server configuration
- Page existence
- Redirects
- Plugin routing
- Custom post types
- Taxonomies
- WooCommerce endpoints
- Cache

Do not immediately edit `.htaccess` without understanding the existing configuration.

## 14. Images and Media Problems

Check:

- File existence
- File URL
- HTTP status
- File permissions
- Upload path
- WordPress Media Library
- Image optimization
- CDN
- Mixed content
- Lazy loading
- Hotlink protection
- Server errors
- Theme/plugin image handling

Distinguish between:

- Image missing
- Image exists but does not load
- Incorrect URL
- Permission issue
- Server response issue
- Frontend rendering issue

## 15. Performance Issues

For performance problems:

- Measure where possible.
- Identify actual bottlenecks.
- Check server response time.
- Check image sizes.
- Check caching.
- Check plugins.
- Check scripts/styles.
- Check database load where available.
- Check third-party resources.
- Check hosting resources.

Never claim a website is "slow" based only on subjective impression if measurement is required.

Do not recommend deleting plugins or changing hosting without evidence.

## 16. Security Issues

For visible security concerns:

- Identify observable evidence.
- Determine whether the issue is configuration, outdated software, suspicious code, or another risk.
- Recommend backup and containment where appropriate.
- Avoid destructive cleanup without evidence and recovery options.

Never claim a website is secure simply because no visible warning was found.

For suspected malware:

1. Preserve evidence.
2. Create/confirm backup.
3. Identify affected files/accounts.
4. Determine likely entry point where possible.
5. Contain the issue.
6. Clean or restore safely.
7. Update vulnerable software.
8. Reset affected credentials.
9. Verify the website.
10. Recommend monitoring and prevention.

Do not delete suspicious files blindly.

## 17. DNS, SSL, and Hosting Issues

When the issue involves hosting or DNS:

Check the relevant configuration before making changes.

Possible areas:

- A record
- AAAA record
- CNAME
- MX
- TXT
- Nameservers
- SSL certificate
- HTTPS redirects
- CDN
- Hosting account
- Server IP
- Web server configuration

DNS changes can affect websites and email. Confirm the intended configuration before changing production DNS.

## 18. Fix Strategy

For every recommended fix, explain:

- Problem
- Root cause or current evidence
- Recommended fix
- Why this fix
- Risk
- Backup/rollback requirement
- Implementation steps
- Verification steps

Prefer:

1. Lowest-risk effective fix
2. Reversible fix
3. Minimal production impact
4. Sustainable fix
5. Documented fix

## 19. Verification

After applying a fix, verify the original problem.

Check where applicable:

- Original error no longer occurs
- Website loads
- Admin works
- Mobile works
- Forms work
- Emails work
- Cart works
- Checkout works
- Links work
- Console errors are resolved
- Relevant integrations work
- No new major errors were introduced

Do not mark an issue as resolved without appropriate verification.

## 20. Client Communication

When explaining a technical issue to a client:

Use this structure:

### Problem
What was happening.

### Cause
What caused it, if confirmed.

### Fix
What was changed.

### Verification
How the fix was tested.

### Recommendation
Any useful prevention or maintenance recommendation.

Avoid unnecessary technical jargon when communicating directly with non-technical clients.

Never blame the client without evidence.

## 21. Output Format

For a troubleshooting task, use:

### Issue
Short description.

### Evidence
What was actually observed or tested.

### Likely / Confirmed Cause
Clearly distinguish confirmed cause from hypothesis.

### Risk
Potential impact.

### Recommended Solution
Safest practical solution.

### Implementation
Step-by-step actions.

### Verification
How to confirm the fix.

### Prevention
Useful future recommendation.

### Status
- Investigating
- Cause Identified
- Fix Planned
- Fix Applied
- Verified
- Blocked
- Escalation Required

## 22. Important Rules

- Never invent logs, errors, test results, versions, or configurations.
- Never claim to have accessed a server, hosting panel, database, DNS account, or admin panel unless access actually exists.
- Never make destructive production changes without an appropriate backup or rollback path.
- Never recommend random fixes.
- Never hide uncertainty.
- Separate facts from hypotheses.
- Protect client credentials and confidential information.
- Prefer evidence-based troubleshooting.
- Keep changes minimal and reversible.
- Verify fixes.
- Document important changes.
- Consider business impact and downtime.
- When required information is missing, ask for the minimum information needed.