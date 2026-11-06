TSL Series · classic socialist studio hardware from the Eastern Bloc,


TSL-A34

<img width="1800" height="301" alt="tsl-a34-panel-v5 3 1" src="https://github.com/user-attachments/assets/136ba670-07e2-4c5a-9438-22d32e04d326" />



A two-channel JFET limiter / compressor built as a component-level circuit model: the whole audio board - input followers, gain stage, the JFET-controlled stage, the precision rectifier, the attack / release network, the RATIO divider and the balanced output driver - is solved as a circuit in real time.

How it works - and how it differs from a plugin compressor. This is a feedback JFET limiter, and the controls mean what they meant on the unit. There is no threshold control: the threshold is fixed by the board’s trimmers (about −6.5 dBFS at 10:1, falling to about −15.5 dBFS at 3:1). GAIN is the drive into the limiter (0 … +20 dB in front of the gain cell), not make-up gain; OUTPUT adds 0 … +6 dB after the board. RATIO moves threshold and slope together - towards 3:1 the unit starts earlier and more softly, towards 10:1 later and harder - and the knee is hard. ATTACK and RELEASE read the unit’s scale; the actual gain change is slower. The first transient after silence passes at full GAIN until the envelope has charged, and at low frequencies the envelope ripple modulates the gain within the cycle. LIMIT lights from the threshold, GAIN lights when the input stage is overdriven. BYPASS is a relay bypass: the board keeps running.

TSL-E26

<img width="1800" height="301" alt="tsl-e26-panel" src="https://github.com/user-attachments/assets/a02d197f-cf56-45f7-b4f3-2547c25e6077" />



A stepped three-band equaliser built as a component-level circuit model: the whole board - three band stages, each a resistor ladder loaded by an active resonator, the HF CUT low-pass and the output stage - is solved as a circuit in real time. Two channels, two units with their own component tolerances.

How it works - and how it differs from a plugin EQ. TSL-E26 is a stepped equaliser and the controls mean what they meant on the unit. Three bands with stepped gain (±15 dB in 3 dB steps) at switched frequencies (LOW 63 Hz – 1 kHz, MID 0.7 – 4 kHz, HI 2.8 – 11 kHz), each band a resistor ladder loaded by an active resonator. There is no Q control and the Q is not constant: the bell gets wider as the gain gets smaller - about Q 0.8 at ±15 dB, 0.5 at ±9 dB and only 0.31 at ±3 dB, so a small correction is a very broad one. The three stages are in cascade and add up where they overlap. SHELF turns the LOW or HI band into a 6 dB/octave shelf hinged at the selected frequency. HF CUT is a second-order (12 dB/oct) low-pass with −3 dB at 13 / 8.3 / 6.5 / 4.1 kHz. BYPASS is EQ OFF: the resonators are disconnected and the board passes flat. The board clips at about +1 dBFS, so large boosts on hot signals clip inside the EQ as they would in the hardware. The two channels are two units with their own component tolerances.

TSL-A95

<img width="1800" height="300" alt="tsl-a95-panel-v4 2 7" src="https://github.com/user-attachments/assets/f5449a12-5641-41df-b533-3f0b365e950e" />


A 12-bit digital delay built as a component-level circuit model: the analogue board - input stage, pre-emphasis, limiter, anti-alias and reconstruction filters, de-emphasis and the output stage - is solved as a circuit in real time around a bit-exact model of the converter, the memory and the clock.

How it works - and how it differs from a plugin delay. TSL-A95 is a 12-bit digital delay modelled part by part: pre-emphasis, a limiter and an anti-alias filter in front of a 12-bit converter, a 32k-word memory, reconstruction filter and de-emphasis after it. The delay time is RANGE (2 ... 512 ms in octaves) × FINE (×0.5 ... ×2). FINE changes the clock of the converter, so turning it while sound is in the memory shifts the pitch like tape; with HOLD the memory loops and FINE transposes it by up to an octave. The delayed signal is band-limited to about 10 kHz and 12 bits; the direct signal is clean. The limiter sits in the delay path after the pre-emphasis, so bright material lights LIMIT first and the repeats come back compressed and darker - FEEDBACK returns them through the limiter and filter again, PHASE inverts the feedback. MODULATION modulates the clock (a vibrato of the delayed sound); its depth in cents grows with RANGE. BYPASS mutes the delayed path only; POWER switches the unit off. HI drives the input 6 dB harder.







