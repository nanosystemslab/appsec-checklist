# Risk Classification

Risk level: Low / Medium / High

Low-risk indicators:
- Local-only or outbound-only data display.
- No remote commands.
- No personal/sensitive data.
- No public internet exposure.

Medium-risk indicators:
- Cloud logging.
- Web dashboard or API.
- MQTT/HTTP/WebSocket connectivity.
- Remote configuration.
- Public repository.

High-risk indicators:
- Remote actuation or safety impact.
- Human-subject, image/audio, location, biometric, health, student, or other identifiable data.
- Public endpoint or inbound service.
- OTA updates.
- Credentials stored on device.
- Field deployment outside lab.

Decision rationale:
Required add-ons:
Faculty/PI sign-off:
