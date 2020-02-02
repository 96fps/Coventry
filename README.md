# Coventry
Self-hosted system for processing voice commands


# Major Components

## HotMic
- detects hotword and streams audio to be processed

### UI 
- Mic/command status information
- intermediate transcript
- display command as interpretted
- display/speak response

## DS transcript
- Receives streaming audio
- returns wip & final transcript

## command parser
- loads command lists
- Receives wip & complete transcript
- if TS is within threshold of command, trigger action and send response
- actions can load new command lists, send commands

## remote command exec
- receives commands that need to be run remotely and returns results/errocs
