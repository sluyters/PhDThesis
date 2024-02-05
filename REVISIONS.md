# Summary of the changes applied to the manuscript
## Chapter 1 - Introduction
- [x] Better introduce key elements of gesture interaction for less-initiated readers. `Section 1.1`
  - [x] Mid-air gestures.
  - [x] Vision-based vs. radar-based sensors, LMC vs. radar.
- [x] Discuss applications of gesture recognition (healthcare, art, education). `Section 1.1`
  - [x] Where is gestural interaction appropriate?
    - Intégration impossible/pas une bonne idée dans quels cas, quelles applications à part celles où on scroll, qui mobilisent un trop grand nombre de gestes : non-critical ; not for too long

## Chapter 2 - State of the Art
- [ ] Discuss the problem of sensor fusion. `Section 2.1.2 / Sensor Limitations`
- [ ] Discuss the question of using DTW for segmentation and link to dynamic recognition. `Section 2.1.2 / Gesture Segmentation`
- [ ] Discuss UX challenges of gesture interaction. `Section 2.1.2`
  - [ ] Gesture discoverability and affordance
    - What solutions? pas les 20+ gestes at once, mais une sélection raisonnée (3-7); usually about 20 sec demonstrating a given gesture + a few minutes mastering the gesture; 
    - How about « ludification » of the learning process? Attention aux personnes plus âgées ou qui n’y arriveraient pas et qui pourraient se décourager
  - [ ] User fatigue (see "Consumed Endurance: A Metric to Quantify Arm Fatigue of Mid-Air Interactions"), mention how to compute the metric of "Gorilla-arm effect"
  - [ ] Gesture set customization
- [x] Provide a justification for limiting the SLR to the ACM DL (e.g., why not IEEE?). `Section 2.2`
- [ ] Emphasize that the use of point clouds does not require convolutional layers and discuss the impact. `Section 2.3.2 / Algorithms`
  - About CNNs (+ LSTM) predominance: It largely depends on the radar features. For example, for point clouds we don't necessarily need CNNs.

## Chapter 3 - Facilitating the Development of Gesture-based Applications
- [x] Clarify that "removeGesture(name)" removes all samples from the same gesture in the gesture set. `Section 3.1.1`

## Chapter 4 - Streamlining the Evaluation of Gesture Recognizers
No modification.

## Chapter 5 - Designing Highly Usable Gesture-based Applications
- [x] Fix formula 5.1: P_1 should be P in the denominator. `Formula 5.1`
- [x] Explicit the modifications applied to Vatavu's $P+ recognizer in $P3+. `Section 5.2.2 / Static Gestures`
- [x] Consider the thinking aloud as a complementary method for evaluation. `Section 5.4.2`
  - Evaluation protocol is mostly quanti (LSM-EPL style), how about qualitative data? Cross-analyze 

## Chapter 6 - Addressing the Challenges of Radar-based Gesture Recognition
- [x] Fix typo in computational complexity estimation: O(n ∗ k) should be O(n · k). `Section 6.2.5`
- [ ] Have you studied the effect of angle? It's mentioned "distance d from the radar and is orthogonal to the radar-hand direction". `Section 6.2.5`
- [ ] In data normalization, discuss the transfer from one sensor to another one (Radar challenges)
  - Would learned features transfer between radars or models? So many formats: FFT-based, Doppler-based, point clouds, etc.

## Chapter 7 - Experimenting with Radar-based Gestures
- [ ] Discuss the problem of sensor fusion. `Section 7.2.4`
- [ ] Gestures through materials dataset: Any thoughts about how would the results transfer/replicate between studies? See e.g. the Slovenia dataset. (Radar experiments)
- [ ] Explicitly include, quote, and discuss the reference Leiva:2020 (State of the art + Radar experiments)
  - Chapter 7: Missing citation (shameless plug): "The wearable radar" paper. We used the same training/testing aproach as shown in Table 146.

## Chapter 8 - Conclusion
- [ ] Discuss the problem of sensor fusion. `Section 8.2`

## Miscellaneous
- [x] Fix academic name of Luis A. Leiva. `Title page`
- [ ] Fix typos. `Everywhere`

## Suggested modifications not applied to the revised thesis
- 	Update Table 2.2 with more up-to-date references, since only 1 ref from 2021 was included.
- 	Explain why JackKnife has 725 LOCs? It's substantailly higher than the rest of recognizers. Was it written in the same programming language?

	

