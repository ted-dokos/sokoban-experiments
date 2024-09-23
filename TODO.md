- Figure out what's going on with KF_REPEAT, or just ignore it.
- Work on interpolation of frames.
- The horizontal movement damping is wrong.
- I am growing more skeptical of my input state idea. Should I re-phrase it as an event queue that gets consumed every update?
- You can hold down the jump key and auto-bunny-hop. Could fix that easily.

- DONE: Experiment with FPS caps in the gpu thread. When does the GPU start to chug from too many render calls?
-- Answer: my frame cap somehow prevents this from happening. At a certain point I hit ~1800 FPS and it would go no higher, despite me amping up the frame limit.
- DONE: Work on adjusting the sleep time granularity. What are the consequences for power consumption?
-- I ended up taking the power consumption from "very high" to "low" and sometimes "moderate" using timeBeginPeriod.