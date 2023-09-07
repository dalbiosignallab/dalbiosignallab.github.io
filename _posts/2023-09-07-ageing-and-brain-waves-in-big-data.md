---
layout: post
title:  "Ageing and Brain Waves in Big Data"
date:   2023-09-07
featured_image: lotsOfData.png
tags: [Big Data, Transients, Ageing]
author_name: Tim Bardouille
---

Most neuroimaging studies contain data from tens of participants, which substantially limits the generalizability and reproducibility of the associated findings. Recent trends towards large open-access datasets have provided opportunity to address this weakness. In particular, the CamCAN dataset contains MEG, structural MRI, fMRI and demographic/cognitive data from roughly 600 participants. With an equal distribution of ages from 18-88, this dataset is ideal for cross-sectional investigation of age-related trends.

We have published a series of papers revealing age-related trends in the CamCAN dataset. The dataset includes functional imaging (MEG/fMRI) during a simple cued button press task and during wakeful resting. In particular, we have been looking at the transient signals associated with rhythmic bursts in the sensorimotor cortices. The focus has been on beta band (~20 Hz) transients, although some other signals have been investigated too.  

<!--more-->

In the cued button press task, we have showed a number of changes in burst characteristics occurring in the contralateral sensorimotor areas. These effects with age include:
+ Increasing magnitude of beta suppression
	+ Likely due to an increase in the pre-movement beta burst rate
+ Decreasing peak frequency of beta rebound
	+ Likely due to a decrease in the peak frequency of beta
+ Decreasing amplitude of beta rebound
	+ Likely due to:
		+ an increase in the pre-movement beta burst rate, and
		+ a decrease in the post-movement beta burst rate
+ Decreasing amplitude of the movement-related gamma burst
	+ The source of this change has not been investigated
+ N-shaped quadratic trend in burst power
	+ Pre-movement
	+ Post-movement
+ U-shaped quadratic trend in frequency span
	+ Pre-movement
	+ Movement
	+ Post-movement
During wakeful resting we found the following trends,
+ N-shaped quadratic trend in burst power
	+ Linear decrease in burst rate
	+ Linear decrease in burst frequency
	+ U-shaped quadratic trend in frequency span

{% include image_caption.html imageurl="/images/posts/Brady_2020_betaAgeRelatedTrends.jpg" title="Age-Related Trends in Beta Events" caption="Age-Related Trends in Beta Event Characteristics" %}

We also developed a new algorithm for generating spatial maps of (and localizing the sources of) transient events <strong>(Power, Neuroimage, 2021)</strong>. This algorithm uses minimum norm estimation to localize a change in spectral power between the pre-burst and burst intervals. MNE was preferred to beamformer for this approach, based on a qualitative comparison of the resulting maps. We showed that beta bursts have different spatial maps in wakeful resting, as compared to pre-movement, as compared to post-movement. In particular, we found an anterior shift in the spatial map for post-movement, as compared to pre-movement, which aligns with previous studies of rebound localization.

{% include image_caption.html imageurl="/images/posts/Power_2021_BetaBurstAnteriorShift.jpg" title="Age-Related Shift in Beta Event Generator" caption="Anterior Shift of Beta Event Generator with Age" %}

In terms of ageing effects, we found an anterior shift (from contralateral post-central gyrus to pre-central gyrus) in the peak location of the spatial map for the post-movement (i.e., rebound) interval and during waveful resting. As well in the post-movement interval, frontal areas (such as medial and superior frontal gyrus) showed an n-shaped quadratic trend in mean activation with age.

These are just some examples of what can be discovered thanks to the large open-access datasets available online. Here’ I’ve just talked about one type of burst (“beta”) in one area of the brain (primary sensorimotor cortex). There’s so much more to discover here, and we will continue to dig in the big data sandbox!

