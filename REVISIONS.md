# Summary of the changes applied to the manuscript
## Chapter 1 - Introduction
- [ ] test

## Chapter 2 - State of the Art
- [ ] test

## Chapter 3 - Facilitating the Development of Gesture-based Applications
- [x] Clarify that "removeGesture(name)" removes all samples from the same gesture in the gesture set. `Section 3.1.1`

## Chapter 4 - Streamlining the Evaluation of Gesture Recognizers
- [ ] test

## Chapter 5 - Designing Highly Usable Gesture-based Applications
- [x] Fix formula 5.1: P_1 should be P in the denominator. `Formula 5.1`
- [x] Explicit the modifications applied to Vatavu's $P+ recognizer in $P3+. `Section 5.2.2 - Static Gestures`

## Chapter 6 - Addressing the Challenges of Radar-based Gesture Recognition
- [x] Fix typo in computational complexity estimation: O(n ∗ k) should be O(n · k). `Section 6.2.5`

## Chapter 7 - Experimenting with Radar-based Gestures
- [ ] test

## Chapter 8 - Conclusion
- [ ] test

## Miscellaneous
- [x] Fix academic name of Luis A. Leiva. `Title page`
- [ ] Fix typos. `Everywhere`


## TODO
	Better introduce the key elements of gesture interaction, such as the difference between the various technologies (for less initiated people) (Introduction)
		§ Mid-gesture
		§ LMC VS radar
		§ Vision-based sensing technology (SOA of radar-based gesture recognition) VS. radar-based gesture interaction in general (applications, sensors, gestures, and algorithms for gesture recognition) video-based
	autres applications : applications de niche, pas limité au scrolling de large datasets. Exemple art + éducation (Introduction)
	Discuss the question of using DTW for segmentation and link to dynamic recognition (State of the art AND/OR Future works?)
	Discuss the problem of gesture discoverabiliy and their affordance (State of the art)
		§ RQ1 has been extensively researched in the past. You discussed technical challenges only, so I'd suggest to include high-level challenges such as discoverability issues (mentioned in the presentation but not in the thesis document), gorilla arm effect (not mentioned), etc
		§ Mention Gorilla-arm effect: cite "Consumed Endurance: A Metric to Quantify Arm Fatigue of Mid-Air Interactions", say how the compute the metric
		§ Intégration impossible/pas une bonne idée dans quels cas, quelles applications à part celles où on scroll, qui mobilisent un trop grand nombre de gestes : non-critical ; not for too long (State of the art - challenges)
		§ affordance des gestes, quelles solutions ? pas les 20+ gestes at once, mais une sélection raisonnée (3-7); usually about 20 sec demonstrating a given gesture + a few minutes mastering the gesture; 
		§ how about « ludification » of the learning process? Attention aux personnes plus âgées ou qui n’y arriveraient pas et qui pourraient se décourager
	-> Gesture discovery
	-> "overload" of gestures
	-> Gorilla arm
	-> Gesture set customization
	Maybe update Table 2.2 with more up-to-date references, since only 1 ref from 2021 was included. (State of the Art) Should I do it ?
	Chapter 2.2: Analysis of a Mature Sensing Technology: Why the systematic literature reviews was limited to the ACM DL? Why not IEEE? Actually, in Chapter 2.3 this search was expanded to other DLs. Some justification should be provided. (State of the art)
	Emphasize that the use of point clouds does not require convolutional layers and discuss the impact (State of the art?)
	Chapter 2.3.2: Algorithms: About CNNs (+ LSTM) predominance: It largely depends on the radar features. For example, for point clouds we don't necessarily need CNNs.
	[minor] Page 82: How is that JackKnife has 725 LOCs? It's substantailly higher than the rest of recognizers. Was it written in the same programming language? (QuantumLeap) Should I do it?
	Consider the thinking aloud as a complementary method for evaluation (Large User Interface limitations)
	evaluation protocol is mostly quanti (LSM-EPL style), how about qualitative data? Cross-analyze 
	[minor] Chapter 6.2.5 Full-wave Inversion: Have you studied the effect of angle? It's mentioned "distance d from the radar and is orthogonal to the radar-hand direction". (Radar challenges)
	In data normalization, discuss the transfer from one sensor to another one (Radar challenges)
	About data normalization: Would learned features transfer between radars or models? So many formats: FFT-based, Doppler-based, point clouds, etc.
	Explicitly include, quote, and discuss the reference Leiva:2020 (State of the art + Radar experiments)
	Chapter 7: Missing citation (shameless plug): "The wearable radar" paper. We used the same training/testing aproach as shown in Table 146.
	[minor] Gestures through materials dataset: Any thoughts about how would the results transfer/replicate between studies? See e.g. the Slovenia dataset. (Radar experiments)
	Discuss the problem of sensor fusion  (Where? State of the Art - challenges? Future works? Radar experiments conclusion with LMC+Walabot…?)

	

