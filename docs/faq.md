# Frequently Asked Questions

## General Questions

### Why would one want to use BirdTalk?

- BirdTalk makes birding more fun.  It enhances the feeing of freedom and joy from being one with nature, compared to incessantly tapping into the eBird app.
- BirdTalk maximizes time looking at birds instead of looking at the phone, so that you can see and record more birds, more accurately, with less fuss.

### What is BirdTalk's relationship with eBird?

We think BirdTalk's capabilities would be a perfect complement to the eBird app, so we are in talks with eBird to see if they're interested in incorporating it into the eBird app.


### What are the limitations of BirdTalk compared to the eBird app?

In most situations BirdTalk is the more convenient way to record bird observations, but it has limitations:

- BirdTalk currently works only within the United States and New Zealand.  By mid-2025 it will work anywhere, world-wide.
- BirdTalk tracks your GPS path while recording a checklist, but there's currently no way to upload that "path where I walked" info to eBird.  This isn't a critical problem, but we hope to add this capability in the future.
- BirdTalk can't record breeding code, age, and sex information in the field because there's no way for it to upload that info to eBird.  The workaround for now is to use the `memo` feature to record this info then edit the checklist in your eBird account after uploading.  We hope to improve this capability in the future.
- In extremely noisy environments, BirdTalk can't understand speech very well.  When that happens the best current alternative is to use the eBird app for manual data entry.  We plan to add a manual-entry option to BirdTalk for such situations.
- BirdTalk doesn't allow making checklists for Personal Locations, only for hotspots.  Search for "personal location" below for how to work around this limitation.

### Do I need an internet connection?

Required for:

- Initial installation and first-time setup
- Uploading checklists

Not required for:

- Creating checklists in the field
- Recording observations
- Location recording

## Using BirdTalk

### Should I edit before uploading a checklist?

Yes:

- Review all entries in your checklist to make sure no undesired species crept in during your session.
- Fix any errors by tapping the bad item and using the editing commands:
    - `No` or `Make that`
    - `Scratch`
    - `Memo`
    - `Insert`
- Review marked (red) entries, and say `Unmark` on each once you've added an appropriate memo.
- Ensure you've selected the checklist location header, by tapping it or saying `Choose checklist`

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
- As a last resort, <a href="https://support.apple.com/guide/iphone/quit-and-reopen-an-app-iph83bfec492/ios">close the BirdTalk app</a> and then open it again from the Desktop.

### Why does BirdTalk sometimes take longer to respond?

- BirdTalk waits for silence to know you've finished speaking
- In quiet conditions: responds within 1 second
- With background noise (wind, traffic): may take up to 4 seconds
- Wait a few seconds after speaking in a noisy environment, to make sure BirdTalk detects the end of the command.
- BirdTalk usually responds faster when using a noise-cancelling microphone.

### Which Bluetooth headset should I use?

See our [recommended](installation/requirements-and-setup.md/#requirements) Bluetooth headset.

### How can BirdTalk understand me better in noisy environments?

- Accuracy is far better when using the above noise-cancelling boom microphone
- Wait for quiet moments (such as when the surf abates at the shore)
- Cup your hand around the microphone to reflect your voice more loudly into it
- Check that the mic remains positioned close to your mouth
- Leave 3-4 seconds after speaking a command
- Say `break` after the command to signal the end when other nearby speech may be picked up by the mic and confuse BirdTalk.  For example say `robin break` or even `break robin break`.  This is only somewhat effective but can help in some situations.

### How can I speak bird entries most effectively?

- Whispering, or whispering + cupping your hand to focus your voice into the mic, can be effective when you want to avoid disturbing birds
- You can use single words or sub-phrases from species names, when they are unique in your area, in place of the complete name.  For instance `rump` or `yellow rump` for Yellow-rumped Warbler
- Or use the full name for species where parts don't work, such as for `Black Scoter`
- Experiment with different shorthands to find what works best for problematic species
- Once a species is in your checklist, it gets recognition priority, and shorthand for it will work that wouldn't before

### How do I enter hundreds or thousands of birds?

- You must say "hundred" or "thousand" when giving large numbers.
- Say `One hundred fifty starlings`, not "one fifty"
- Say `One thousand two hundred starlings`, not "twelve hundred".

## Using with Other Apps

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

