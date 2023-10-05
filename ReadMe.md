# Repair-Mesh

## Elevator speech
First off, chatgpt helped me reword what I was trying to say. So thanks chatgpt!

This project aims to revolutionize how we handle modern physical technology.

It has become increasingly difficult to repair and recycle our devices.

If repair wasn't already complex enough to scare would-be repair-people away, right-to-repair is threated constantly in several legal systems around the world.

I imagine:
- A non-central mesh of home-labs
  - Running automated tools made from off the shelf 3d-printer parts and web cameras
    - scanning traces, tagging/identifying known and unknown chips and components
  - consentually sharing the data as queryable among the mesh network to automate identification of novel chips
  - automatically identifying components with issues such as charing/burning, bad solder-pads
    - simply compiling a list a list of defects that the operator can share or use to examine for repair work
  - possibly even automate cost of repair estimation

Other motivations / hoped for results:
- Bring barrier-for-entry of board repair to "friend with a soldering kit" level
- Reduce electronic waste, and possibly even reverse it
- Reverse the close-sourced nature of circuit design and documentation
- Reduce manual human labor
- Reduce human intervention necessity to find issues
- Reduce the cost of repair
- Allow younger generations of humans to confidently get into the nitty-gritty of circuit engineering with less learning curve

We'll create a decentralized network where everyone can contribute their discoveries, making this a collaborative effort on a planetary scale.
You shouldn't need to be a tech genius to contribute or benefit, just someone with a passion for making a difference.

It is apparent to me that this task isn't too complex, but does infact require your help.
The software and hardware needs to be open and accessible for home-labs to reliably exchange collected circuit data for cross-referencing unknown chips and components.
This will require a lot of brain power to get to a self-sustaining level.

If you're interested, stick around:
- Eventually I'd like to have a discord server, for now, you can DM me: repcomm

If enough folks turn up interested for a discord server we'll go from there.

## technical thoughts

The above is a human-centric way to think about the project
Actually building the software and the hardware specs is more of a technical challenge.

So far I have identified these components that need to be implemented:

- A decentralized yet easy way to query boards and components
  - Known challenges include:
    - Multi-platform support vs embeded hardware solutions
    - Distributing collected data while maintaining informed consent
    - Storing decentralized data cheaply
    - Querying decentralized databases efficiently
  - Questions to get conversation going:
    - Should WebRTC be used for connecting databases for making it accessible to the most amount of home-labs possible?
    - 
- A physical system to perform scanning of physical circuit boards
  - Known challenges include:
    - Unknown chips or unknown functions of chips
    - Unmarked chips
    - Auto-tagging components that are degraded (ex: visibly burned)
    - Auto-tagging components that are MISSING
    - Auto-tagging components that are non-standard or fake
    - Multi-layer board scanning with only web camera tech may not be possible, possibly electron scanning? but this defeats a major goal-set of simplicity of implementation, populator-proliferation, and ease of safety
