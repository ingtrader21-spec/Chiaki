# NABEEL Chiaki integration

The system package `/usr/bin/chiaki` is the governed local Remote Play client. `docs/scripts/nabeel-chiaki-launch.sh` provides a credential-free status/launch boundary.

Rules:
- pairing and account credentials remain in the user's local Chiaki configuration and are never copied into Git;
- launch is local-only and does not enable streaming/publishing;
- status readback reports the executable/config location without printing secrets;
- the final PAS-261 gate still requires an authorized PlayStation to pair, reconnect, and prove video/audio.

```bash
docs/scripts/nabeel-chiaki-launch.sh status
docs/scripts/nabeel-chiaki-launch.sh launch
```
