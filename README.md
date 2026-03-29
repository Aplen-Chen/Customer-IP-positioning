# Customer IP Positioning Reports

This repository collects a series of static HTML reports that describe the IP (ideal persona) positioning for different customers. Each report is written in Traditional Chinese and combines narrative analysis with charts styled via embedded CSS. The files are named after the respective customer personas (for example, `Catherine1.html`, `Chris1.html`, and so on).

## Getting started

To view a report, open the corresponding HTML file directly in a modern web browser. No additional build tools or dependencies are required because every page is fully self-contained.

## Repository structure

- `*.html`: Persona-specific IP positioning reports. Most personas have multiple revisions that are differentiated with numerical suffixes in their filenames.

## Contributing

Updates can be made by editing the relevant HTML file and opening it in a browser to verify the layout. When contributing, please try to keep the existing visual style and typography consistent across the different persona reports.

## Troubleshooting

If you see terminal output similar to `stream error: exceeded retry limit, last status: 401 Unauthorized`, it usually means the request that generated the report is missing valid credentials. You can resolve this by:

- Confirming that the API key or session token used by your tool is still active and has not expired or been revoked.
- Re-authenticating (for example, by running the CLI login command again) so that a fresh credential is stored in your environment.
- Verifying any environment variables that store credentials are correctly exported in the terminal session where you run the command.

Once valid credentials are supplied, the command should complete without the repeated 401 Unauthorized retries.
