# Security Policy

## Production Usage Requirements

Before deploying OptiMin in a production environment (public server, shared infrastructure, hosted platform), you **must use a clean and verified installation**.

A "clean installation" means:

- A freshly downloaded Minecraft server/client
- A freshly installed Fabric Loader
- Only the officially listed OptiMin mods
- No leftover configuration files from previous modpacks
- No unknown or unverified third-party modifications

Failure to start from a clean environment may result in:

- Leakage of sensitive Minecraft data
- Exposure of server IP addresses
- Exposure of authentication/session tokens
- Compromised configuration files
- Accidental logging of player-related information

## Sensitive Minecraft Data

The following data should always be treated as sensitive:

- Server IP addresses
- Player UUIDs
- Session tokens
- Authentication data
- Server configuration files
- Voice chat keys and networking configuration
- Essential session data
- Local world backups containing player information

Never publish these publicly.
Never commit them to GitHub.
Never share them in issue reports.

## Secure Deployment Checklist

Before going live:

- Verify all mods are official releases
- Remove debug logs
- Delete old crash reports
- Clear `/logs` and `/crash-reports` folders
- Regenerate voice chat keys if previously used
- Review `server.properties`
- Check file permissions on hosted machines

## Reporting a Vulnerability

If you discover a security issue related to this modpack:

- Do NOT open a public GitHub issue
- Contact the maintainer privately
- Provide clear reproduction steps
- Include only necessary logs (with sensitive data removed)

## Disclaimer

OptiMin is a performance-focused modpack.  
Security of your environment ultimately depends on your hosting setup, server configuration, and operational practices.

Always treat production environments as sensitive infrastructure.
