TSL Series · classic socialist studio hardware from the Eastern Bloc,


TSL-A34

<img width="1800" height="301" alt="tsl-a34-panel-v5 3" src="https://github.com/user-attachments/assets/697ab1c9-61a1-4206-9f4b-e5bcd05cd675" />


A two-channel JFET limiter / compressor built as a component-level circuit model: the whole audio board - input followers, gain stage, the JFET-controlled stage, the precision rectifier, the attack / release network, the RATIO divider and the balanced output driver - is solved as a circuit in real time.

How it works - and how it differs from a plugin compressor. This is a feedback JFET limiter, and the controls mean what they meant on the unit. There is no threshold control: the threshold is fixed by the board’s trimmers (about −6.5 dBFS at 10:1, falling to about −15.5 dBFS at 3:1). GAIN is the drive into the limiter (0 … +20 dB in front of the gain cell), not make-up gain; OUTPUT adds 0 … +6 dB after the board. RATIO moves threshold and slope together - towards 3:1 the unit starts earlier and more softly, towards 10:1 later and harder - and the knee is hard. ATTACK and RELEASE read the unit’s scale; the actual gain change is slower. The first transient after silence passes at full GAIN until the envelope has charged, and at low frequencies the envelope ripple modulates the gain within the cycle. LIMIT lights from the threshold, GAIN lights when the input stage is overdriven. BYPASS is a relay bypass: the board keeps running.

TSL-E26

<img width="1800" height="301" alt="tsl-e26-panel" src="https://github.com/user-attachments/assets/b967f096-428a-4f6d-bb68-e50a6584265f" />


A stepped three-band equaliser built as a component-level circuit model: the whole board - three band stages, each a resistor ladder loaded by an active resonator, the HF CUT low-pass and the output stage - is solved as a circuit in real time. Two channels, two units with their own component tolerances.

How it works - and how it differs from a plugin EQ. TSL-E26 is a stepped equaliser and the controls mean what they meant on the unit. Three bands with stepped gain (±15 dB in 3 dB steps) at switched frequencies (LOW 63 Hz – 1 kHz, MID 0.7 – 4 kHz, HI 2.8 – 11 kHz), each band a resistor ladder loaded by an active resonator. There is no Q control and the Q is not constant: the bell gets wider as the gain gets smaller - about Q 0.8 at ±15 dB, 0.5 at ±9 dB and only 0.31 at ±3 dB, so a small correction is a very broad one. The three stages are in cascade and add up where they overlap. SHELF turns the LOW or HI band into a 6 dB/octave shelf hinged at the selected frequency. HF CUT is a second-order (12 dB/oct) low-pass with −3 dB at 13 / 8.3 / 6.5 / 4.1 kHz. BYPASS is EQ OFF: the resonators are disconnected and the board passes flat. The board clips at about +1 dBFS, so large boosts on hot signals clip inside the EQ as they would in the hardware. The two channels are two units with their own component tolerances.
