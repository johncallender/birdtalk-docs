# Frequently Asked Questions

## General Questions

### What are the advantages of BirdTalk?

- Makes birding more fun by being "in the moment", compared to intermittently tapping into the eBird app.
- Maximizes time looking at birds instead of the phone, so that you can see and record more birds, more accurately, with less fuss.

### What are the limitations of BirdTalk compared to the eBird app?

- Currently works only within the United States.
- Has no way to upload the following info:
    - Locations that are not hotspots
    - Bird sex, age, and breeding code info
    - The track you walked while birding
- Record such extra info as comments using the `Memo` command, then review and edit the checklist online after upload.

### What is BirdTalk's relationship with eBird?

BirdTalk acts as a replacement for the eBird app.  However, we would love to see BirdTalk's features built into the eBird app itself, so we are talking to eBird about how that could happen.

### Do I need an internet connection?

- Internet is not needed in the field.
- Records bird and location info completely offline.
- Internet needed for initial install, and to upload checklists at the end of a day of birding.

## Using BirdTalk

### Should I edit before uploading a checklist?

Yes!

- Review all entries in your checklist to make sure no undesired species crept in during your session.
- Fix any errors by tapping the bad item and using the editing commands:
    - `No` or `Make that`
    - `Scratch`
    - `Memo`
    - `Insert`
- Review marked (red) entries, and say `Unmark` on each once you've added an appropriate memo.

### How should I handle a multi-hotspot walk?

- The standard approach is to say `Start checklist` as you enter each new checklist area, which automatically stops the prior checklist.
- Alternatively you can just `Start checklist` once at the start and record all birds as you go.
- Then, later, use `Insert checklist` at appropriate points to split it into several checklists.
- Use `Scratch` to removes checklist headers if you started a new checklist but decide to combine those entries into the previous one.

### How can I make a checklist at a personal location rather than a hotspot?

- BirdTalk doesn't allow making a checklist for a Personal Location.
- The work-around is to start a checklist using the neareset hotspot instead.
- Then, after completing and uploading the checklist, edit the location for that checklist on your web account at eBird.

### How does BirdTalk handle distance where I retrace part of my path?

- BirdTalk automatically figures distance according to eBird's checklist requirements.
- This means if you retrace part of your path, that is not added to the recorded distance.
- For instance, on a trail that is 3 miles out and 3 miles back, BirdTalk will note the total checklist distance as 3 miles.
- It is clever about this so if there is a 1 mile loop excursion somewhere along the 3-out-and-back path, it will give a total of 4 miles for that total path, even though you walked 7 miles.

## Voice Recognition

## What if BirdTalk is not responding to my speech?

- Say `Time` to check that the microphone is receiving the audio
- Make sure the volume on your phone is turned up enough to hear BirdTalk talking back to you
- There may be an up to 30 second delay in response the first time you turn on BirdTalk, as it loads its database from the internet.
- Make sure the Start/Stop button at upper left says "Stop" which means it is listening.  If it says "Start", tap it to tell BirdTalk to listen.
- Power off the Bluetooth headset and make sure the phone internal mic can hear you by saying `Time`.  Then power on the Bluetooth headset and try again.
- This works because the most recently connected device takes control
- Make sure there is no other app running that is controlling the mic, such as Merlin or a phone call
- If you have never installed Siri, do so.  This activates speech recognition.
- As a last resort, <a href="https://support.apple.com/guide/iphone/quit-and-reopen-an-app-iph83bfec492/ios">close the BirdTalk app</a>, re-open it, and say `Resume` to pick up where you left off.

### Why does BirdTalk sometimes take longer to respond?

- BirdTalk waits for silence to know you've finished speaking
- In quiet conditions: responds within 1 second
- With background noise (wind, traffic): may take up to 4 seconds
- Wait a few seconds after speaking in a noisy environment, to make sure BirdTalk detects the end of the command.
- BirdTalk responds faster when using a noise-cancelling microphone.

### Which Bluetooth headset should I use?

