# Frequently Asked Questions

## General Questions

### What is BirdTalk's relationship with eBird?
BirdTalk is a voice-controlled interface for creating and submitting eBird checklists. It uses your eBird account credentials to:
- Access eBird hotspots near your location
- Submit completed checklists to your eBird account
- Validate bird species for your region

### Do I need an internet connection?
- Required for:
  - Initial installation
  - Downloading regional bird data
  - Submitting checklists
- Not required for:
  - Creating checklists in the field
  - Recording observations
  - GPS tracking

### How does BirdTalk handle GPS tracking?
- Automatically tracks your route during active checklists
- Records location for each observation
- Can stop/resume tracking within the same checklist
- Shows total distance traveled

## Voice Recognition

### Why does BirdTalk sometimes take longer to respond?
- BirdTalk waits for silence to know you've finished speaking
- In quiet conditions: responds within 1 second
- With background noise (wind, traffic): may take up to 3 seconds
- Solution: Wait for a quiet moment or speak more clearly

### How can I improve voice recognition?
1. Speak clearly and consistently
2. If a command isn't recognized, repeat the exact same phrase
3. In noisy conditions:
   - Speak slightly louder
   - Position microphone closer
   - Wait for quieter moments

### What if BirdTalk doesn't recognize a bird name?
- Try using a unique part of the name
- Repeat the exact same phrase
- Check the [command reference](commands/reference.md) for shorthand examples
- Once a species is in your checklist, its name gets priority for recognition

## Using with Other Apps

### Can I use Merlin Sound ID simultaneously with BirdTalk?
Yes, but with some considerations:
1. Start BirdTalk before Merlin for optimal audio control
2. Both apps share the same microphone input
3. Headset microphone may reduce Merlin's effectiveness
4. Use "Switch" command to change to phone microphone if needed

### Will I hear notifications while using BirdTalk?
- iPhone automatically silences notifications when Merlin Sound ID is active
- Solution: Use an Apple Watch to receive notifications
- BirdTalk itself doesn't affect notifications

## Hardware and Audio

### Which Bluetooth headset should I use?
We recommend the OpenComm2 Bone Conduction Headset because:
- Leaves ears unobstructed for birding
- Has a boom microphone for better voice recognition
- Provides good noise isolation
- Uses bone conduction technology

### How do I manage multiple Bluetooth devices?
- iPhone can handle two audio devices:
  - Internal mic/speaker
  - One Bluetooth device
- Most recently connected device takes control
- Use "Switch" command to toggle between devices
- Power cycle headset or use Settings/Bluetooth to change control

## Checklists and Data

### How do I manage multiple checklists?
- You can have multiple incomplete checklists
- Use "Stop checklist" to pause current checklist
- Start new checklist when location changes
- Submit checklists when you have internet connection

### Can I edit checklists after creation?
Yes:
- Use "Insert checklist" to split observations into separate lists
- "Scratch" removes checklist headers to combine lists
- Edit comments and counts at any time
- Review and mark entries before submission

### How do I prepare for birding in a new location?
1. Start a dummy checklist at your hotel/base
2. This downloads the regional bird database
3. Once downloaded, you can bird offline
4. Remember to submit checklists when back online

## Privacy and Data

### What information does BirdTalk collect?
- Logs voice recognition attempts for improvement
- Stores phonetic format of commands (not readable text)
- Uses GPS data for tracking and hotspot detection
- All data is used solely for app functionality and debugging

### Can I opt out of data collection?
- When muted or checklist stopped, no logging occurs
- Use "Shut down" to completely stop all app functions
- Contact developer for specific privacy concerns

## Troubleshooting

### What if my headset stops working?
1. Try power cycling the headset
2. Use "Switch" command to reset audio routing
3. Check Bluetooth connections in iPhone Settings
4. Ensure headset is most recently connected device

### Why can't I submit my checklist?
Common reasons:
- No internet connection
- Marked (red) entries need review
- Not selected on checklist header
- Solution: Unmark entries, select header, ensure connection

### What if I lose GPS signal?
- BirdTalk continues recording observations
- Location data may be less accurate
- Consider adding location notes in memos
- GPS track will resume when signal returns
