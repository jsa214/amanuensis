# The Amanuensis
- [Tutorial #1 - Getting Up and Running](https://steemit.com/utopian-io/@to-the-sun/getting-up-and-running-a-tutorial-for-the-open-source-project-the-amanuensis-automated-songwriting-and-recording)
- [Tutorial #2 - Setting Up Tracks' Recording Sources](https://steemit.com/utopian-io/@to-the-sun/setting-up-tracks-recording-sources-a-tutorial-for-the-open-source-project-the-amanuensis-automated-songwriting-and-recording)
- [Tutorial #3 - Setting Up Tracks' MIDI Sources](https://steemit.com/utopian-io/@to-the-sun/setting-up-tracks-midi-sources-a-tutorial-for-the-open-source-project-the-amanuensis-automated-songwriting-and-recording)

Currently The Amanuensis is in a version 1.x beta. **Playtesters wanted!**

## Version 2.0

At this point perhaps one use of an open-source effort might be in creating a brand-new version 2.0 from the ground up. One major upgrade would be to decouple The Amanuensis from its reliance on MIDI. Although more difficult to get working correctly, this would be more streamlined and straightforward from a user's perspective, as well as address certain idiosyncrasies such as what happens when MIDI notes have long attacks or when dealing with glissando in vocals or other instruments. This could be accomplished by reworking the algorithm that judges what parts of the music are best. Instead of relying entirely on analyzing rhythm, i.e. specific moments in time, a more comprehensive machine learning approach could be implemented.

I imagine a deep neural net focused on spectral analysis that on the lowest level is looking at a period of time equivalent to that of maybe a beat, determining where in that window an onset is likely to occur. This would be the layer that judges rhythm, by taking notice of any deviance in their positions. The next layer might look at windows the length of a measure and be able to identify repeated riffs and the like. Additional layers would find patterns on the scale of whole choruses and verses. In theory, deviations in pitch from an established scale could also be detected implicitly. A rating could then be derived based more heavily on the essentials like rhythm, but also taking into account the repetition of higher-level motifs.

At any given moment then, a percentage score could be calculated based on what the user is actually playing versus what the program expected would be most likely to hear. 100% would not necessarily be ideal; good music requires the establishment of patterns and then the breaking away from them. So perhaps a target percentage more like 50 or 75% similar to the expected could be used. At this point, it would be only a small step further to imagine an AI for you to jam right along with. The algorithm could actually generate the audio it expects to come next, rather than just judging based upon it. It would probably be ideal if the AI trained on each instrument it heard independently, so it could truly play alongside you with a different instrument than yours rather than the same one right on top of you, which would be jarring. This is also one of the issues of a player using the system by themselves: as soon as it starts looping, it's often playing the same thing (not quite) totally in sync with you. An AI would be something to brace against while you got going and you wouldn't even need to hear the audio in the track currently being captured until later.

It is also the eventual goal for this system to blend seamlessly into any situation, so music truly can flow out from you wherever you go. I imagine walking down the street and because the sensors on your feet are picking up a steady repetition, a beat starts up spontaneously. Then, as you're compelled to start tapping your fingers on your thigh, the sensors there begin adding a melody of some kind to this inchoate song. A personal soundtrack of new, original music at all times. This is basically my goal in life. The first requirement in moving toward this reality would be an Amanuensis for mobile devices. For this reason it might be ideal to write version 2.0 using JUCE, which I hear is totally cross-platform. A more in-depth framework and one I have not used, but if it's going to be done, it should probably be done right.

## Versions Beyond

The absolute best way to play music is with other people. If your band's not around and the AI (trained to play just like you) isn't stimulating enough, it would be great to be able to jump online and write music with any random person in the world. I find this feedback loop, the give and take with foreign minds, to be essential. Sites like JamKazam.com are great, but if augmented with The Amanuensis, they could be taken to another level. Jamming with The Amanuensis becomes a lot like a game, a far more open-ended version of Guitar Hero with the goal to score highly and create the best music possible. An online matchmaking system could be every bit like those in videogames, throwing players together to compete against (or with) each other to write songs.

And I'll raise the ante once more. There's no reason this sort of pattern detection system has to be limited to audio. If your instrument plays video in addition to audio, you're basically describing what happens in a videogame. In the same way The Amanuensis currently plays back bits of audio that you must interact and deal with, a video Amanuensis would also send visual obstacles and enemies back your way that would then inform and determine your future playing. If you're not familiar with the game Crypt of the Necrodancer, I highly recommend checking it out. What I have in mind would be something like that but on a grander scale, with a soundtrack and even the levels themselves created by and evolving with you as you play, instead of ones that are set from the beginning.