See our [recommended](installation/requirements-and-setup.md/#requirements) Bluetooth headset.

### How can BirdTalk understand me better in noisy environments?

- Accuracy is far better when using the above Bluetooth headset due to its noise-cancelling boom microphone
- Wait for quiet moments (such as between surf crashes at the shore)
- Cup your hand around the microphone to reflect your voice more loudly into it
- Check that the mic remains positioned close to your mouth
- Leave 3-4 seconds after speaking a command
- Say `break` after the command to signal the end when other nearby speech may be picked up by the mic and confuse BirdTalk.  For example say `robin break` or even `break robin break`.  This is only somewhat effective but can help in some situations.

### How can I speak bird entries most effectively?

- Whispering, or whispering + cupping your hand to focus your voice into the mic, can be effective when you want to avoid disturbing birds
- You can use single words or sub-phrases from species names, when they are unique in your area, in place of the complete name.  For instance `rump` or `yellow rump` for Yellow-rumped Warbler
- Or use the full name for species where parts don't work, such as for `Black Scoter`
- Experiment with different forms to find what works best for each problematic species
- Once a species is in your checklist, it gets recognition priority, and shorthand for it will work that wouldn't before
- Please contact us about particularly troublesome species.  We can improve their recognition accuracy.

### How do I enter big numbers of birds, like hundreds or thousands?

- You must say "hundred" or "thousand" when giving large numbers.
- Say `One hundred fifty starlings`, not "one fifty"
- Say `One thousand two hundred starlings`, not "twelve hundred".

The iPhone can handle only two audio devices at a time:  the internal mic&speaker, and one external Bluetooth mic&speaker.  Even if you have several Bluetooth devices (such as your JBL speaker and your headset) connected, the iPhone only recognizes the one that was most recently connected to the phone, i.e. was most recently powered up.

Whenever a Bluetooth device powers up and connects to the iPhone, that Bluetooth device grabs control and becomes the only accessible Bluetooth device.

So for example if you are talking to BirdTalk via the headset and then you turn on your JBL, the JBL will connect to the iPhone and take control.  Suddenly you’ll have to talk to BirdTalk through the JBL and it will talk back through it.

If you get in a situation where you’d like to switch audio to a different Bluetooth device, say the headset, you can do so by either turning the headset power off and then on (so that it grabs audio control); or use the phone’s Settings/Bluetooth page to disconnect other Bluetooth audio devices so control switches back to the headset, or use the Settings/Bluetooth page to disconnect and reconnect the headset, which makes it grab audio control.

One tricky case is where you want to switch audio back to your headset when you’ve set the external speaker down out of reach.  Unfortunately since you’re playing back sounds through that speaker, it also means that the microphone that BirdTalk is listening on is also at that speaker.  If it’s several feet away from you it will be too inconvenient to shout your BirdTalk commands at it!

So to switch from playback back to your headset for giving BirdTalk commands, you need to switch audio control away from the speaker.  Do this using the same steps mentioned above: easiest is probably to power the headset off and then on so it grabs control, but you could instead use Settings/Bluetooth on the iPhone to disconnect the external playback speaker.

## Using with Other Apps/Devices

### Using External Speakers

- If using a Bluetooth headset with BirdTalk:
    - Turn on the headset and control switches to it.
    - Say `Switch` to tell BirdTalk to switch from the headset mic/speaker to the internal iPhone mic/speaker.
    - Say `Switch` again to tell BirdTalk to switch from the internal iPhone mic/speaker back to the headset iPhone mic/speaker.

- Handling multiple Bluetooth devices:
    - *iPhone issue*: If you have two Bluetooth devices (say a headset and an external speaker), only the one most recently turned is known to the iPhone.
    - So `Switch` goes between the internal mic/speaker and the most recently powered on Bluetooth device, ignoring any other Bluetooth devices.
    - Turning on a Bluetooth device makes it take control as the "active" device.
    - When you power up your external speaker, it gets control, and BirdTalk will talk and listen to you through it.
    - To get BirdTalk back to the headset, turn the headset power off and then back on.
    - Or power off the speaker and control returns to the last Bluetooth device, i.e. the headset.

### Phone and text notifications

- When a phone call comes in, BirdTalk stops listening until the phone call is complete
- If BirdTalk stop responding after a call or notification, tap "Stop" at upper left then tap "Start" to resume listening
- Usually you must then say `Resume` to pick up with the last-active checklist

### Note About Merlin Sound ID

Due to a recent Merlin or iOS update, Merlin Sound ID is no longer compatible with BirdTalk. The apps cannot run simultaneously.  Hopefully they'll soon fix Merlin to again allow other apps to share the microphone with it.


## Privacy and Data

### What information does BirdTalk collect?

- Logs voice recognition attempts for improvement
- Stores phonetic format of commands (not readable text)
- Uses GPS data for hotspot detection and location recording
- All data is used solely for app functionality and debugging

