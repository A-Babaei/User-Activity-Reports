# User-Activity-Reports WordPress Plugin

A comprehensive WordPress plugin designed for membership and educational websites to protect premium content and gain deep insights into user engagement through detailed activity tracking.

**Current Version:** 1.0.0  
**Requires at least:** WordPress 5.0  
**Tested up to:** WordPress 6.5  
**Stable tag:** 1.0.0  
**License:** GPLv2 or later  
**License URI:** https://www.gnu.org/licenses/gpl-2.0.html  
**Contributors:** Jules + Grok + DeepSeak  

## Features

### 1. Protected Content
- Restricts access to premium content (pages, posts, custom post types) to logged-in users with appropriate membership levels or course enrollments.
- Seamless integration with common membership and LMS systems (extendable via hooks).

### 2. User Activity Reports (Primary Feature)
- Accurately tracks time spent by logged-in users on individual pages and posts using lightweight client-side JavaScript with heartbeat and visibility detection.
- Detailed reports available in the WordPress admin:
  - **Per User Report** – View activity for a specific user over a selected date range (total visits, total time, average time per visit).
  - **Per Page/Course Report** – Identify most popular content, with optional grouping by course/category and filters for date range and user roles.
  - **Overall Stats** – High-level insights including Top 10 most viewed pages/courses and a list of inactive users (configurable inactivity threshold: 30/60/90 days).
- CSV export for both Per User and Per Page/Course reports.
- Custom database table with efficient indexing for fast queries even on large sites.

### 3. Settings & Privacy Controls
- Enable/disable activity tracking globally.
- Exclude specific user roles or individual post IDs from tracking.
- Configurable data retention period (e.g., automatically delete logs older than 6/12/24 months).
- Automatic log pruning via WP-Cron.
- Tracks only logged-in users – respects visitor privacy.

## Installation

1. Download the plugin ZIP file.
2. In your WordPress admin dashboard, go to **Plugins > Add New > Upload Plugin**.
3. Upload the ZIP file and click **Install Now**.
4. After installation, click **Activate**.

Alternatively (manual):
1. Extract the `protected-content` folder.
2. Upload it to the `/wp-content/plugins/` directory of your WordPress installation.
3. Activate the plugin through the **Plugins** menu in WordPress.

## Usage

### Accessing User Activity Reports
1. In the WordPress admin, navigate to **Protected Content > User Activity Reports**.
2. Use the tabs to switch between:
   - **Per User Report**
   - **Per Page/Course Report**
   - **Overall Stats**
3. Apply filters (date range, user role, etc.) and export data as needed.

### Configuring Settings
1. Go to **Protected Content > Settings**.
2. Adjust the following options:
   - Enable/Disable User Activity Tracking
   - Exclude specific user roles
   - Exclude specific post/page IDs
   - Set data retention period for automatic cleanup

## Privacy & Performance
- No tracking of non-logged-in visitors.
- Lightweight JavaScript with proper nonces and security checks.
- Minimal performance impact – optimized queries and efficient storage.
- GDPR-friendly design with configurable data retention.

## Changelog

### 1.0.0 – December 2025
- Initial release with full User Activity Reports feature.
- Per-user, per-page/course, and overall statistics dashboards.
- CSV export functionality.
- Comprehensive settings page with tracking controls and data retention.
- Automatic log pruning via WP-Cron.
- Secure, performant, and privacy-conscious implementation.

## Support & Contributions
This plugin is actively maintained. For bug reports, feature requests, or contributions, please open an issue or pull request on the GitHub repository.

Thank you for using Protected Content!
